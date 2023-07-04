# Comparing `tmp/tencentcloud-sdk-python-nlp-3.0.926.tar.gz` & `tmp/tencentcloud-sdk-python-nlp-3.0.927.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.926.tar", last modified: Mon Jul  3 00:31:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.927.tar", last modified: Tue Jul  4 00:26:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-nlp-3.0.926.tar` & `tencentcloud-sdk-python-nlp-3.0.927.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/setup.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/tencentcloud_sdk_python_nlp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/tencentcloud/nlp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/tencentcloud/nlp/v20190408/
--rw-r--r--   0 root         (0) root         (0)    90360 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/tencentcloud/nlp/v20190408/models.py
--rw-r--r--   0 root         (0) root         (0)     6090 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/tencentcloud/nlp/v20190408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/tencentcloud/nlp/v20190408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49107 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/tencentcloud/nlp/v20190408/nlp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:31:22.000000 tencentcloud-sdk-python-nlp-3.0.926/tencentcloud/nlp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:26:31.000000 tencentcloud-sdk-python-nlp-3.0.927/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:26:31.000000 tencentcloud-sdk-python-nlp-3.0.927/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-04 00:26:30.000000 tencentcloud-sdk-python-nlp-3.0.927/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:26:31.000000 tencentcloud-sdk-python-nlp-3.0.927/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-04 00:26:30.000000 tencentcloud-sdk-python-nlp-3.0.927/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:26:31.000000 tencentcloud-sdk-python-nlp-3.0.927/tencentcloud_sdk_python_nlp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-04 00:26:31.000000 tencentcloud-sdk-python-nlp-3.0.927/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:26:31.000000 tencentcloud-sdk-python-nlp-3.0.927/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:26:31.000000 tencentcloud-sdk-python-nlp-3.0.927/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:26:31.000000 tencentcloud-sdk-python-nlp-3.0.927/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:26:31.000000 tencentcloud-sdk-python-nlp-3.0.927/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:26:30.000000 tencentcloud-sdk-python-nlp-3.0.927/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:26:31.000000 tencentcloud-sdk-python-nlp-3.0.927/tencentcloud/nlp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:26:31.000000 tencentcloud-sdk-python-nlp-3.0.927/tencentcloud/nlp/v20190408/
+-rw-r--r--   0 root         (0) root         (0)     6090 2023-07-04 00:26:30.000000 tencentcloud-sdk-python-nlp-3.0.927/tencentcloud/nlp/v20190408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    90359 2023-07-04 00:26:30.000000 tencentcloud-sdk-python-nlp-3.0.927/tencentcloud/nlp/v20190408/models.py
+-rw-r--r--   0 root         (0) root         (0)    49107 2023-07-04 00:26:30.000000 tencentcloud-sdk-python-nlp-3.0.927/tencentcloud/nlp/v20190408/nlp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:26:30.000000 tencentcloud-sdk-python-nlp-3.0.927/tencentcloud/nlp/v20190408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:26:30.000000 tencentcloud-sdk-python-nlp-3.0.927/tencentcloud/nlp/__init__.py
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.926/setup.py` & `tencentcloud-sdk-python-nlp-3.0.927/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.926/README.rst` & `tencentcloud-sdk-python-nlp-3.0.927/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.926/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.927/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.926
+Version: 3.0.927
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.926/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.927/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.926
+Version: 3.0.927
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.926/tencentcloud/__init__.py` & `tencentcloud-sdk-python-nlp-3.0.927/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-nlp-3.0.926/tencentcloud/nlp/v20190408/models.py` & `tencentcloud-sdk-python-nlp-3.0.927/tencentcloud/nlp/v20190408/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1218,15 +1218,15 @@
 class EvaluateSentenceSimilarityRequest(AbstractModel):
     """EvaluateSentenceSimilarity请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param SentencePairList: 待分析的句子对数组。句子对应不超过5对，支持中英文文本，原句子与目标句子均应不超过500字符。
+        :param SentencePairList: 待分析的句子对数组。句子对应不超过1对，仅支持中文文本，原句子与目标句子均应不超过64字符。
         :type SentencePairList: list of SentencePair
         """
         self.SentencePairList = None
 
 
     def _deserialize(self, params):
         if params.get("SentencePairList") is not None:
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.926/tencentcloud/nlp/v20190408/errorcodes.py` & `tencentcloud-sdk-python-nlp-3.0.927/tencentcloud/nlp/v20190408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.926/tencentcloud/nlp/v20190408/nlp_client.py` & `tencentcloud-sdk-python-nlp-3.0.927/tencentcloud/nlp/v20190408/nlp_client.py`

 * *Files identical despite different names*

