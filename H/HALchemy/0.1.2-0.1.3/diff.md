# Comparing `tmp/HALchemy-0.1.2-py3-none-any.whl.zip` & `tmp/HALchemy-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 4861 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     6850 b- defN 23-Jul-04 00:58 halchemy/halchemy.py
+Zip file size: 5070 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       73 b- defN 23-Jul-04 01:21 halchemy/__init__.py
+-rw-rw-rw-  2.0 fat     6851 b- defN 23-Jul-04 01:21 halchemy/api.py
 -rw-rw-rw-  2.0 fat     2548 b- defN 23-Jul-01 18:46 halchemy/requests_helper.py
--rw-rw-rw-  2.0 fat      669 b- defN 23-Jul-04 01:12 HALchemy-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 01:12 HALchemy-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-04 01:12 HALchemy-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      461 b- defN 23-Jul-04 01:12 HALchemy-0.1.2.dist-info/RECORD
-6 files, 10629 bytes uncompressed, 4025 bytes compressed:  62.1%
+-rw-rw-rw-  2.0 fat      669 b- defN 23-Jul-04 01:23 HALchemy-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 01:23 HALchemy-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-04 01:23 HALchemy-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      531 b- defN 23-Jul-04 01:23 HALchemy-0.1.3.dist-info/RECORD
+7 files, 10773 bytes uncompressed, 4128 bytes compressed:  61.7%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
-Filename: halchemy/halchemy.py
+Filename: halchemy/__init__.py
+Comment: 
+
+Filename: halchemy/api.py
 Comment: 
 
 Filename: halchemy/requests_helper.py
 Comment: 
 
-Filename: HALchemy-0.1.2.dist-info/METADATA
+Filename: HALchemy-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: HALchemy-0.1.2.dist-info/WHEEL
+Filename: HALchemy-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: HALchemy-0.1.2.dist-info/top_level.txt
+Filename: HALchemy-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: HALchemy-0.1.2.dist-info/RECORD
+Filename: HALchemy-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `halchemy/halchemy.py` & `halchemy/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
     SOFTWARE.
 """
 
 import json
-from requests_helper import requests, RequestsWithDefaults
+from .requests_helper import requests, RequestsWithDefaults
 import socket
 import re
 import sys
 from urllib.parse import urlencode
 
 
 class Api:
```

## Comparing `HALchemy-0.1.2.dist-info/METADATA` & `HALchemy-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HALchemy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Toolkit for creating clients of HAL based Hypermedia APIs.
 Home-page: https://github.com/pointw-dev/HALchemy
 Author: Michael Ottoson
 Author-email: michael@pointw.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
```

