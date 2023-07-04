# Comparing `tmp/tencentcloud-sdk-python-tcr-3.0.926.tar.gz` & `tmp/tencentcloud-sdk-python-tcr-3.0.927.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcr-3.0.926.tar", last modified: Mon Jul  3 00:35:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcr-3.0.927.tar", last modified: Tue Jul  4 00:30:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcr-3.0.926.tar` & `tencentcloud-sdk-python-tcr-3.0.927.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:35:20.000000 tencentcloud-sdk-python-tcr-3.0.926/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:35:20.000000 tencentcloud-sdk-python-tcr-3.0.926/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:35:20.000000 tencentcloud-sdk-python-tcr-3.0.926/tencentcloud_sdk_python_tcr.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-03 00:35:20.000000 tencentcloud-sdk-python-tcr-3.0.926/tencentcloud_sdk_python_tcr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:35:20.000000 tencentcloud-sdk-python-tcr-3.0.926/tencentcloud_sdk_python_tcr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:35:20.000000 tencentcloud-sdk-python-tcr-3.0.926/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:35:20.000000 tencentcloud-sdk-python-tcr-3.0.926/tencentcloud_sdk_python_tcr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-03 00:35:19.000000 tencentcloud-sdk-python-tcr-3.0.926/setup.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-03 00:35:19.000000 tencentcloud-sdk-python-tcr-3.0.926/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:35:20.000000 tencentcloud-sdk-python-tcr-3.0.926/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:35:20.000000 tencentcloud-sdk-python-tcr-3.0.926/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:35:20.000000 tencentcloud-sdk-python-tcr-3.0.926/tencentcloud/tcr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:35:20.000000 tencentcloud-sdk-python-tcr-3.0.926/tencentcloud/tcr/v20190924/
--rw-r--r--   0 root         (0) root         (0)   269587 2023-07-03 00:35:19.000000 tencentcloud-sdk-python-tcr-3.0.926/tencentcloud/tcr/v20190924/models.py
--rw-r--r--   0 root         (0) root         (0)   100588 2023-07-03 00:35:19.000000 tencentcloud-sdk-python-tcr-3.0.926/tencentcloud/tcr/v20190924/tcr_client.py
--rw-r--r--   0 root         (0) root         (0)     8520 2023-07-03 00:35:19.000000 tencentcloud-sdk-python-tcr-3.0.926/tencentcloud/tcr/v20190924/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:35:19.000000 tencentcloud-sdk-python-tcr-3.0.926/tencentcloud/tcr/v20190924/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:35:19.000000 tencentcloud-sdk-python-tcr-3.0.926/tencentcloud/tcr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:35:19.000000 tencentcloud-sdk-python-tcr-3.0.926/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/tencentcloud_sdk_python_tcr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/tencentcloud_sdk_python_tcr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/tencentcloud_sdk_python_tcr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/tencentcloud_sdk_python_tcr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/tencentcloud/tcr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/tencentcloud/tcr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/tencentcloud/tcr/v20190924/
+-rw-r--r--   0 root         (0) root         (0)     8520 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/tencentcloud/tcr/v20190924/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   269587 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/tencentcloud/tcr/v20190924/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/tencentcloud/tcr/v20190924/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   100588 2023-07-04 00:30:39.000000 tencentcloud-sdk-python-tcr-3.0.927/tencentcloud/tcr/v20190924/tcr_client.py
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.926/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcr-3.0.927/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcr
-Version: 3.0.926
+Version: 3.0.927
 Summary: Tencent Cloud Tcr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.926/setup.py` & `tencentcloud-sdk-python-tcr-3.0.927/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcr-3.0.926/README.rst` & `tencentcloud-sdk-python-tcr-3.0.927/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcr-3.0.926/PKG-INFO` & `tencentcloud-sdk-python-tcr-3.0.927/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcr
-Version: 3.0.926
+Version: 3.0.927
 Summary: Tencent Cloud Tcr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.926/tencentcloud/tcr/v20190924/models.py` & `tencentcloud-sdk-python-tcr-3.0.927/tencentcloud/tcr/v20190924/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcr-3.0.926/tencentcloud/tcr/v20190924/tcr_client.py` & `tencentcloud-sdk-python-tcr-3.0.927/tencentcloud/tcr/v20190924/tcr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcr-3.0.926/tencentcloud/tcr/v20190924/errorcodes.py` & `tencentcloud-sdk-python-tcr-3.0.927/tencentcloud/tcr/v20190924/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcr-3.0.926/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcr-3.0.927/tencentcloud/__init__.py`

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

