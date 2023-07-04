# Comparing `tmp/xata-0.9.3.tar.gz` & `tmp/xata-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xata-0.9.3.tar", max compression
+gzip compressed data, was "xata-1.0.0a1.tar", max compression
```

## Comparing `xata-0.9.3.tar` & `xata-1.0.0a1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2023-04-27 12:49:08.009065 xata-0.9.3/LICENSE
--rw-r--r--   0        0        0     1156 2023-04-27 12:49:08.009065 xata-0.9.3/README.md
--rw-r--r--   0        0        0      749 2023-04-27 12:49:08.033046 xata-0.9.3/pyproject.toml
--rw-r--r--   0        0        0      858 2023-04-27 12:49:08.037043 xata-0.9.3/xata/__init__.py
--rw-r--r--   0        0        0    31963 2023-04-27 12:49:08.037043 xata-0.9.3/xata/client.py
--rw-r--r--   0        0        0     1715 2023-04-27 12:49:08.037043 xata-0.9.3/xata/errors.py
--rw-r--r--   0        0        0    11090 2023-04-27 12:49:08.037043 xata-0.9.3/xata/helpers.py
--rw-r--r--   0        0        0     2114 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespace.py
--rw-r--r--   0        0        0      769 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/__init__.py
--rw-r--r--   0        0        0      769 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/core/__init__.py
--rw-r--r--   0        0        0     2666 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/core/authentication.py
--rw-r--r--   0        0        0     6182 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/core/databases.py
--rw-r--r--   0        0        0     6204 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/core/invites.py
--rw-r--r--   0        0        0     2554 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/core/users.py
--rw-r--r--   0        0        0     7419 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/core/workspaces.py
--rw-r--r--   0        0        0      769 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/workspace/__init__.py
--rw-r--r--   0        0        0    12315 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/workspace/branch.py
--rw-r--r--   0        0        0    11721 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/workspace/migrations.py
--rw-r--r--   0        0        0    12491 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/workspace/records.py
--rw-r--r--   0        0        0    30137 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/workspace/search_and_filter.py
--rw-r--r--   0        0        0    12792 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/workspace/table.py
--rw-r--r--   0        0        0     1867 1970-01-01 00:00:00.000000 xata-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-04 18:58:29.629796 xata-1.0.0a1/LICENSE
+-rw-r--r--   0        0        0     1156 2023-07-04 18:58:29.633796 xata-1.0.0a1/README.md
+-rw-r--r--   0        0        0      818 2023-07-04 18:58:29.657796 xata-1.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0      873 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/__init__.py
+-rw-r--r--   0        0        0      769 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/__init__.py
+-rw-r--r--   0        0        0     2681 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/authentication.py
+-rw-r--r--   0        0        0    12341 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/branch.py
+-rw-r--r--   0        0        0     7553 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/databases.py
+-rw-r--r--   0        0        0     8958 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/files.py
+-rw-r--r--   0        0        0     6083 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/invites.py
+-rw-r--r--   0        0        0    11676 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/migrations.py
+-rw-r--r--   0        0        0    12501 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/records.py
+-rw-r--r--   0        0        0    31539 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/search_and_filter.py
+-rw-r--r--   0        0        0    12238 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/table.py
+-rw-r--r--   0        0        0     2532 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/users.py
+-rw-r--r--   0        0        0     7314 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/workspaces.py
+-rw-r--r--   0        0        0     2294 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api_response.py
+-rw-r--r--   0        0        0    13623 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/client.py
+-rw-r--r--   0        0        0     1188 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/errors.py
+-rw-r--r--   0        0        0    15888 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/helpers.py
+-rw-r--r--   0        0        0     3076 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/namespace.py
+-rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 xata-1.0.0a1/PKG-INFO
```

### Comparing `xata-0.9.3/LICENSE` & `xata-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `xata-0.9.3/README.md` & `xata-1.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `xata-0.9.3/pyproject.toml` & `xata-1.0.0a1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xata"
-version = "0.9.3"
+version = "1.0.0a1"
 description = "Python client for Xata.io"
 authors = ["Xata <support@xata.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 documentation = "https://xata-py.readthedocs.io"
 
 [tool.poetry.dependencies]
@@ -24,11 +24,14 @@
 flake8-bugbear = "^22.10.27"
 flake8-annotations = "^2.9.1"
 pdoc3 = "^0.10.0"
 Faker = "^17.0.0"
 sphinx-rtd-theme = "^1.2.0"
 mako = "^1.2.4"
 pytz = "^2022.7.1"
+Pillow = "^9.5.0"
+python-magic = "^0.4.22"
+pep8-naming = "^0.13.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `xata-0.9.3/xata/__init__.py` & `xata-1.0.0a1/xata/api/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,11 +12,7 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
-
-from .client import XataClient
-
-__all__ = ("XataClient", "BulkProcessor", "to_rfc3339")
```

### Comparing `xata-0.9.3/xata/errors.py` & `xata-1.0.0a1/xata/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,49 +14,26 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 
 
-class UnauthorizedException(Exception):
+class UnauthorizedError(Exception):
     pass
 
 
-class RateLimitException(Exception):
+class RateLimitError(Exception):
     pass
 
 
-class RecordNotFoundException(Exception):
-    id: str
-
-    def __init__(self, id: str):
-        self.id = id
-
-    def __str__(self) -> str:
-        return f"Record with id {self.id} not found"
-
-
-class BadRequestException(Exception):
-    status_code: int
-    message: str
-
-    def __init__(self, status_code, message):
-        self.status_code = status_code
-        self.message = message
-        super().__init__(message)
-
-    def __str__(self) -> str:
-        return f"Bad request: {self.status_code} {self.message}"
-
-
-class ServerErrorException(Exception):
+class XataServerError(Exception):
     status_code: int
     message: str
 
-    def __init__(self, status_code, message):
+    def __init__(self, status_code, message="n/a"):
         self.status_code = status_code
         self.message = message
         super().__init__(message)
 
     def __str__(self) -> str:
         return f"Server error: {self.status_code} {self.message}"
```

### Comparing `xata-0.9.3/xata/helpers.py` & `xata-1.0.0a1/xata/helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,61 +20,65 @@
 import logging
 import time
 from datetime import datetime, timezone
 from threading import Lock, Thread
 
 from .client import XataClient
 
-DEFAULT_THREAD_POOL_SIZE = 4
-DEFAULT_BATCH_SIZE = 25
-DEFAULT_FLUSH_INTERVAL = 5
-DEFAULT_PROCESSING_TIMEOUT = 0.025
-DEFAULT_THROW_EXCEPTION = False
+BP_DEFAULT_THREAD_POOL_SIZE = 4
+BP_DEFAULT_BATCH_SIZE = 25
+BP_DEFAULT_FLUSH_INTERVAL = 5
+BP_DEFAULT_PROCESSING_TIMEOUT = 0.025
+BP_DEFAULT_THROW_EXCEPTION = False
+BP_VERSION = "0.2.1"
+TRX_MAX_OPERATIONS = 1000
+TRX_VERSION = "0.0.1"
 
 
 class BulkProcessor(object):
     """
-    !!! This helper is still work in progress !!!
-
     Additional abstraction for bulk requests that process'
     requests in parallel
-    :stability alpha
+    :stability beta
     """
 
     def __init__(
         self,
         client: XataClient,
-        thread_pool_size: int = DEFAULT_THREAD_POOL_SIZE,
-        batch_size: int = DEFAULT_BATCH_SIZE,
-        flush_interval: int = DEFAULT_FLUSH_INTERVAL,
-        processing_timeout: float = DEFAULT_PROCESSING_TIMEOUT,
-        throw_exception: bool = DEFAULT_THROW_EXCEPTION,
+        thread_pool_size: int = BP_DEFAULT_THREAD_POOL_SIZE,
+        batch_size: int = BP_DEFAULT_BATCH_SIZE,
+        flush_interval: int = BP_DEFAULT_FLUSH_INTERVAL,
+        processing_timeout: float = BP_DEFAULT_PROCESSING_TIMEOUT,
+        throw_exception: bool = BP_DEFAULT_THROW_EXCEPTION,
     ):
         """
         BulkProcessor: Abstraction for bulk ingestion of records.
 
         :stability beta
 
         :param client: XataClient
         :param thread_pool_size: int How many data queue workers should be deployed (default: 4)
         :param batch_size: int How many records per table should be pushed as batch (default: 25)
         :param flush_interval: int After how many seconds should the per table queue be flushed (default: 5 seconds)
         :processing_timeout: float Cooldown period between batches (default: 0.025 seconds)
         :throw_exception: bool Throw exception ingestion, could kill all workers (default: False)
+
+        :raises Exception if throw exception is enabled
         """
         if thread_pool_size < 1:
-            raise Exception("thread pool size must be greater than 0, default: %d" % DEFAULT_THREAD_POOL_SIZE)
+            raise Exception("thread pool size must be greater than 0, default: %d" % BP_DEFAULT_THREAD_POOL_SIZE)
         if processing_timeout < 0:
-            raise Exception("processing timeout can not be negative, default: %f" % DEFAULT_PROCESSING_TIMEOUT)
+            raise Exception("processing timeout can not be negative, default: %f" % BP_DEFAULT_PROCESSING_TIMEOUT)
         if flush_interval < 0:
-            raise Exception("flush interval can not be negative, default: %f" % DEFAULT_FLUSH_INTERVAL)
+            raise Exception("flush interval can not be negative, default: %f" % BP_DEFAULT_FLUSH_INTERVAL)
         if batch_size < 1:
-            raise Exception("batch size can not be less than one, default: %d" % DEFAULT_BATCH_SIZE)
+            raise Exception("batch size can not be less than one, default: %d" % BP_DEFAULT_BATCH_SIZE)
 
         self.client = client
+        self.client.set_header("x-xata-helper", f"bulkprocessor/{BP_VERSION}")
         self.processing_timeout = processing_timeout
         self.batch_size = batch_size
         self.flush_interval = flush_interval
         self.failed_batches_queue = []
         self.throw_exception = throw_exception
         self.stats = {"total": 0, "queue": 0, "failed_batches": 0, "tables": {}}
         self.logger = logging.getLogger(f"{__name__}.{self.__class__.__name__}")
@@ -88,28 +92,28 @@
             self.thread_workers.append(worker)
 
     def process(self, id: int):
         """
         Process the records
         """
         self.logger.debug(
-            "thread #%d: starting bulk processor [thread_pool_size=%d, batch_size=%d, flush_interval=%d, processing_timeout=%s"
+            "thread #%d: starting bulk processor [thread_pool=%d, batch=%d, flush=%d, processing_timeout=%s"
             % (
                 id,
                 len(self.thread_workers),
                 self.batch_size,
                 self.flush_interval,
                 self.processing_timeout,
             )
         )
         while True:
             batch = self.records.next_batch()
             if "table" in batch and len(batch["records"]) > 0:
                 try:
-                    r = self.client.records().bulkInsertTableRecords(batch["table"], {"records": batch["records"]})
+                    r = self.client.records().bulk_insert(batch["table"], {"records": batch["records"]})
                     if r.status_code != 200:
                         self.logger.error(
                             "thread #%d: unable to process batch for table '%s', with error: %d - %s"
                             % (id, batch["table"], r.status_code, r.json())
                         )
                         # Add to failed queue
                         self.failed_batches_queue.append(
@@ -286,7 +290,123 @@
     :link https://datatracker.ietf.org/doc/html/rfc3339
 
     :param dt: datetime instance to convert
     :param tz: timezone to convert in, default: UTC
     :return str
     """
     return dt.replace(tzinfo=tz).isoformat()
+
+
+class Transaction(object):
+    """
+    Additional abstraction for bulk requests that process'
+    requests in parallel
+    :stability beta
+    """
+
+    def __init__(
+        self,
+        client: XataClient,
+    ) -> None:
+        """
+        Transaction Helper
+        Wrapper to simplify running transactions
+
+        :stability beta
+
+        :param client: XataClient
+        """
+        self.client = client
+        self.client.set_header("x-xata-helper", f"transaction/{TRX_VERSION}")
+
+        self.has_run = False
+        self.operations = {"operations": []}
+
+    def _add_operation(self, operation: dict) -> None:
+        if len(self.operations["operations"]) >= TRX_MAX_OPERATIONS:
+            raise Exception(f"Maximum amount of {TRX_MAX_OPERATIONS} transaction operations exceeded.")
+        self.operations["operations"].append(operation)
+
+    def insert(self, table: str, record: dict, create_only: bool = False) -> None:
+        """
+        Inserts can be used to insert records across any number of tables in your database. As with the
+        insert endpoints, you can explicitly set an ID, or omit it and have Xata auto-generate one for you.
+        Either way, on a successful transaction, Xata will return the ID to you.
+
+        :param table: str
+        :param record: dict
+        :param create_only: bool By default, if a record exists with the same explicit ID, Xata will overwrite
+            the record. You can adjust this behavior by setting `create_only` to `true` for the operation.
+            Default: False
+
+        :raises Exception if limit of 1000 operations is exceeded
+        """
+        self._add_operation({"insert": {"table": table, "record": record, "createOnly": create_only}})
+
+    def update(self, table: str, record_id: str, fields: dict, upsert: bool = False) -> None:
+        """
+        Updates can be used to update records in any number of tables in your database. The update operation
+        requires an ID parameter explicitly defined. The operation will only replace the fields explicitly
+        specified in your operation. The update operation also supports the upsert flag. Off by default, but
+        if set to `true`, the update operation will insert the record if no record is found with the provided ID.
+
+        :param table: str
+        :param record_id: str
+        :param fields: dict
+        :param upsert: bool Default: False
+
+        :raises Exception if limit of 1000 operations is exceeded
+        """
+        self._add_operation({"update": {"table": table, "id": record_id, "fields": fields, "upsert": upsert}})
+
+    def delete(self, table: str, record_id: str, columns: list[str] = [], fail_if_missing: bool = False) -> None:
+        """
+        A delete is used to remove records. Delete can operate on records from the same transaction, and will
+        not cancel a transaction if no record is found.
+        https://xata.io/docs/api-reference/db/db_branch_name/transaction#execute-a-transaction-on-a-branch
+
+        :param table: str
+        :param record_id: str
+        :param columns: list of columns to retrieve
+        :param fail_if_missing: bool, Default: False
+
+        :raises Exception if limit of 1000 operations is exceeded
+        """
+        self._add_operation(
+            {"delete": {"table": table, "id": record_id, "columns": columns, "failIfMissing": fail_if_missing}}
+        )
+
+    def get(self, table: str, record_id: str, columns: list[str] = []) -> None:
+        """
+        A get is used to retrieve a record by id. A get operation can retrieve records created in the same transaction
+        but will not cancel a transaction if no record is found.
+
+        :param table: str
+        :param record_id: str
+        :param columns: list of columns to retrieve
+
+        :raises Exception if limit of 1000 operations is exceeded
+        """
+        self._add_operation({"get": {"table": table, "id": record_id, "columns": columns}})
+
+    def run(self) -> dict:
+        """
+        Commit the transactions. Flushes the operations queue
+
+        :return dict
+        """
+        r = self.client.records().transaction(self.operations)
+        result = {
+            "status_code": r.status_code,
+            "results": r["results"] if "results" in r else [],
+            "has_errors": True if "errors" in r else False,
+            "errors": r["errors"] if "errors" in r else [],
+        }
+        self.operations["operations"] = []  # free memory
+        return result
+
+    def size(self) -> int:
+        """
+        Get amount of operations in queue
+        :return int
+        """
+        return len(self.operations["operations"])
```

### Comparing `xata-0.9.3/xata/namespace.py` & `xata-1.0.0a1/xata/api_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,48 +13,68 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 
-from requests import Response, request
+import logging
+from typing import Union
 
-from .errors import RateLimitException
+from requests import Response
+from requests.exceptions import JSONDecodeError
 
 
-class Namespace:
-    """
-    Parent class for Namespaces
-    """
-
-    def __init__(self, client):
-        self.client = client
-
-    def get_scope(self) -> str:
-        return self.scope
-
-    def is_control_plane(self) -> bool:
-        return self.get_scope() == "core"
-
-    def get_base_url(self) -> str:
-        if self.is_control_plane():
-            return "https://" + self.client.get_config()["domain_core"]
-        # Base URL must be build on the fly as the region & workspace Id can change
-        cfg = self.client.get_config()
-        return "https://%s.%s.%s" % (cfg["workspaceId"], cfg["region"], cfg["domain_workspace"])
-
-    def request(self, http_method: str, url_path: str, headers: dict = {}, payload: dict = None) -> Response:
-        headers = {
-            **headers,
-            **self.client.get_headers(),
-        }  # TODO use "|" when client py min version >= 3.9
-        url = "%s/%s" % (self.get_base_url(), url_path.lstrip("/"))
-        if payload is None:
-            resp = request(http_method, url, headers=headers)
-        else:
-            resp = request(http_method, url, headers=headers, json=payload)
-
-        if resp.status_code == 429:
-            raise RateLimitException(f"Rate limited: {resp.json()}")
-
-        return resp
+class ApiResponse(dict):
+    def __init__(self, response: Response):
+        self.response = response
+        self.logger = logging.getLogger(self.__class__.__name__)
+
+        # Don't serialize an empty response
+        try:
+            self.update(self.response.json())
+        except JSONDecodeError:
+            pass
+
+        # log server message
+        if "x-xata-message" in self.headers:
+            self.logger.warn(self.headers["x-xata-message"])
+
+    def server_message(self) -> Union[str, None]:
+        """
+        Get the server message from the response
+        :return str | None
+        """
+        if "x-xata-message" in self.headers:
+            return self.headers["x-xata-message"]
+        return None
+
+    def is_success(self) -> bool:
+        """
+        Was the request successful?
+        :return bool
+        """
+        return 200 <= self.status_code < 300
+
+    @property
+    def status_code(self) -> int:
+        """
+        Get the status code of the response
+        :return int
+        """
+        return self.response.status_code
+
+    @property
+    def headers(self) -> dict:
+        """
+        Get the response headers
+        :return dict
+        """
+        return self.response.headers
+
+    @property
+    def content(self) -> bytes:
+        """
+        For files support, to get the file content
+        :return bytes
+        """
+        return self.response.content
```

### Comparing `xata-0.9.3/xata/namespaces/__init__.py` & `xata-1.0.0a1/xata/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,7 +12,11 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
+
+from .client import XataClient
+
+__all__ = ("XataClient", "BulkProcessor", "to_rfc3339", "Transaction")
```

### Comparing `xata-0.9.3/xata/namespaces/core/authentication.py` & `xata-1.0.0a1/xata/api/authentication.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,46 +19,42 @@
 
 # ------------------------------------------------------- #
 # Authentication
 # Authentication and API Key management.
 # Specification: core:v1.0
 # ------------------------------------------------------- #
 
-from requests import Response
-
+from xata.api_response import ApiResponse
 from xata.namespace import Namespace
 
 
 class Authentication(Namespace):
 
     scope = "core"
 
-    def getUserAPIKeys(
-        self,
-    ) -> Response:
+    def get_user_api_keys(self) -> ApiResponse:
         """
         Retrieve a list of existing user API keys
 
         Path: /user/keys
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
-
         :return Response
         """
         url_path = "/user/keys"
         return self.request("GET", url_path)
 
-    def createUserAPIKey(self, key_name: str) -> Response:
+    def create_user_api_keys(self, key_name: str) -> ApiResponse:
         """
         Create and return new API key
 
         Path: /user/keys/{key_name}
         Method: POST
         Response status codes:
         - 201: OK
@@ -71,15 +67,15 @@
         :param key_name: str API Key name
 
         :return Response
         """
         url_path = f"/user/keys/{key_name}"
         return self.request("POST", url_path)
 
-    def deleteUserAPIKey(self, key_name: str) -> Response:
+    def delete_user_api_keys(self, key_name: str) -> ApiResponse:
         """
         Delete an existing API key
 
         Path: /user/keys/{key_name}
         Method: DELETE
         Response status codes:
         - 204: No Content
```

### Comparing `xata-0.9.3/xata/namespaces/core/databases.py` & `xata-1.0.0a1/xata/api/databases.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,24 +19,23 @@
 
 # ------------------------------------------------------- #
 # Databases
 # Workspace databases management.
 # Specification: core:v1.0
 # ------------------------------------------------------- #
 
-from requests import Response
-
+from xata.api_response import ApiResponse
 from xata.namespace import Namespace
 
 
 class Databases(Namespace):
 
     scope = "core"
 
-    def getDatabaseList(self, workspace_id: str = None) -> Response:
+    def list(self, workspace_id: str = None) -> ApiResponse:
         """
         List all databases available in your Workspace.
 
         Path: /workspaces/{workspace_id}/dbs
         Method: GET
         Response status codes:
         - 200: OK
@@ -46,19 +45,19 @@
         Response: application/json
 
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
         :return Response
         """
         if workspace_id is None:
-            workspace_id = self.client.get_config()["workspaceId"]
+            workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/dbs"
         return self.request("GET", url_path)
 
-    def getDatabaseMetadata(self, db_name: str, workspace_id: str = None) -> Response:
+    def get_metadata(self, db_name: str, workspace_id: str = None) -> ApiResponse:
         """
         Retrieve metadata of the given database
 
         Path: /workspaces/{workspace_id}/dbs/{db_name}
         Method: GET
         Response status codes:
         - 200: OK
@@ -70,19 +69,21 @@
 
         :param db_name: str The Database Name
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
         :return Response
         """
         if workspace_id is None:
-            workspace_id = self.client.get_config()["workspaceId"]
+            workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/dbs/{db_name}"
         return self.request("GET", url_path)
 
-    def createDatabase(self, db_name: str, payload: dict, workspace_id: str = None) -> Response:
+    def create(
+        self, db_name: str, workspace_id: str = None, region: str = None, branch_name: str = None
+    ) -> ApiResponse:
         """
         Create Database with identifier name
 
         Path: /workspaces/{workspace_id}/dbs/{db_name}
         Method: PUT
         Response status codes:
         - 201: Created
@@ -90,26 +91,31 @@
         - 401: Authentication Error
         - 422: Example response
         - 423: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
         :param db_name: str The Database Name
-        :param payload: dict content
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
+        :param region: str = None Which region to deploy. Default: region defined in the client, if not specified: us-east-1
+        :param branch_name: str = None Which branch to create. Default: branch name used from the client, if not speicifed: main
 
         :return Response
         """
         if workspace_id is None:
-            workspace_id = self.client.get_config()["workspaceId"]
+            workspace_id = self.client.get_workspace_id()
+        payload = {
+            "region": region if region else self.client.get_region(),
+            "branchName": branch_name if branch_name else self.client.get_branch_name(),
+        }
         url_path = f"/workspaces/{workspace_id}/dbs/{db_name}"
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
-    def deleteDatabase(self, db_name: str, workspace_id: str = None) -> Response:
+    def delete(self, db_name: str, workspace_id: str = None) -> ApiResponse:
         """
         Delete a database and all of its branches and tables permanently.
 
         Path: /workspaces/{workspace_id}/dbs/{db_name}
         Method: DELETE
         Response status codes:
         - 200: OK
@@ -121,19 +127,19 @@
 
         :param db_name: str The Database Name
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
         :return Response
         """
         if workspace_id is None:
-            workspace_id = self.client.get_config()["workspaceId"]
+            workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/dbs/{db_name}"
         return self.request("DELETE", url_path)
 
-    def updateDatabaseMetadata(self, db_name: str, payload: dict, workspace_id: str = None) -> Response:
+    def update_metadata(self, db_name: str, payload: dict, workspace_id: str = None) -> ApiResponse:
         """
         Update the color of the selected database
 
         Path: /workspaces/{workspace_id}/dbs/{db_name}
         Method: PATCH
         Response status codes:
         - 200: OK
@@ -146,20 +152,47 @@
         :param db_name: str The Database Name
         :param payload: dict content
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
         :return Response
         """
         if workspace_id is None:
-            workspace_id = self.client.get_config()["workspaceId"]
+            workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/dbs/{db_name}"
         headers = {"content-type": "application/json"}
         return self.request("PATCH", url_path, headers, payload)
 
-    def listRegions(self, workspace_id: str = None) -> Response:
+    def rename(self, db_name: str, payload: dict, workspace_id: str = None) -> ApiResponse:
+        """
+        Change the name of an existing database
+
+        Path: /workspaces/{workspace_id}/dbs/{db_name}/rename
+        Method: POST
+        Response status codes:
+        - 200: OK
+        - 400: Bad Request
+        - 401: Authentication Error
+        - 422: Example response
+        - 423: Example response
+        - 5XX: Unexpected Error
+        Response: application/json
+
+        :param db_name: str The Database Name
+        :param payload: dict content
+        :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
+
+        :return Response
+        """
+        if workspace_id is None:
+            workspace_id = self.client.get_workspace_id()
+        url_path = f"/workspaces/{workspace_id}/dbs/{db_name}/rename"
+        headers = {"content-type": "application/json"}
+        return self.request("POST", url_path, headers, payload)
+
+    def get_regions(self, workspace_id: str = None) -> ApiResponse:
         """
         List regions available to create a database on
 
         Path: /workspaces/{workspace_id}/regions
         Method: GET
         Response status codes:
         - 200: OK
@@ -169,10 +202,10 @@
         Response: application/json
 
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
         :return Response
         """
         if workspace_id is None:
-            workspace_id = self.client.get_config()["workspaceId"]
+            workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/regions"
         return self.request("GET", url_path)
```

### Comparing `xata-0.9.3/xata/namespaces/core/invites.py` & `xata-1.0.0a1/xata/api/invites.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,24 +19,23 @@
 
 # ------------------------------------------------------- #
 # Invites
 # Manage user invites.
 # Specification: core:v1.0
 # ------------------------------------------------------- #
 
-from requests import Response
-
+from xata.api_response import ApiResponse
 from xata.namespace import Namespace
 
 
 class Invites(Namespace):
 
     scope = "core"
 
-    def inviteWorkspaceMember(self, payload: dict, workspace_id: str = None) -> Response:
+    def new(self, payload: dict, workspace_id: str = None) -> ApiResponse:
         """
         Invite some user to join the workspace with the given role
 
         Path: /workspaces/{workspace_id}/invites
         Method: POST
         Response status codes:
         - 201: Created
@@ -50,20 +49,20 @@
 
         :param payload: dict content
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
         :return Response
         """
         if workspace_id is None:
-            workspace_id = self.client.get_config()["workspaceId"]
+            workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/invites"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def cancelWorkspaceMemberInvite(self, invite_id: str, workspace_id: str = None) -> Response:
+    def cancel(self, invite_id: str, workspace_id: str = None) -> ApiResponse:
         """
         This operation provides a way to cancel invites by deleting them.  Already accepted
         invites cannot be deleted.
 
         Path: /workspaces/{workspace_id}/invites/{invite_id}
         Method: DELETE
         Response status codes:
@@ -76,19 +75,19 @@
 
         :param invite_id: str Invite identifier
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
         :return Response
         """
         if workspace_id is None:
-            workspace_id = self.client.get_config()["workspaceId"]
+            workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/invites/{invite_id}"
         return self.request("DELETE", url_path)
 
-    def updateWorkspaceMemberInvite(self, invite_id: str, payload: dict, workspace_id: str = None) -> Response:
+    def update(self, invite_id: str, payload: dict, workspace_id: str = None) -> ApiResponse:
         """
         This operation provides a way to update an existing invite.  Updates are performed in-
         place; they do not change the invite link, the expiry time, nor do they re-notify the
         recipient of the invite.
 
         Path: /workspaces/{workspace_id}/invites/{invite_id}
         Method: PATCH
@@ -105,20 +104,20 @@
         :param invite_id: str Invite identifier
         :param payload: dict content
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
         :return Response
         """
         if workspace_id is None:
-            workspace_id = self.client.get_config()["workspaceId"]
+            workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/invites/{invite_id}"
         headers = {"content-type": "application/json"}
         return self.request("PATCH", url_path, headers, payload)
 
-    def acceptWorkspaceMemberInvite(self, invite_key: str, workspace_id: str = None) -> Response:
+    def accept(self, invite_key: str, workspace_id: str = None) -> ApiResponse:
         """
         Accept the invitation to join a workspace.  If the operation succeeds the user will be a
         member of the workspace
 
         Path: /workspaces/{workspace_id}/invites/{invite_key}/accept
         Method: POST
         Response status codes:
@@ -131,19 +130,19 @@
 
         :param invite_key: str Invite Key (secret) for the invited user
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
         :return Response
         """
         if workspace_id is None:
-            workspace_id = self.client.get_config()["workspaceId"]
+            workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/invites/{invite_key}/accept"
         return self.request("POST", url_path)
 
-    def resendWorkspaceMemberInvite(self, invite_id: str, workspace_id: str = None) -> Response:
+    def resend(self, invite_id: str, workspace_id: str = None) -> ApiResponse:
         """
         This operation provides a way to resend an Invite notification.  Invite notifications can
         only be sent for Invites not yet accepted.
 
         Path: /workspaces/{workspace_id}/invites/{invite_id}/resend
         Method: POST
         Response status codes:
@@ -156,10 +155,10 @@
 
         :param invite_id: str Invite identifier
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
         :return Response
         """
         if workspace_id is None:
-            workspace_id = self.client.get_config()["workspaceId"]
+            workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/invites/{invite_id}/resend"
         return self.request("POST", url_path)
```

### Comparing `xata-0.9.3/xata/namespaces/core/users.py` & `xata-1.0.0a1/xata/api/users.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,26 +19,23 @@
 
 # ------------------------------------------------------- #
 # Users
 # Users management
 # Specification: core:v1.0
 # ------------------------------------------------------- #
 
-from requests import Response
-
+from xata.api_response import ApiResponse
 from xata.namespace import Namespace
 
 
 class Users(Namespace):
 
     scope = "core"
 
-    def getUser(
-        self,
-    ) -> Response:
+    def get(self) -> ApiResponse:
         """
         Return details of the user making the request
 
         Path: /user
         Method: GET
         Response status codes:
         - 200: OK
@@ -50,15 +47,15 @@
 
 
         :return Response
         """
         url_path = "/user"
         return self.request("GET", url_path)
 
-    def updateUser(self, payload: dict) -> Response:
+    def update(self, payload: dict) -> ApiResponse:
         """
         Update user info
 
         Path: /user
         Method: PUT
         Response status codes:
         - 200: OK
@@ -72,17 +69,15 @@
 
         :return Response
         """
         url_path = "/user"
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
-    def deleteUser(
-        self,
-    ) -> Response:
+    def delete(self) -> ApiResponse:
         """
         Delete the user making the request
 
         Path: /user
         Method: DELETE
         Response status codes:
         - 204: No Content
```

### Comparing `xata-0.9.3/xata/namespaces/core/workspaces.py` & `xata-1.0.0a1/xata/api/workspaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,26 +19,23 @@
 
 # ------------------------------------------------------- #
 # Workspaces
 # Workspaces management
 # Specification: core:v1.0
 # ------------------------------------------------------- #
 
-from requests import Response
-
+from xata.api_response import ApiResponse
 from xata.namespace import Namespace
 
 
 class Workspaces(Namespace):
 
     scope = "core"
 
-    def getWorkspacesList(
-        self,
-    ) -> Response:
+    def get_workspaces(self) -> ApiResponse:
         """
         Retrieve the list of workspaces the user belongs to
 
         Path: /workspaces
         Method: GET
         Response status codes:
         - 200: OK
@@ -50,15 +47,15 @@
 
 
         :return Response
         """
         url_path = "/workspaces"
         return self.request("GET", url_path)
 
-    def createWorkspace(self, payload: dict) -> Response:
+    def create(self, payload: dict) -> ApiResponse:
         """
         Creates a new workspace with the user requesting it as its single owner.
 
         Path: /workspaces
         Method: POST
         Response status codes:
         - 201: Created
@@ -72,15 +69,15 @@
 
         :return Response
         """
         url_path = "/workspaces"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def getWorkspace(self, workspace_id: str = None) -> Response:
+    def get(self, workspace_id: str = None) -> ApiResponse:
         """
         Retrieve workspace info from a workspace ID
 
         Path: /workspaces/{workspace_id}
         Method: GET
         Response status codes:
         - 200: OK
@@ -92,19 +89,19 @@
         Response: application/json
 
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
         :return Response
         """
         if workspace_id is None:
-            workspace_id = self.client.get_config()["workspaceId"]
+            workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}"
         return self.request("GET", url_path)
 
-    def updateWorkspace(self, payload: dict, workspace_id: str = None) -> Response:
+    def update(self, payload: dict, workspace_id: str = None) -> ApiResponse:
         """
         Update workspace info
 
         Path: /workspaces/{workspace_id}
         Method: PUT
         Response status codes:
         - 200: OK
@@ -117,20 +114,20 @@
 
         :param payload: dict content
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
         :return Response
         """
         if workspace_id is None:
-            workspace_id = self.client.get_config()["workspaceId"]
+            workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}"
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
-    def deleteWorkspace(self, workspace_id: str = None) -> Response:
+    def delete(self, workspace_id: str = None) -> ApiResponse:
         """
         Delete the workspace with the provided ID
 
         Path: /workspaces/{workspace_id}
         Method: DELETE
         Response status codes:
         - 204: No Content
@@ -141,19 +138,19 @@
         - 5XX: Unexpected Error
 
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
         :return Response
         """
         if workspace_id is None:
-            workspace_id = self.client.get_config()["workspaceId"]
+            workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}"
         return self.request("DELETE", url_path)
 
-    def getWorkspaceMembersList(self, workspace_id: str = None) -> Response:
+    def get_members(self, workspace_id: str = None) -> ApiResponse:
         """
         Retrieve the list of members of the given workspace
 
         Path: /workspaces/{workspace_id}/members
         Method: GET
         Response status codes:
         - 200: OK
@@ -165,19 +162,19 @@
         Response: application/json
 
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
         :return Response
         """
         if workspace_id is None:
-            workspace_id = self.client.get_config()["workspaceId"]
+            workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/members"
         return self.request("GET", url_path)
 
-    def updateWorkspaceMemberRole(self, user_id: str, payload: dict, workspace_id: str = None) -> Response:
+    def update_member(self, user_id: str, payload: dict, workspace_id: str = None) -> ApiResponse:
         """
         Update a workspace member role.  Workspaces must always have at least one owner, so this
         operation will fail if trying to remove owner role from the last owner in the workspace.
 
         Path: /workspaces/{workspace_id}/members/{user_id}
         Method: PUT
         Response status codes:
@@ -191,20 +188,20 @@
         :param user_id: str UserID
         :param payload: dict content
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
         :return Response
         """
         if workspace_id is None:
-            workspace_id = self.client.get_config()["workspaceId"]
+            workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/members/{user_id}"
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
-    def removeWorkspaceMember(self, user_id: str, workspace_id: str = None) -> Response:
+    def remove_member(self, user_id: str, workspace_id: str = None) -> ApiResponse:
         """
         Remove the member from the workspace
 
         Path: /workspaces/{workspace_id}/members/{user_id}
         Method: DELETE
         Response status codes:
         - 204: No Content
@@ -216,10 +213,10 @@
 
         :param user_id: str UserID
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
         :return Response
         """
         if workspace_id is None:
-            workspace_id = self.client.get_config()["workspaceId"]
+            workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/members/{user_id}"
         return self.request("DELETE", url_path)
```

### Comparing `xata-0.9.3/xata/namespaces/workspace/branch.py` & `xata-1.0.0a1/xata/api/branch.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,24 +19,23 @@
 
 # ------------------------------------------------------- #
 # Branch
 # Branch management.
 # Specification: workspace:v1.0
 # ------------------------------------------------------- #
 
-from requests import Response
-
+from xata.api_response import ApiResponse
 from xata.namespace import Namespace
 
 
 class Branch(Namespace):
 
     scope = "workspace"
 
-    def getBranchList(self, db_name: str) -> Response:
+    def get_branches(self, db_name: str) -> ApiResponse:
         """
         List all available Branches
 
         Path: /dbs/{db_name}
         Method: GET
         Response status codes:
         - 200: OK
@@ -49,15 +48,15 @@
         :param db_name: str The Database Name
 
         :return Response
         """
         url_path = f"/dbs/{db_name}"
         return self.request("GET", url_path)
 
-    def getBranchDetails(self, db_name: str = None, branch_name: str = None) -> Response:
+    def get_details(self, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Get branch schema and metadata
 
         Path: /db/{db_branch_name}
         Method: GET
         Response status codes:
         - 200: OK
@@ -72,15 +71,15 @@
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}"
         return self.request("GET", url_path)
 
-    def createBranch(self, payload: dict, db_name: str = None, branch_name: str = None, _from: str = None) -> Response:
+    def create(self, payload: dict, db_name: str = None, branch_name: str = None, _from: str = None) -> ApiResponse:
         """
         Create Database branch
 
         Path: /db/{db_branch_name}
         Method: PUT
         Response status codes:
         - 201: Created
@@ -101,15 +100,15 @@
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}"
         if _from is not None:
             url_path += "?from={_from}"
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
-    def deleteBranch(self, db_name: str = None, branch_name: str = None) -> Response:
+    def delete(self, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Delete the branch in the database and all its resources
 
         Path: /db/{db_branch_name}
         Method: DELETE
         Response status codes:
         - 200: OK
@@ -125,15 +124,15 @@
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}"
         return self.request("DELETE", url_path)
 
-    def getBranchMetadata(self, db_name: str = None, branch_name: str = None) -> Response:
+    def get_metadata(self, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Get Branch Metadata
 
         Path: /db/{db_branch_name}/metadata
         Method: GET
         Response status codes:
         - 200: OK
@@ -148,15 +147,15 @@
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/metadata"
         return self.request("GET", url_path)
 
-    def updateBranchMetadata(self, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def update_metadata(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Update the branch metadata
 
         Path: /db/{db_branch_name}/metadata
         Method: PUT
         Response status codes:
         - 204: No Content
@@ -172,15 +171,15 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/metadata"
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
-    def getBranchStats(self, db_name: str = None, branch_name: str = None) -> Response:
+    def get_stats(self, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Get branch usage metrics.
 
         Path: /db/{db_branch_name}/stats
         Method: GET
         Response status codes:
         - 200: OK
@@ -195,15 +194,15 @@
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/stats"
         return self.request("GET", url_path)
 
-    def getGitBranchesMapping(self, db_name: str) -> Response:
+    def get_git_branches_mapping(self, db_name: str) -> ApiResponse:
         """
         Lists all the git branches in the mapping, and their associated Xata branches.  Example
         response:  ```json {   "mappings": [       {         "gitBranch": "main",
         "xataBranch": "main"       },       {         "gitBranch": "gitBranch1",
         "xataBranch": "xataBranch1"       }       {         "gitBranch": "xataBranch2",
         "xataBranch": "xataBranch2"       }   ] } ```
 
@@ -219,15 +218,15 @@
         :param db_name: str The Database Name
 
         :return Response
         """
         url_path = f"/dbs/{db_name}/gitBranches"
         return self.request("GET", url_path)
 
-    def addGitBranchesEntry(self, db_name: str, payload: dict) -> Response:
+    def add_git_branches_entry(self, db_name: str, payload: dict) -> ApiResponse:
         """
         Adds an entry to the mapping of git branches to Xata branches.  The git branch and the
         Xata branch must be present in the body of the request.  If the Xata branch doesn't exist,
         a 400 error is returned.  If the git branch is already present in the mapping, the old
         entry is overwritten, and a warning message is included in the response.  If the git
         branch is added and didn't exist before, the response code is 204. If the git branch
         existed and it was overwritten, the response code is 201.  Example request:  ```json //
@@ -249,15 +248,15 @@
 
         :return Response
         """
         url_path = f"/dbs/{db_name}/gitBranches"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def removeGitBranchesEntry(self, db_name: str, gitBranch: str) -> Response:
+    def remove_git_branches_entry(self, db_name: str, git_branch: str) -> ApiResponse:
         """
         Removes an entry from the mapping of git branches to Xata branches.  The name of the git
         branch must be passed as a query parameter.  If the git branch is not found, the endpoint
         returns a 404 status code.  Example request:  ```json // DELETE https://tutorial-
         ng7s8c.xata.sh/dbs/demo/gitBranches?gitBranch=fix%2Fbug123 ```
 
         Path: /dbs/{db_name}/gitBranches
@@ -266,24 +265,24 @@
         - 204: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: The git branch was not found in the mapping
         - 5XX: Unexpected Error
 
         :param db_name: str The Database Name
-        :param gitBranch: str The Git Branch to remove from the mapping
+        :param git_branch: str The Git Branch to remove from the mapping
 
         :return Response
         """
         url_path = f"/dbs/{db_name}/gitBranches"
-        if gitBranch is not None:
-            url_path += "?gitBranch={gitBranch}"
+        if git_branch is not None:
+            url_path += "?gitBranch={git_branch}"
         return self.request("DELETE", url_path)
 
-    def resolveBranch(self, db_name: str, gitBranch: str = None, fallbackBranch: str = None) -> Response:
+    def resolve(self, db_name: str, git_branch: str = None, fallback_branch: str = None) -> ApiResponse:
         """
         In order to resolve the database branch, the following algorithm is used: * if the
         `gitBranch` was provided and is found in the [git branches mapping](/api-
         reference/dbs/db_name/gitBranches), the associated Xata branch is returned * else, if a
         Xata branch with the exact same name as `gitBranch` exists, return it * else, if
         `fallbackBranch` is provided and a branch with that name exists, return it * else, return
         the default branch of the DB (`main` or the first branch)  Example call:  ```json // GET
@@ -298,21 +297,21 @@
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 5XX: Unexpected Error
         Response: application/json
 
         :param db_name: str The Database Name
-        :param gitBranch: str = None The Git Branch
-        :param fallbackBranch: str = None Default branch to fallback to
+        :param git_branch: str = None The Git Branch
+        :param fallback_branch: str = None Default branch to fallback to
 
         :return Response
         """
         url_path = f"/dbs/{db_name}/resolveBranch"
         query_params = []
-        if gitBranch is not None:
-            query_params.append(f"gitBranch={gitBranch}")
-        if fallbackBranch is not None:
-            query_params.append(f"fallbackBranch={fallbackBranch}")
+        if git_branch is not None:
+            query_params.append(f"gitBranch={git_branch}")
+        if fallback_branch is not None:
+            query_params.append(f"fallbackBranch={fallback_branch}")
         if query_params:
             url_path += "?" + "&".join(query_params)
         return self.request("GET", url_path)
```

### Comparing `xata-0.9.3/xata/namespaces/workspace/migrations.py` & `xata-1.0.0a1/xata/api/migrations.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,24 +19,23 @@
 
 # ------------------------------------------------------- #
 # Migrations
 # Branch schema migrations and history.
 # Specification: workspace:v1.0
 # ------------------------------------------------------- #
 
-from requests import Response
-
+from xata.api_response import ApiResponse
 from xata.namespace import Namespace
 
 
 class Migrations(Namespace):
 
     scope = "workspace"
 
-    def getBranchMigrationHistory(self, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def get_history(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Get branch migration history [deprecated]
 
         Path: /db/{db_branch_name}/migrations
         Method: GET
         Response status codes:
         - 200: OK
@@ -53,15 +52,15 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/migrations"
         headers = {"content-type": "application/json"}
         return self.request("GET", url_path, headers, payload)
 
-    def getBranchMigrationPlan(self, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def get_plan(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Compute a migration plan from a target schema the branch should be migrated too.
 
         Path: /db/{db_branch_name}/migrations/plan
         Method: POST
         Response status codes:
         - 200: Example response
@@ -77,15 +76,15 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/migrations/plan"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def executeBranchMigrationPlan(self, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def execute_plan(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Apply a migration plan to the branch
 
         Path: /db/{db_branch_name}/migrations/execute
         Method: POST
         Response status codes:
         - 200: Schema migration response with ID and migration status.
@@ -101,15 +100,15 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/migrations/execute"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def getBranchSchemaHistory(self, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def get_schema_history(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Query schema history.
 
         Path: /db/{db_branch_name}/schema/history
         Method: POST
         Response status codes:
         - 200: OK
@@ -126,15 +125,17 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/schema/history"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def compareBranchWithUserSchema(self, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def compare_branch_with_user_schema(
+        self, payload: dict, db_name: str = None, branch_name: str = None
+    ) -> ApiResponse:
         """
         Compare branch with user schema.
 
         Path: /db/{db_branch_name}/schema/compare
         Method: POST
         Response status codes:
         - 200: Schema comparison response.
@@ -150,15 +151,15 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/schema/compare"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def compareBranchSchemas(self, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def compare_schemas(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Compare branch schemas.
 
         Path: /db/{db_branch_name}/schema/compare/{branch_name}
         Method: POST
         Response status codes:
         - 200: Schema comparison response.
@@ -174,15 +175,15 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/schema/compare/{branch_name}"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def updateBranchSchema(self, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def upadte_schema(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Update Branch schema
 
         Path: /db/{db_branch_name}/schema/update
         Method: POST
         Response status codes:
         - 200: Schema migration response with ID and migration status.
@@ -198,15 +199,15 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/schema/update"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def previewBranchSchemaEdit(self, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def preview(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Preview branch schema edits.
 
         Path: /db/{db_branch_name}/schema/preview
         Method: POST
         Response status codes:
         - 200: OK
@@ -223,15 +224,15 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/schema/preview"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def applyBranchSchemaEdit(self, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def apply(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Apply edit script.
 
         Path: /db/{db_branch_name}/schema/apply
         Method: POST
         Response status codes:
         - 200: Schema migration response with ID and migration status.
@@ -247,15 +248,15 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/schema/apply"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def pushBranchMigrations(self, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def push(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         The `schema/push` API accepts a list of migrations to be applied to the current branch.  A
         list of applicable migrations can be fetched using the `schema/history` API from another
         branch or database.  The most recent migration must be part of the list or referenced (via
         `parentID`) by the first migration in the list of migrations to be pushed.  Each migration
         in the list has an `id`, `parentID`, and `checksum`. The checksum for migrations are
         generated and verified by xata.  The operation fails if any migration in the list has an
```

### Comparing `xata-0.9.3/xata/namespaces/workspace/records.py` & `xata-1.0.0a1/xata/api/records.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,24 +19,23 @@
 
 # ------------------------------------------------------- #
 # Records
 # Record access API.
 # Specification: workspace:v1.0
 # ------------------------------------------------------- #
 
-from requests import Response
-
+from xata.api_response import ApiResponse
 from xata.namespace import Namespace
 
 
 class Records(Namespace):
 
     scope = "workspace"
 
-    def branchTransaction(self, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def transaction(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Execute a transaction on a branch
 
         Path: /db/{db_branch_name}/transaction
         Method: POST
         Response status codes:
         - 200: Returns the results of a successful transaction.
@@ -53,24 +52,24 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/transaction"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def insertRecord(
+    def insert(
         self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None, columns: list = None
-    ) -> Response:
+    ) -> ApiResponse:
         """
         Insert a new Record into the Table
 
         Path: /db/{db_branch_name}/tables/{table_name}/data
         Method: POST
         Response status codes:
-        - 201: Record ID and version
+        - 201: Record ID and metadata
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
 
         :param table_name: str The Table name
         :param payload: dict content
@@ -83,17 +82,17 @@
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/data"
         if columns is not None:
             url_path += "?columns=%s" % ",".join(columns)
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def getRecord(
+    def get(
         self, table_name: str, record_id: str, db_name: str = None, branch_name: str = None, columns: list = None
-    ) -> Response:
+    ) -> ApiResponse:
         """
         Retrieve record by ID
 
         Path: /db/{db_branch_name}/tables/{table_name}/data/{record_id}
         Method: GET
         Response status codes:
         - 200: Table Record Reponse
@@ -112,115 +111,115 @@
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/data/{record_id}"
         if columns is not None:
             url_path += "?columns=%s" % ",".join(columns)
         return self.request("GET", url_path)
 
-    def insertRecordWithID(
+    def insert_with_id(
         self,
         table_name: str,
         record_id: str,
         payload: dict,
         db_name: str = None,
         branch_name: str = None,
         columns: list = None,
-        createOnly: bool = None,
-        ifVersion: int = None,
-    ) -> Response:
+        create_only: bool = None,
+        if_version: int = None,
+    ) -> ApiResponse:
         """
         By default, IDs are auto-generated when data is insterted into Xata.  Sending a request to
         this endpoint allows us to insert a record with a pre-existing ID, bypassing the default
         automatic ID generation.
 
         Path: /db/{db_branch_name}/tables/{table_name}/data/{record_id}
         Method: PUT
         Response status codes:
-        - 200: Record ID and version
-        - 201: Record ID and version
+        - 200: Record ID and metadata
+        - 201: Record ID and metadata
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 422: Example response
         - 5XX: Unexpected Error
 
         :param table_name: str The Table name
         :param record_id: str The Record name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
         :param columns: list = None Column filters
-        :param createOnly: bool = None
-        :param ifVersion: int = None
+        :param create_only: bool = None
+        :param if_version: int = None
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/data/{record_id}"
         query_params = []
         if columns is not None:
             query_params.append("columns=%s" % ",".join(columns))
-        if createOnly is not None:
-            query_params.append(f"createOnly={createOnly}")
-        if ifVersion is not None:
-            query_params.append(f"ifVersion={ifVersion}")
+        if create_only is not None:
+            query_params.append(f"createOnly={create_only}")
+        if if_version is not None:
+            query_params.append(f"ifVersion={if_version}")
         if query_params:
             url_path += "?" + "&".join(query_params)
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
-    def upsertRecordWithID(
+    def upsert_with_id(
         self,
         table_name: str,
         record_id: str,
         payload: dict,
         db_name: str = None,
         branch_name: str = None,
         columns: list = None,
-        ifVersion: int = None,
-    ) -> Response:
+        if_version: int = None,
+    ) -> ApiResponse:
         """
         Upsert record with ID
 
         Path: /db/{db_branch_name}/tables/{table_name}/data/{record_id}
         Method: POST
         Response status codes:
-        - 200: Record ID and version
-        - 201: Record ID and version
+        - 200: Record ID and metadata
+        - 201: Record ID and metadata
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 422: Example response
         - 5XX: Unexpected Error
 
         :param table_name: str The Table name
         :param record_id: str The Record name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
         :param columns: list = None Column filters
-        :param ifVersion: int = None
+        :param if_version: int = None
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/data/{record_id}"
         query_params = []
         if columns is not None:
             query_params.append("columns=%s" % ",".join(columns))
-        if ifVersion is not None:
-            query_params.append(f"ifVersion={ifVersion}")
+        if if_version is not None:
+            query_params.append(f"ifVersion={if_version}")
         if query_params:
             url_path += "?" + "&".join(query_params)
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def deleteRecord(
+    def delete(
         self, table_name: str, record_id: str, db_name: str = None, branch_name: str = None, columns: list = None
-    ) -> Response:
+    ) -> ApiResponse:
         """
         Delete record from table
 
         Path: /db/{db_branch_name}/tables/{table_name}/data/{record_id}
         Method: DELETE
         Response status codes:
         - 200: Table Record Reponse
@@ -240,62 +239,62 @@
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/data/{record_id}"
         if columns is not None:
             url_path += "?columns=%s" % ",".join(columns)
         return self.request("DELETE", url_path)
 
-    def updateRecordWithID(
+    def update_with_id(
         self,
         table_name: str,
         record_id: str,
         payload: dict,
         db_name: str = None,
         branch_name: str = None,
         columns: list = None,
-        ifVersion: int = None,
-    ) -> Response:
+        if_version: int = None,
+    ) -> ApiResponse:
         """
         Update record with ID
 
         Path: /db/{db_branch_name}/tables/{table_name}/data/{record_id}
         Method: PATCH
         Response status codes:
-        - 200: Record ID and version
+        - 200: Record ID and metadata
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 422: Example response
         - 5XX: Unexpected Error
 
         :param table_name: str The Table name
         :param record_id: str The Record name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
         :param columns: list = None Column filters
-        :param ifVersion: int = None
+        :param if_version: int = None
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/data/{record_id}"
         query_params = []
         if columns is not None:
             query_params.append("columns=%s" % ",".join(columns))
-        if ifVersion is not None:
-            query_params.append(f"ifVersion={ifVersion}")
+        if if_version is not None:
+            query_params.append(f"ifVersion={if_version}")
         if query_params:
             url_path += "?" + "&".join(query_params)
         headers = {"content-type": "application/json"}
         return self.request("PATCH", url_path, headers, payload)
 
-    def bulkInsertTableRecords(
+    def bulk_insert(
         self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None, columns: list = None
-    ) -> Response:
+    ) -> ApiResponse:
         """
         Bulk insert records
 
         Path: /db/{db_branch_name}/tables/{table_name}/bulk
         Method: POST
         Response status codes:
         - 200: OK
```

### Comparing `xata-0.9.3/xata/namespaces/workspace/search_and_filter.py` & `xata-1.0.0a1/xata/api/search_and_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,29 +14,28 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 
 # ------------------------------------------------------- #
-# Search_and_filter
+# SearchAndFilter
 # APIs for searching, querying, filtering, and aggregating records.
 # Specification: workspace:v1.0
 # ------------------------------------------------------- #
 
-from requests import Response
-
+from xata.api_response import ApiResponse
 from xata.namespace import Namespace
 
 
-class Search_and_filter(Namespace):
+class SearchAndFilter(Namespace):
 
     scope = "workspace"
 
-    def queryTable(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def query(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         The Query Table API can be used to retrieve all records in a table.  The API support
         filtering, sorting, selecting a subset of columns, and pagination.  The overall structure
         of the request looks like this:  ```json // POST
         /db/<dbname>:<branch>/tables/<table>/query {   "columns": [...],   "filter": {     "$all":
         [...],     "$any": [...]     ...   },   "sort": {     "multiple": [...]     ...   },
         "page": {     ...   } } ```  For usage, see also the [API Guide](https://xata.io/docs/api-
@@ -216,54 +215,55 @@
         Path: /db/{db_branch_name}/tables/{table_name}/query
         Method: POST
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
+        - 503: ServiceUnavailable
         - 5XX: Unexpected Error
 
         :param table_name: str The Table name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/query"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def searchBranch(self, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def search_branch(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Run a free text search operation across the database branch.
 
         Path: /db/{db_branch_name}/search
         Method: POST
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
-        - 503: Unexpected Error
+        - 503: ServiceUnavailable
         - 5XX: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/search"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def searchTable(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def search_table(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Run a free text search operation in a particular table.  The endpoint accepts a `query`
         parameter that is used for the free text search and a set of structured filters (via the
         `filter` parameter) that are applied before the search.  The `filter` parameter uses the
         same syntax as the [query endpoint](/api-reference/db/db_branch_name/tables/table_name/)
         with the following exceptions: * filters `$contains`, `$startsWith`, `$endsWith` don't
         work on columns of type `text` * filtering on columns of type `multiple` is currently
@@ -286,17 +286,17 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/search"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def vectorSearchTable(
+    def vector_search(
         self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None
-    ) -> Response:
+    ) -> ApiResponse:
         """
         This endpoint can be used to perform vector-based similarity searches in a table.  It can
         be used for implementing semantic search and product recommendation.  To use this
         endpoint, you need a column of type vector.  The input vector must have the same dimension
         as the vector column.
 
         Path: /db/{db_branch_name}/tables/{table_name}/vectorSearch
@@ -316,22 +316,22 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/vectorSearch"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def askTable(
+    def ask(
         self,
         table_name: str,
         payload: dict,
         db_name: str = None,
         branch_name: str = None,
         response_content_type: str = "application/json",
-    ) -> Response:
+    ) -> ApiResponse:
         """
         Ask your table a question.  If the `Accept` header is set to `text/event-stream`, Xata
         will stream the results back as SSE's.
 
         Path: /db/{db_branch_name}/tables/{table_name}/ask
         Method: POST
         Response status codes:
@@ -358,15 +358,47 @@
         url_path = f"/db/{db_branch_name}/tables/{table_name}/ask"
         headers = {
             "content-type": "application/json",
             "accept": response_content_type,
         }
         return self.request("POST", url_path, headers, payload)
 
-    def summarizeTable(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def chat_session_message(
+        self, table_name: str, session_id: str, payload: dict, db_name: str = None, branch_name: str = None
+    ) -> ApiResponse:
+        """
+        Ask a follow-up question.  If the `Accept` header is set to `text/event-stream`, Xata will
+        stream the results back as SSE's.
+
+        Path: /db/{db_branch_name}/tables/{table_name}/ask/{session_id}
+        Method: POST
+        Response status codes:
+        - 200: Response to the question
+        - 400: Bad Request
+        - 401: Authentication Error
+        - 404: Example response
+        - 429: Rate limit exceeded
+        - 503: ServiceUnavailable
+        - 5XX: Unexpected Error
+        Response: application/json
+
+        :param table_name: str The Table name
+        :param session_id: str
+        :param payload: dict content
+        :param db_name: str = None The name of the database to query. Default: database name from the client.
+        :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
+
+        :return Response
+        """
+        db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
+        url_path = f"/db/{db_branch_name}/tables/{table_name}/ask/{session_id}"
+        headers = {"content-type": "application/json"}
+        return self.request("POST", url_path, headers, payload)
+
+    def summarize(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         This endpoint allows you to (optionally) define groups, and then to run calculations on
         the values in each group.  This is most helpful when  you'd like to understand the data
         you have in your database.  A group is a combination of unique values.  If you create a
         group for  `sold_by`, `product_name`, we will return one row for every combination  of
         `sold_by` and `product_name` you have in your database.  When you  want to calculate
         statistics, you define these groups and ask Xata to  calculate data on each group.  **Some
@@ -415,15 +447,15 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/summarize"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def aggregateTable(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def aggregate(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         This endpoint allows you to run aggregations (analytics) on the data from one table.
         While the summary endpoint is served from a transactional store and the results are
         strongly  consistent, the aggregate endpoint is served from our columnar store and the
         results are  only eventually consistent.  On the other hand, the aggregate endpoint uses a
         store that is more appropiate for analytics, makes use of approximative algorithms  (e.g
         for cardinality), and is generally faster and can do more complex aggregations.  For
```

### Comparing `xata-0.9.3/xata/namespaces/workspace/table.py` & `xata-1.0.0a1/xata/api/table.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,24 +19,23 @@
 
 # ------------------------------------------------------- #
 # Table
 # Table management.
 # Specification: workspace:v1.0
 # ------------------------------------------------------- #
 
-from requests import Response
-
+from xata.api_response import ApiResponse
 from xata.namespace import Namespace
 
 
 class Table(Namespace):
 
     scope = "workspace"
 
-    def createTable(self, table_name: str, db_name: str = None, branch_name: str = None) -> Response:
+    def create(self, table_name: str, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Creates a new table with the given name.  Returns 422 if a table with the same name
         already exists.
 
         Path: /db/{db_branch_name}/tables/{table_name}
         Method: PUT
         Response status codes:
@@ -55,15 +54,15 @@
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}"
         return self.request("PUT", url_path)
 
-    def deleteTable(self, table_name: str, db_name: str = None, branch_name: str = None) -> Response:
+    def delete(self, table_name: str, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Deletes the table with the given name.
 
         Path: /db/{db_branch_name}/tables/{table_name}
         Method: DELETE
         Response status codes:
         - 200: OK
@@ -79,15 +78,15 @@
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}"
         return self.request("DELETE", url_path)
 
-    def updateTable(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def update(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Update table.  Currently there is only one update operation supported: renaming the table
         by providing a new name.  In the example below, we rename a table from “users” to
         “people”:  ```json // PATCH /db/test:main/tables/users  {   "name": "people" } ```
 
         Path: /db/{db_branch_name}/tables/{table_name}
         Method: PATCH
@@ -107,15 +106,15 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}"
         headers = {"content-type": "application/json"}
         return self.request("PATCH", url_path, headers, payload)
 
-    def getTableSchema(self, table_name: str, db_name: str = None, branch_name: str = None) -> Response:
+    def get_schema(self, table_name: str, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Get table schema
 
         Path: /db/{db_branch_name}/tables/{table_name}/schema
         Method: GET
         Response status codes:
         - 200: OK
@@ -131,15 +130,15 @@
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/schema"
         return self.request("GET", url_path)
 
-    def setTableSchema(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def set_schema(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Update table schema
 
         Path: /db/{db_branch_name}/tables/{table_name}/schema
         Method: PUT
         Response status codes:
         - 200: Schema migration response with ID and migration status.
@@ -158,15 +157,15 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/schema"
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
-    def getTableColumns(self, table_name: str, db_name: str = None, branch_name: str = None) -> Response:
+    def get_columns(self, table_name: str, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Retrieves the list of table columns and their definition.  This endpoint returns the
         column list with object columns being reported with their full dot-separated path
         (flattened).
 
         Path: /db/{db_branch_name}/tables/{table_name}/columns
         Method: GET
@@ -184,21 +183,18 @@
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/columns"
         return self.request("GET", url_path)
 
-    def addTableColumn(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+    def add_column(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Adds a new column to the table.  The body of the request should contain the column
-        definition.  In the column definition, the 'name' field should contain the full path
-        separated by dots.  If the parent objects do not exists, they will be automatically
-        created.  For example, passing `"name": "address.city"` will auto-create the `address`
-        object if it doesn't exist.
+        definition.
 
         Path: /db/{db_branch_name}/tables/{table_name}/columns
         Method: POST
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
@@ -213,18 +209,19 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/columns"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def getColumn(self, table_name: str, column_name: str, db_name: str = None, branch_name: str = None) -> Response:
+    def get_column(
+        self, table_name: str, column_name: str, db_name: str = None, branch_name: str = None
+    ) -> ApiResponse:
         """
-        Get the definition of a single column.  To refer to sub-objects, the column name can
-        contain dots.  For example `address.country`.
+        Get the definition of a single column.
 
         Path: /db/{db_branch_name}/tables/{table_name}/columns/{column_name}
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
@@ -239,18 +236,19 @@
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/columns/{column_name}"
         return self.request("GET", url_path)
 
-    def deleteColumn(self, table_name: str, column_name: str, db_name: str = None, branch_name: str = None) -> Response:
+    def delete_column(
+        self, table_name: str, column_name: str, db_name: str = None, branch_name: str = None
+    ) -> ApiResponse:
         """
-        Deletes the specified column.  To refer to sub-objects, the column name can contain dots.
-        For example `address.country`.
+        Deletes the specified column.
 
         Path: /db/{db_branch_name}/tables/{table_name}/columns/{column_name}
         Method: DELETE
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
@@ -264,21 +262,20 @@
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/columns/{column_name}"
         return self.request("DELETE", url_path)
 
-    def updateColumn(
+    def update_column(
         self, table_name: str, column_name: str, payload: dict, db_name: str = None, branch_name: str = None
-    ) -> Response:
+    ) -> ApiResponse:
         """
         Update column with partial data.  Can be used for renaming the column by providing a new
-        "name" field.  To refer to sub-objects, the column name can contain dots.  For example
-        `address.country`.
+        "name" field.
 
         Path: /db/{db_branch_name}/tables/{table_name}/columns/{column_name}
         Method: PATCH
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
```

### Comparing `xata-0.9.3/PKG-INFO` & `xata-1.0.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xata
-Version: 0.9.3
+Version: 1.0.0a1
 Summary: Python client for Xata.io
 License: Apache-2.0
 Author: Xata
 Author-email: support@xata.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

