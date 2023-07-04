# Comparing `tmp/cqi-0.1.2.tar.gz` & `tmp/cqi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqi-0.1.2.tar", last modified: Thu Jun 29 10:15:01 2023, max compression
+gzip compressed data, was "cqi-0.1.3.tar", last modified: Tue Jul  4 07:07:36 2023, max compression
```

## Comparing `cqi-0.1.2.tar` & `cqi-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-29 10:15:01.528545 cqi-0.1.2/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1072 2023-06-22 07:21:07.000000 cqi-0.1.2/LICENSE
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1576 2023-06-29 10:15:01.518545 cqi-0.1.2/PKG-INFO
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1090 2023-06-29 10:11:38.000000 cqi-0.1.2/README.md
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-29 10:15:01.518545 cqi-0.1.2/cqi/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      166 2023-06-22 09:48:22.000000 cqi-0.1.2/cqi/__init__.py
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-29 10:15:01.518545 cqi-0.1.2/cqi/api/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       45 2023-06-22 09:48:22.000000 cqi-0.1.2/cqi/api/__init__.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    20849 2023-06-29 09:21:22.000000 cqi-0.1.2/cqi/api/client.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    12641 2023-06-22 09:48:22.000000 cqi-0.1.2/cqi/api/specification.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1934 2023-06-29 08:20:25.000000 cqi-0.1.2/cqi/client.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     5016 2023-06-28 11:38:07.000000 cqi-0.1.2/cqi/errors.py
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-29 10:15:01.518545 cqi-0.1.2/cqi/models/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 09:48:22.000000 cqi-0.1.2/cqi/models/__init__.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     7097 2023-06-29 08:09:02.000000 cqi-0.1.2/cqi/models/attributes.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2599 2023-06-29 09:22:31.000000 cqi-0.1.2/cqi/models/corpora.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2345 2023-06-29 08:07:30.000000 cqi-0.1.2/cqi/models/resource.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     3927 2023-06-29 08:08:13.000000 cqi-0.1.2/cqi/models/subcorpora.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1084 2023-06-22 09:48:22.000000 cqi-0.1.2/cqi/status.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      145 2023-06-29 10:10:28.000000 cqi-0.1.2/cqi/version.py
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-29 10:15:01.518545 cqi-0.1.2/cqi.egg-info/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1576 2023-06-29 10:15:01.000000 cqi-0.1.2/cqi.egg-info/PKG-INFO
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      388 2023-06-29 10:15:01.000000 cqi-0.1.2/cqi.egg-info/SOURCES.txt
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        1 2023-06-29 10:15:01.000000 cqi-0.1.2/cqi.egg-info/dependency_links.txt
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        4 2023-06-29 10:15:01.000000 cqi-0.1.2/cqi.egg-info/top_level.txt
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       38 2023-06-29 10:15:01.528545 cqi-0.1.2/setup.cfg
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      781 2023-06-22 07:21:07.000000 cqi-0.1.2/setup.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-04 07:07:36.728287 cqi-0.1.3/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1072 2023-06-22 07:21:07.000000 cqi-0.1.3/LICENSE
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1615 2023-07-04 07:07:36.728287 cqi-0.1.3/PKG-INFO
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1129 2023-07-04 07:07:09.000000 cqi-0.1.3/README.md
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-04 07:07:36.728287 cqi-0.1.3/cqi/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      166 2023-06-22 09:48:22.000000 cqi-0.1.3/cqi/__init__.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-04 07:07:36.728287 cqi-0.1.3/cqi/api/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       45 2023-06-22 09:48:22.000000 cqi-0.1.3/cqi/api/__init__.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    20426 2023-07-03 11:30:33.000000 cqi-0.1.3/cqi/api/client.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    12641 2023-06-22 09:48:22.000000 cqi-0.1.3/cqi/api/specification.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1798 2023-06-30 12:05:11.000000 cqi-0.1.3/cqi/client.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     4963 2023-07-03 10:18:41.000000 cqi-0.1.3/cqi/errors.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-04 07:07:36.728287 cqi-0.1.3/cqi/models/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 09:48:22.000000 cqi-0.1.3/cqi/models/__init__.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     7077 2023-07-04 06:47:57.000000 cqi-0.1.3/cqi/models/attributes.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2789 2023-07-04 07:00:23.000000 cqi-0.1.3/cqi/models/corpora.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2374 2023-07-04 06:58:38.000000 cqi-0.1.3/cqi/models/resource.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     3911 2023-07-04 06:55:29.000000 cqi-0.1.3/cqi/models/subcorpora.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1077 2023-07-03 10:13:19.000000 cqi-0.1.3/cqi/status.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      145 2023-07-04 07:01:59.000000 cqi-0.1.3/cqi/version.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-04 07:07:36.728287 cqi-0.1.3/cqi.egg-info/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1615 2023-07-04 07:07:36.000000 cqi-0.1.3/cqi.egg-info/PKG-INFO
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      388 2023-07-04 07:07:36.000000 cqi-0.1.3/cqi.egg-info/SOURCES.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        1 2023-07-04 07:07:36.000000 cqi-0.1.3/cqi.egg-info/dependency_links.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        4 2023-07-04 07:07:36.000000 cqi-0.1.3/cqi.egg-info/top_level.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       38 2023-07-04 07:07:36.728287 cqi-0.1.3/setup.cfg
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      781 2023-06-22 07:21:07.000000 cqi-0.1.3/setup.py
```

### Comparing `cqi-0.1.2/LICENSE` & `cqi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cqi-0.1.2/PKG-INFO` & `cqi-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqi
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library for the IMS Open Corpus Workbench (CWB) corpus query interface (CQi) API.
 Home-page: https://github.com/Pevtrick/cqi-py
 Author: Patrick Jentsch
 Author-email: patrickjentsch@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,14 +27,15 @@
 ## Version compatibility
 
 | Package version | Protocol version |
 |-----------------|------------------|
 | 0.1.0           | 0.1              |
 | 0.1.1           | 0.1              |
 | 0.1.2           | 0.1              |
+| 0.1.3           | 0.1              |
 
 ## Usage
 
 ```python
 import cqi
```

### Comparing `cqi-0.1.2/README.md` & `cqi-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ## Version compatibility
 
 | Package version | Protocol version |
 |-----------------|------------------|
 | 0.1.0           | 0.1              |
 | 0.1.1           | 0.1              |
 | 0.1.2           | 0.1              |
+| 0.1.3           | 0.1              |
 
 ## Usage
 
 ```python
 import cqi
```

### Comparing `cqi-0.1.2/cqi/api/client.py` & `cqi-0.1.3/cqi/api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import List, Tuple
-import math
 import socket
 import struct
 import time
 from . import specification
 from .. import errors
 from .. import status
 
@@ -24,30 +23,29 @@
     259  # CQI_STATUS_BYE_OK
 
     Attributes:
     host (str): URL to the CQP server. For example,
         ``cqpserver.localhost`` or ``127.0.0.1``.
     port (int): Port the CQP server listens on. Default: ``4877``
     socket (socket.socket): Socket for communicating with a CQP server.
-    timeout (int): Time to wait for bytes from the server. If the timeout is
-        exceeded, an exception is raised. Default: ``math.inf``
+    timeout (int): Default timeout for API calls, in seconds. Default: ``60``
     version (str): The version of the CQi protocol to use. Default: ``0.1``
     '''
 
     def __init__(
         self,
         host: str,
         port: int = 4877,
-        timeout: float = math.inf,
+        timeout: int = 60,
         version: str = '0.1'
     ):
         self.host: str = host
         self.port: int = port
         self.socket: socket.socket = socket.socket()
-        self.timeout: float = timeout
+        self.timeout: int = timeout
         self.version: str = version
 
     def ctrl_connect(
         self,
         username: str,
         password: str
     ) -> status.StatusConnectOk:
@@ -428,26 +426,20 @@
         self.__send_BYTE(field2)
         self.__send_STRING(attribute2)
         return self.__recv_response()
 
     def __recv_response(self):
         byte_data = self.__recv_WORD()
         response_type = byte_data >> 8
-        if response_type == specification.CL_ERROR:
-            raise errors.cl_error_lookup[byte_data]()
-        elif response_type == specification.CQP_ERROR:
-            raise errors.cqp_error_lookup[byte_data]()
-        elif response_type == specification.DATA:
+        if response_type == specification.DATA:
             return self.__recv_DATA(byte_data)
-        elif response_type == specification.ERROR:
-            raise errors.error_lookup[byte_data]()
         elif response_type == specification.STATUS:
-            return status.status_lookup[byte_data]()
+            return status.lookup[byte_data]()
         else:
-            raise errors.CQiException(f'Unknown response type: {response_type}')
+            raise errors.lookup.get(byte_data, errors.CQiException)()
 
     def __recv_DATA(self, data_type):
         if data_type == specification.DATA_BYTE:
             return self.__recv_DATA_BYTE()
         elif data_type == specification.DATA_BOOL:
             return self.__recv_DATA_BOOL()
         elif data_type == specification.DATA_INT:
```

### Comparing `cqi-0.1.2/cqi/api/specification.py` & `cqi-0.1.3/cqi/api/specification.py`

 * *Files identical despite different names*

### Comparing `cqi-0.1.2/cqi/client.py` & `cqi-0.1.3/cqi/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .status import StatusByeOk, StatusConnectOk, StatusPingOk
-import math
 from .api import APIClient
 from .models.corpora import CorpusCollection
 
 
 
 class CQiClient:
     '''
@@ -25,26 +24,25 @@
     api (APIClient): An API client pointing to the specified CQP server.
     '''
 
     def __init__(
         self,
         host: str,
         port: int = 4877,
-        timeout: float = math.inf,
+        timeout: int = 60,
         version: str = '0.1'
     ):
         '''
         CQiClient constructor
 
         Args:
         host (str): URL to the CQP server. For example,
             ``cqpserver.localhost`` or ``127.0.0.1``.
         port (int): Port the CQP server listens on. Default: ``4877``
-        timeout (int): Time to wait for bytes from the server. If the timeout
-            is exceeded, an exception is raised. Default: ``math.inf``
+        timeout (int): Default timeout for API calls, in seconds. Default: ``60``
         version (str): The version of the CQi protocol to use. Default: ``0.1``
         '''
         self.api: APIClient = APIClient(
             host,
             port=port,
             timeout=timeout,
             version=version
@@ -53,19 +51,15 @@
     @property
     def corpora(self) -> CorpusCollection:
         return CorpusCollection(client=self)
 
     def bye(self) -> 'StatusByeOk':
         return self.api.ctrl_bye()
 
-    def connect(
-        self,
-        username: str = 'anonymous',
-        password: str = ''
-    ) -> 'StatusConnectOk':
+    def connect(self, username: str, password: str) -> 'StatusConnectOk':
         return self.api.ctrl_connect(username, password)
 
     def ping(self) -> 'StatusPingOk':
         return self.api.ctrl_ping()
 
     def user_abort(self):
         self.api.ctrl_user_abort()
```

### Comparing `cqi-0.1.2/cqi/errors.py` & `cqi-0.1.3/cqi/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,35 +129,27 @@
 class CQPErrorOutOfRange(CQPError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CQP_ERROR_OUT_OF_RANGE
         self.description = 'A number is out of range'
 
 
-error_lookup = {
+lookup = {
     specification.ERROR: Error,
     specification.ERROR_GENERAL_ERROR: ErrorGeneralError,
     specification.ERROR_CONNECT_REFUSED: ErrorConnectRefused,
     specification.ERROR_USER_ABORT: ErrorUserAbort,
-    specification.ERROR_SYNTAX_ERROR: ErrorSyntaxError
-}
-
-
-cl_error_lookup = {
+    specification.ERROR_SYNTAX_ERROR: ErrorSyntaxError,
     specification.CL_ERROR: CLError,
     specification.CL_ERROR_NO_SUCH_ATTRIBUTE: CLErrorNoSuchAttribute,
     specification.CL_ERROR_WRONG_ATTRIBUTE_TYPE: CLErrorWrongAttributeType,
     specification.CL_ERROR_OUT_OF_RANGE: CLErrorOutOfRange,
     specification.CL_ERROR_REGEX: CLErrorRegex,
     specification.CL_ERROR_CORPUS_ACCESS: CLErrorCorpusAccess,
     specification.CL_ERROR_OUT_OF_MEMORY: CLErrorOutOfMemory,
-    specification.CL_ERROR_INTERNAL: CLErrorInternal
-}
-
-
-cqp_error_lookup = {
+    specification.CL_ERROR_INTERNAL: CLErrorInternal,
     specification.CQP_ERROR: CQPError,
     specification.CQP_ERROR_GENERAL: CQPErrorGeneral,
     specification.CQP_ERROR_NO_SUCH_CORPUS: CQPErrorNoSuchCorpus,
     specification.CQP_ERROR_INVALID_FIELD: CQPErrorInvalidField,
     specification.CQP_ERROR_OUT_OF_RANGE: CQPErrorOutOfRange
 }
```

### Comparing `cqi-0.1.2/cqi/models/attributes.py` & `cqi-0.1.3/cqi/models/attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
     from .corpora import Corpus
 from .resource import Collection, Model
 
 
 class Attribute(Model):
     @property
     def api_name(self) -> str:
-        return self.attrs.get('api_name')
+        return self.attrs['api_name']
 
     @property
     def name(self) -> str:
-        return self.attrs.get('name')
+        return self.attrs['name']
 
     @property
     def size(self) -> int:
-        return self.attrs.get('size')
+        return self.attrs['size']
 
     def drop(self) -> 'StatusOk':
         ''' unload attribute from memory '''
         return self.client.api.cl_drop_attribute(self.api_name)
 
 
 class AttributeCollection(Collection):
@@ -65,15 +65,15 @@
             self.client.api.corpus_alignment_attributes(self.corpus.api_name)
         ]
 
 
 class PositionalAttribute(Attribute):
     @property
     def lexicon_size(self) -> int:
-        return self.attrs.get('lexicon_size')
+        return self.attrs['lexicon_size']
 
     def cpos_by_id(self, id: int) -> List[int]:
         ''' returns all corpus positions where the given token occurs '''
         return self.client.api.cl_id2cpos(self.api_name, id)
 
     def cpos_by_ids(self, id_list: List[int]) -> List[int]:
         '''
@@ -133,15 +133,15 @@
             self.client.api.corpus_positional_attributes(self.corpus.api_name)
         ]
 
 
 class StructuralAttribute(Attribute):
     @property
     def has_values(self) -> bool:
-        return self.attrs.get('has_values')
+        return self.attrs['has_values']
 
     def cpos_by_id(self, id: int) -> Tuple[int, int]:
         '''
         returns start and end corpus positions of structure region with id
         <id>
         '''
         return self.client.api.cl_struc2cpos(self.api_name, id)
```

### Comparing `cqi-0.1.2/cqi/models/corpora.py` & `cqi-0.1.3/cqi/models/corpora.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 from .resource import Collection, Model
 from .subcorpora import SubcorpusCollection
 
 
 class Corpus(Model):
     @property
     def api_name(self) -> str:
-        return self.attrs.get('api_name')
+        return self.attrs['api_name']
 
     @property
     def name(self) -> str:
-        return self.attrs.get('name')
+        return self.attrs['name']
 
     @property
     def size(self) -> int:
-        return self.attrs.get('size')
+        return self.attrs['size']
 
     @property
     def charset(self) -> str:
-        return self.attrs.get('charset')
+        return self.attrs['charset']
 
     @property
     def properties(self) -> List[str]:
-        return self.attrs.get('properties')
+        return self.attrs['properties']
 
     @property
     def alignment_attributes(self) -> AlignmentAttributeCollection:
         return AlignmentAttributeCollection(client=self.client, corpus=self)
 
     @property
     def positional_attributes(self) -> PositionalAttributeCollection:
@@ -57,22 +57,27 @@
 
 
 class CorpusCollection(Collection):
     model: Type[Corpus] = Corpus
 
     def _get(self, corpus_name: str) -> Dict:
         api_name: str = corpus_name
+        p_attr_names: List[str] = self.client.api.corpus_positional_attributes(api_name)
+        corpus_size: int = (
+            0 if len(p_attr_names) == 0 else
+            self.client.api.cl_attribute_size(f'{api_name}.{p_attr_names[0]}')
+        )
         return {
             'api_name': api_name,
             'charset': self.client.api.corpus_charset(api_name),
             # 'full_name': self.client.api.corpus_full_name(api_name),
             # 'info': self.client.api.corpus_info(api_name),
             'name': corpus_name,
             'properties': self.client.api.corpus_properties(api_name),
-            'size': self.client.api.cl_attribute_size(f'{api_name}.word')
+            'size': corpus_size
         }
 
     def get(self, corpus_name: str) -> Corpus:
         return self.prepare_model(self._get(corpus_name))
 
     def list(self) -> List[Corpus]:
         return [self.get(x) for x in self.client.api.corpus_list_corpora()]
```

### Comparing `cqi-0.1.2/cqi/models/resource.py` & `cqi-0.1.3/cqi/models/resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,24 @@
         #: The collection that this model is part of.
         self.collection: Collection = collection
 
         #: The raw representation of this object from the API
         self.attrs: Dict = attrs or {}
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__}: {self.id}>'
+        return f'<{self.__class__.__name__}: {self.api_name}>'
 
     def __eq__(self, other) -> bool:
-        return isinstance(other, self.__class__) and self.id == other.id
+        return (
+            isinstance(other, self.__class__)
+            and self.api_name == other.api_name
+        )
 
     def __hash__(self) -> int:
-        return hash(f'{self.__class__.__name__}:{self.id}')
+        return hash(f'{self.__class__.__name__}:{self.api_name}')
 
     @property
     def api_name(self) -> str:
         raise NotImplementedError
 
     def reload(self):
         '''
@@ -75,10 +78,8 @@
         elif isinstance(attrs, dict):
             return self.model(
                 attrs=attrs,
                 client=self.client,
                 collection=self
             )
         else:
-            raise Exception(
-                f'Can\'t create {self.model.__name__} from {attrs}'
-            )
+            raise Exception(f"Can't create {self.model.__name__} from {attrs}")
```

### Comparing `cqi-0.1.2/cqi/models/subcorpora.py` & `cqi-0.1.3/cqi/models/subcorpora.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 )
 from .resource import Collection, Model
 
 
 class Subcorpus(Model):
     @property
     def api_name(self) -> str:
-        return self.attrs.get('api_name')
+        return self.attrs['api_name']
 
     @property
     def fields(self) -> Dict[str, int]:
-        return self.attrs.get('fields')
+        return self.attrs['fields']
 
     @property
     def name(self) -> str:
-        return self.attrs.get('name')
+        return self.attrs['name']
 
     @property
     def size(self) -> int:
-        return self.attrs.get('size')
+        return self.attrs['size']
 
     def drop(self) -> 'StatusOk':
         ''' delete a subcorpus from memory '''
         return self.client.api.cqp_drop_subcorpus(self.api_name)
 
     def dump(self, field: int, first: int, last: int) -> List[int]:
         '''
```

### Comparing `cqi-0.1.2/cqi/status.py` & `cqi-0.1.3/cqi/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,13 +29,13 @@
 
 class StatusPingOk(CQiStatus):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.STATUS_PING_OK
 
 
-status_lookup = {
+lookup = {
     specification.STATUS_OK: StatusOk,
     specification.STATUS_CONNECT_OK: StatusConnectOk,
     specification.STATUS_BYE_OK: StatusByeOk,
     specification.STATUS_PING_OK: StatusPingOk
 }
```

### Comparing `cqi-0.1.2/cqi.egg-info/PKG-INFO` & `cqi-0.1.3/cqi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqi
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library for the IMS Open Corpus Workbench (CWB) corpus query interface (CQi) API.
 Home-page: https://github.com/Pevtrick/cqi-py
 Author: Patrick Jentsch
 Author-email: patrickjentsch@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,14 +27,15 @@
 ## Version compatibility
 
 | Package version | Protocol version |
 |-----------------|------------------|
 | 0.1.0           | 0.1              |
 | 0.1.1           | 0.1              |
 | 0.1.2           | 0.1              |
+| 0.1.3           | 0.1              |
 
 ## Usage
 
 ```python
 import cqi
```

### Comparing `cqi-0.1.2/setup.py` & `cqi-0.1.3/setup.py`

 * *Files identical despite different names*

