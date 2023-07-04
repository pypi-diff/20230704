# Comparing `tmp/tencentcloud-sdk-python-chdfs-3.0.926.tar.gz` & `tmp/tencentcloud-sdk-python-chdfs-3.0.927.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-chdfs-3.0.926.tar", last modified: Mon Jul  3 00:21:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-chdfs-3.0.927.tar", last modified: Tue Jul  4 00:17:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-chdfs-3.0.926.tar` & `tencentcloud-sdk-python-chdfs-3.0.927.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/setup.py
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud_sdk_python_chdfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud_sdk_python_chdfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud_sdk_python_chdfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud_sdk_python_chdfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud_sdk_python_chdfs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/v20190718/
--rw-r--r--   0 root         (0) root         (0)    51568 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/v20190718/models.py
--rw-r--r--   0 root         (0) root         (0)    28022 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/v20190718/chdfs_client.py
--rw-r--r--   0 root         (0) root         (0)     3280 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/v20190718/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/v20190718/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/v20201112/
--rw-r--r--   0 root         (0) root         (0)    60336 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/v20201112/models.py
--rw-r--r--   0 root         (0) root         (0)    27286 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/v20201112/chdfs_client.py
--rw-r--r--   0 root         (0) root         (0)     3600 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/v20201112/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/v20201112/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:21:57.000000 tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud_sdk_python_chdfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud_sdk_python_chdfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud_sdk_python_chdfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud_sdk_python_chdfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud_sdk_python_chdfs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/v20201112/
+-rw-r--r--   0 root         (0) root         (0)     3600 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/v20201112/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    60336 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/v20201112/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/v20201112/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27286 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/v20201112/chdfs_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/v20190718/
+-rw-r--r--   0 root         (0) root         (0)     3280 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/v20190718/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    51568 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/v20190718/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/v20190718/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28022 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/v20190718/chdfs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:17:34.000000 tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/__init__.py
```

### Comparing `tencentcloud-sdk-python-chdfs-3.0.926/setup.py` & `tencentcloud-sdk-python-chdfs-3.0.927/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.926/README.rst` & `tencentcloud-sdk-python-chdfs-3.0.927/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud_sdk_python_chdfs.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud_sdk_python_chdfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud_sdk_python_chdfs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-chdfs-3.0.927/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-chdfs
-Version: 3.0.926
+Version: 3.0.927
 Summary: Tencent Cloud Chdfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-chdfs-3.0.926/PKG-INFO` & `tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud_sdk_python_chdfs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-chdfs
-Version: 3.0.926
+Version: 3.0.927
 Summary: Tencent Cloud Chdfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/__init__.py` & `tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/v20190718/models.py` & `tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/v20190718/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/v20190718/chdfs_client.py` & `tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/v20190718/chdfs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/v20190718/errorcodes.py` & `tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/v20190718/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/v20201112/models.py` & `tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/v20201112/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/v20201112/chdfs_client.py` & `tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/v20201112/chdfs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.926/tencentcloud/chdfs/v20201112/errorcodes.py` & `tencentcloud-sdk-python-chdfs-3.0.927/tencentcloud/chdfs/v20201112/errorcodes.py`

 * *Files identical despite different names*

