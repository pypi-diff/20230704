# Comparing `tmp/python-sapcommissions-1.0.1.tar.gz` & `tmp/python-sapcommissions-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sapcommissions-1.0.1.tar", last modified: Tue Jun 27 05:20:29 2023, max compression
+gzip compressed data, was "python-sapcommissions-1.0.2.tar", last modified: Tue Jun 27 14:08:07 2023, max compression
```

## Comparing `python-sapcommissions-1.0.1.tar` & `python-sapcommissions-1.0.2.tar`

### file list

```diff
@@ -1,33 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.125092 python-sapcommissions-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.117092 python-sapcommissions-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.121092 python-sapcommissions-1.0.1/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.121092 python-sapcommissions-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.121092 python-sapcommissions-1.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-06-27 05:20:29.125092 python-sapcommissions-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.121092 python-sapcommissions-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    12172 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/docs/ENDPOINTS.md
--rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.121092 python-sapcommissions-1.0.1/python_sapcommissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-06-27 05:20:29.000000 python-sapcommissions-1.0.1/python_sapcommissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-27 05:20:29.000000 python-sapcommissions-1.0.1/python_sapcommissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:20:29.000000 python-sapcommissions-1.0.1/python_sapcommissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-27 05:20:29.000000 python-sapcommissions-1.0.1/python_sapcommissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 05:20:29.000000 python-sapcommissions-1.0.1/python_sapcommissions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.121092 python-sapcommissions-1.0.1/sapcommissions/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/sapcommissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24379 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/sapcommissions/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/sapcommissions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)   112084 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/sapcommissions/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 05:20:29.125092 python-sapcommissions-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.125092 python-sapcommissions-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/tests/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.967275 python-sapcommissions-1.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.967275 python-sapcommissions-1.0.2/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.github/workflows/pr-labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    12172 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/docs/ENDPOINTS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/python_sapcommissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-06-27 14:08:07.000000 python-sapcommissions-1.0.2/python_sapcommissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-27 14:08:07.000000 python-sapcommissions-1.0.2/python_sapcommissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:08:07.000000 python-sapcommissions-1.0.2/python_sapcommissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 14:08:07.000000 python-sapcommissions-1.0.2/python_sapcommissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 14:08:07.000000 python-sapcommissions-1.0.2/python_sapcommissions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/sapcommissions/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/sapcommissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25047 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/sapcommissions/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/sapcommissions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112297 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/sapcommissions/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/tests/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/tox.ini
```

### Comparing `python-sapcommissions-1.0.1/.github/scripts/release.py` & `python-sapcommissions-1.0.2/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.0.1/.github/workflows/publish.yml` & `python-sapcommissions-1.0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.0.1/LICENSE` & `python-sapcommissions-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.0.1/PKG-INFO` & `python-sapcommissions-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sapcommissions
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python wrapper for the SAP Commissions API
 Author-email: Niels Perfors <niels.perfors1987@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/niro1987/python-sapcommissions
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
```

### Comparing `python-sapcommissions-1.0.1/docs/ENDPOINTS.md` & `python-sapcommissions-1.0.2/docs/ENDPOINTS.md`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.0.1/docs/README.md` & `python-sapcommissions-1.0.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.0.1/python_sapcommissions.egg-info/PKG-INFO` & `python-sapcommissions-1.0.2/python_sapcommissions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sapcommissions
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python wrapper for the SAP Commissions API
 Author-email: Niels Perfors <niels.perfors1987@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/niro1987/python-sapcommissions
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
```

### Comparing `python-sapcommissions-1.0.1/sapcommissions/__init__.py` & `python-sapcommissions-1.0.2/sapcommissions/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,23 +10,23 @@
     Connection variables used to connect with SAP Commissions.
     """
 
     tenant: str = field(repr=True)
     environment: str = field(repr=True)
     username: str = field(repr=True)
     password: str = field(repr=False)
-    verify_ssl: bool = field(default=True, repr=False)
+    verifySsl: bool = field(default=True, repr=False)
 
     @property
     def url(self) -> str:
         """Return the Commissions URL."""
         return f"https://{self.tenant}-{self.environment}.callidusondemand.com"
 
     @property
-    def api_url(self) -> str:
+    def apiUrl(self) -> str:
         """Returns the base url for the Commissions REST API."""
         return self.url + "/api"
 
     @property
-    def api_document(self) -> str:
+    def apiDocument(self) -> str:
         """Returns the url for the Commissions API documentation."""
         return self.url + "/APIDocument"
```

### Comparing `python-sapcommissions-1.0.1/sapcommissions/endpoints.py` & `python-sapcommissions-1.0.2/sapcommissions/endpoints.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Endpoints are used to interact with SAP Commissions objects."""
 import logging
 from datetime import date
 from typing import Any
 
 from requests.auth import HTTPBasicAuth
 from requests.exceptions import HTTPError
 from requests.models import Response
@@ -15,37 +16,37 @@
 
 
 class _Client(Session):
     """Interacts with SAP Commissions REST API. Extends requests.Session."""
 
     def __init__(
         self,
-        base_url: str,
+        baseUrl: str,
         username: str,
         password: str,
-        verify_ssl: bool = True,
+        verifySsl: bool = True,
     ) -> None:
         """Initialize an endpoint to interact with SAP Commissions."""
         super().__init__()
-        self.base_url: str = base_url
+        self.baseUrl: str = baseUrl
         self.auth = HTTPBasicAuth(username, password)
-        if verify_ssl is False:
+        if verifySsl is False:
             disable_warnings()
-            self.verify = verify_ssl
+            self.verify = verifySsl
 
-    def request(
+    def request(  # pylint: disable=arguments-differ
         self,
         method: str,
         uri: str,
         parameters: dict[str, str] | None = None,
         body: list[dict[str, str]] | None = None,
     ) -> dict[str, Any | list[dict[str, Any]]] | Response:
         """Perform an HTTP request to the SAP Commissions REST API."""
         LOGGER.debug("%s %s %s", method.upper(), uri, parameters)
-        url: str = self.base_url + uri
+        url: str = self.baseUrl + uri
         with super().request(
             method=method,
             url=url,
             params=parameters,
             json=body,
         ) as response:
             try:
@@ -59,69 +60,72 @@
                     method.upper(),
                     response.status_code,
                     uri,
                     response.text,
                 )
                 if 401 <= response.status_code <= 403:
                     raise AuthenticationError(response.text) from error
-                elif 400 <= response.status_code < 500:
+                if 400 <= response.status_code < 500:
                     raise ClientError(response.text) from error
-                elif 500 <= response.status_code < 600:
+                if 500 <= response.status_code < 600:
                     raise ServerError(response.text) from error
+        return None
 
-    def get(
+    def get(  # pylint: disable=arguments-renamed,arguments-differ
         self,
         uri: str,
         parameters: dict[str, str] | None = None,
     ) -> dict[str, Any | list[dict[str, Any]]]:
         """Perform a GET request to the SAP Commissions REST API."""
         return self.request("GET", uri, parameters=parameters)
 
-    def delete(
+    def delete(  # pylint: disable=arguments-renamed,arguments-differ
         self, uri: str, parameters: dict[str, str] | None = None
     ) -> dict[str, Any | list[dict[str, Any]]]:
         """Perform a DELETE request to the SAP Commissions REST API."""
         return self.request("DELETE", uri, parameters=parameters)
 
-    def post(
+    def post(  # pylint: disable=arguments-renamed,arguments-differ
         self, uri: str, body: list[dict[str, str]]
     ) -> dict[str, Any | list[dict[str, Any]]]:
         """Perform a POST request to the SAP Commissions REST API."""
         return self.request("POST", uri, body=body)
 
-    def put(
+    def put(  # pylint: disable=arguments-renamed,arguments-differ
         self, uri: str, body: list[dict[str, str]]
     ) -> dict[str, Any | list[dict[str, Any]]]:
         """Perform a PUT request to the SAP Commissions REST API."""
         return self.request("PUT", uri, body=body)
 
 
 class _Endpoint:
     """Provides a base template for an endpoint method."""
 
     resource: resources._Resource
 
     def __init__(self, connection: Connection) -> None:
         """Initialize a base template for an endpoint method."""
         self._client = _Client(
-            base_url=connection.api_url,
+            baseUrl=connection.apiUrl,
             username=connection.username,
             password=connection.password,
-            verify_ssl=connection.verify_ssl,
+            verifySsl=connection.verifySsl,
         )
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.name})"
 
     @property
     def name(self) -> str:
-        return self.resource._name
+        """Returns the name of the resource."""
+        return self.resource._name  # pylint: disable=protected-access
 
     @property
     def url(self) -> str:
+        """Returns the API URL of the endpoint."""
         return f"/v2/{self.name}"
 
 
 class _Create(_Endpoint):
     def create(self, instance: resources._Resource) -> resources._Resource:
         """
         Create a new resource for the endpoint.
@@ -217,15 +221,15 @@
             Resource effectiveEndDate.
         fillFromRight : bool
             If true, then the gap will be filled by the right (next) version,
             otherwise by the left (prev) version. Default is false (prev).
         """
         LOGGER.info("Delete versions for %s with seq %s", self.name, seq)
 
-        query = dict()
+        query = {}
         assert isinstance(seq, int)
         assert isinstance(effectiveStartDate, date)
         query["effectiveStartDate"] = effectiveStartDate.strftime("%Y-%m-%d")
         assert isinstance(effectiveEndDate, date)
         query["effectiveEndDate"] = effectiveEndDate.strftime("%Y-%m-%d")
         assert isinstance(fillFromRight, bool)
         query["fillFromRight"] = fillFromRight
@@ -274,15 +278,15 @@
         startDate : date
             Filter List for resources effective for startDate.
         endDate : date
             Filter List for resources effective for endDate.
         """
         LOGGER.info("Get versions of %s with seq %s", self.name, seq)
 
-        query = dict()
+        query = {}
         assert isinstance(seq, int)
         if startDate:
             assert isinstance(startDate, date)
             query["startDate"] = startDate.strftime("%Y-%m-%d")
         if endDate:
             assert isinstance(endDate, date)
             query["endDate"] = endDate.strftime("%Y-%m-%d")
@@ -293,15 +297,15 @@
 
         return resource_versions
 
 
 class _List(_Endpoint):
     def list(
         self,
-        filter: str = None,
+        filter: str = None,  # pylint: disable=redefined-builtin
         startDate: date = None,
         endDate: date = None,
         limit: int = None,
         raw: bool = False,
         **filter_kwargs: dict,
     ) -> list[resources._Resource]:
         """
@@ -334,15 +338,15 @@
 
         The keyword arguments are converted to filters. The keyword must be a
         part of the resource's attributes.
         """
         LOGGER.info("List %s", self.name)
 
         query = {"top": limit if limit and limit < 100 else 100}
-        if expand := self.resource._expands:
+        if expand := self.resource._expands:  # pylint: disable=protected-access
             query["expand"] = ",".join(expand)
         if filter:
             assert isinstance(filter, str)
             query["$filter"] = filter
         if startDate:
             assert isinstance(startDate, date)
             # Unlike the other methods, this one requires a date in [YYYY/MM/DD]
@@ -379,15 +383,15 @@
                 yield item if raw else self.resource.from_dict(item)
                 yield_count += 1
                 if limit and yield_count >= limit:
                     return
 
     def get_id(
         self,
-        id: str,
+        id: str,  # pylint: disable=redefined-builtin
         raw: bool = False,
     ) -> resources._Resource:
         """
         Reads all of the attributes of an existing resource.
 
         Parameters
         ----------
@@ -396,36 +400,36 @@
         raw : bool
             If true, then the response is returned as is, otherwise it is converted
             to resource objects. Default is False.
         """
         LOGGER.info("Get %s with id %s", self.name, id)
 
         assert isinstance(id, str)
-        id_attr = self.resource._id_attr
-        if id_attr is None:
+        # pylint: disable-next=protected-access
+        if (id_attr := self.resource._idAttr) is None:
             LOGGER.warning("%s has no id attribute.", self.name)
             return None
 
         query = {"top": 10}
-        if expand := self.resource._expands:
+        if expand := self.resource._expands:  # pylint: disable=protected-access
             query["expand"] = ",".join(expand)
         query["$filter"] = f"{id_attr} eq '{id}'"
 
         response = self._client.get(self.url, query)
         data = response[self.name]
         items = data if raw else [self.resource.from_dict(item) for item in data]
         if len(data) > 1:
             LOGGER.warning("Returned %s items for id %s.", len(data), id)
         item = items[0] if items else None
 
         return item
 
     def count(
         self,
-        filter: str = None,
+        filter: str = None,  # pylint: disable=redefined-builtin
         startDate: date = None,
         endDate: date = None,
         **filter_kwargs: dict,
     ) -> int:
         """
         Returns the number of resources.
```

### Comparing `python-sapcommissions-1.0.1/sapcommissions/resources.py` & `python-sapcommissions-1.0.2/sapcommissions/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,65 +8,65 @@
 from datetime import date, datetime, timezone
 from types import UnionType
 from typing import ClassVar, get_args, get_origin, get_type_hints
 
 LOGGER = logging.getLogger(__name__)
 
 
-def _decode(value, astype):
+def _decode(value, astype):  # pylint: disable=too-many-return-statements
     if isinstance(value, list):
         if astype is list:
             LOGGER.error("Unknown type for list elements: %s", astype)
-            raise TypeError("Unknown type for list elements: %s", astype)
+            raise TypeError("Unknown type for list elements")
         if get_origin(astype) is list:
             if len(subtypes := get_args(astype)) > 1:
                 LOGGER.error("Impropper type for list elements: %s", subtypes)
-                raise TypeError("Impropper type for list elements: %s", subtypes)
+                raise TypeError("Impropper type for list elements")
             return [_decode(v, subtypes[0]) for v in value]
         LOGGER.error("Impropper type, value is list: %s", astype)
-        raise TypeError("Impropper type, value is list: %s", astype)
+        raise TypeError("Impropper type, value is list")
     if isinstance(astype, UnionType):
         LOGGER.error("UnionType is not supported: %s", astype)
-        raise NotImplementedError("Unsupported type: %s", astype)
+        raise NotImplementedError("Unsupported type")
     if value is None:
         return None
     if astype is datetime:
         return datetime.fromisoformat(value).astimezone(timezone.utc)
     if astype is date:
         return datetime.fromisoformat(value).astimezone(timezone.utc).date()
     if isinstance(value, astype):
         return value
     if issubclass(astype, _Resource) and isinstance(value, dict):
         return astype.from_dict(value)
     if issubclass(astype, _Resource) and isinstance(value, (str, int)):
-        return astype(**{astype._seq_attr: value})
+        return astype(**{astype._seqAttr: value})  # pylint: disable=protected-access
     return astype(value)
 
 
 def _encode(value, fromtype):
     if isinstance(value, list):
         if fromtype is list:
             LOGGER.error("Unknown type for list elements: %s", fromtype)
-            raise TypeError("Unknown type for list elements: %s", fromtype)
+            raise TypeError("Unknown type for list elements")
         if get_origin(fromtype) is list:
             if len(subtypes := get_args(fromtype)) > 1:
                 LOGGER.error("Impropper type for list elements: %s", subtypes)
-                raise TypeError("Impropper type for list elements: %s", subtypes)
+                raise TypeError("Impropper type for list elements")
             return [_decode(v, subtypes[0]) for v in value]
         LOGGER.error("Impropper type, value is list: %s", fromtype)
-        raise TypeError("Impropper type, value is list: %s", fromtype)
+        raise TypeError("Impropper type, value is list")
     if isinstance(fromtype, UnionType):
         LOGGER.error("UnionType is not supported: %s", fromtype)
-        raise NotImplementedError("Unsupported type: %s", fromtype)
+        raise NotImplementedError("Unsupported type")
     if value is None:
         return None
     if isinstance(value, (datetime, date)):
         return value.isoformat()
-    elif isinstance(value, _Resource):
-        return value.to_dict(ignore_seq=False)
+    if isinstance(value, _Resource):
+        return value.to_dict(ignoreSeq=False)
     if isinstance(value, int):
         return value
     return str(value)
 
 
 class _Resource:
     _endpoint_name: ClassVar[str]
@@ -75,69 +75,72 @@
     @property
     def _name(cls) -> str:
         """Returns the name resource."""
         return cls._endpoint_name
 
     @classmethod
     @property
-    def _seq_attr(cls) -> str | None:
+    def _seqAttr(cls) -> str | None:
         """Returns the name of the sequence attribute or None."""
-        for f in fields(cls):
-            if f.metadata.get("seq"):
-                return f.name
+        for fld in fields(cls):
+            if fld.metadata.get("seq"):
+                return fld.name
+        return None
 
     @property
     def _seq(self) -> int | None:
         """Returns the sequence or None."""
-        seq_attr = self._seq_attr
+        seq_attr = self._seqAttr
         return self[seq_attr] if seq_attr else None
 
     @classmethod
     @property
-    def _id_attr(cls) -> str | None:
+    def _idAttr(cls) -> str | None:
         """Returns the name of the identifier attribute or None."""
-        for f in fields(cls):
-            if f.metadata.get("id"):
-                return f.name
+        for fld in fields(cls):
+            if fld.metadata.get("id"):
+                return fld.name
+        return None
 
     @property
     def _id(self) -> str | None:
         """Returns the identifier or None."""
-        id_attr = self._id_attr
+        id_attr = self._idAttr
         return self[id_attr] if id_attr else None
 
     @classmethod
     @property
     def _expands(cls) -> tuple:
         """Returns the name of the expandable attributes."""
         return tuple(f.name for f in fields(cls) if f.metadata.get("expand"))
 
     @classmethod
     def from_dict(cls, json: dict) -> _Resource:
+        """Convert dictionary to _Resource instance."""
         types = get_type_hints(cls)
         invalid_json = {k: v for k, v in json.items() if k not in types.keys()}
         for field_name in invalid_json.keys():
             LOGGER.warning("%s is not a valid field for %s", field_name, cls.__name__)
         valid_json = {k: v for k, v in json.items() if k in types.keys()}
         for field_name, value in valid_json.items():
             valid_json[field_name] = _decode(value, types[field_name])
         return cls(**valid_json)
 
-    def to_dict(self, ignore_seq: bool = True) -> dict:
+    def to_dict(self, ignoreSeq: bool = True) -> dict:
+        """Convert _Resource instance to dictionary."""
         types = get_type_hints(self.__class__)
         data = {}
-        for f in fields(self):
-            value = self[f.name]
-            if value is None:
+        for fld in fields(self):
+            if (value := self[fld.name]) is None:
                 continue
-            if f.metadata.get("json_ignore"):
+            if fld.metadata.get("json_ignore"):
                 continue
-            if ignore_seq and f.metadata.get("seq"):
+            if ignoreSeq and fld.metadata.get("seq"):
                 continue
-            data[f.name] = _encode(value, types[f.name])
+            data[fld.name] = _encode(value, types[fld.name])
         return data
 
     def __getitem__(self, attribute: str):
         return getattr(self, attribute)
 
 
 @dataclass(frozen=True)
@@ -937,15 +940,15 @@
     dimensionType: int = field(default=None, repr=False)
     dimensionSlot: int = field(default=None, repr=False)
     dimensionUnitType: UnitType = field(default=None, repr=False)
     isRanged: bool = field(default=None, repr=False)
     includeStartInRange: bool = field(default=None, repr=False)
     includeEndInRange: bool = field(default=None, repr=False)
     flags: str = field(default=None, repr=False)
-    MDLT: LookUpTable = field(default=None, repr=False)
+    MDLT: LookUpTable = field(default=None, repr=False)  # pylint: disable=invalid-name
     categoryTree: CategoryTree = field(default=None, repr=False)
     modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
     etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
 
 
 @dataclass
 class LookUpTableIndice(_Resource):
@@ -956,21 +959,21 @@
     maxString: str = field(default=None, repr=False)
     minValue: str = field(default=None, repr=False)
     maxValue: str = field(default=None, repr=False)
     minDate: date = field(default=None, repr=False)
     maxDate: date = field(default=None, repr=False)
     validStart: date = field(default=None, repr=False)
     validEnd: date = field(default=None, repr=False)
-    classifier: str = field(default=None, repr=False)  # TODO Implement Classifier
-    category: str = field(default=None, repr=False)  # TODO Implement Category
+    classifier: str = field(default=None, repr=False)  # Implement Classifier
+    category: str = field(default=None, repr=False)  # Implement Category
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
     createDate: datetime = field(default=None, repr=False)
     removeDate: datetime = field(default=None, repr=False)
-    MDLT: LookUpTable = field(default=None, repr=False)
+    MDLT: LookUpTable = field(default=None, repr=False)  # pylint: disable=invalid-name
     dimensionSeq: LookUpTableDimension = field(default=None, repr=False)
     modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
     etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
 
 
 @dataclass
 class LookUpTableVariable(_Resource):
@@ -1357,15 +1360,15 @@
     pipelineRun: Pipeline = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     pipelineRunDate: datetime = field(default=None, repr=False)
     appliedDeposit: Value = field(default=None, repr=False)
     priorBalance: Value = field(default=None, repr=False)
     balance: Value = field(default=None, repr=False)
     payment: Value = field(default=None, repr=False)
-    Deposit: Value = field(default=None, repr=False)
+    Deposit: Value = field(default=None, repr=False)  # pylint: disable=invalid-name
     outstandingBalance: Value = field(default=None, repr=False)
     etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
 
 
 @dataclass
 class Period(_Resource):
     _endpoint_name: ClassVar[str] = "periods"
```

### Comparing `python-sapcommissions-1.0.1/tests/test_base.py` & `python-sapcommissions-1.0.2/tests/test_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,72 @@
+"""Tests for the sapcommissions module."""
 import unittest
 from dataclasses import asdict
 
 from sapcommissions import Connection
 
 
 class TestConnection(unittest.TestCase):
+    """Tests for the Connection class."""
+
     def test_url(self):
+        """Test the url attribute."""
         # Create a connection instance to test
         conn = Connection(
             tenant="spam", environment="eggs", username="user", password="pass"
         )
 
         # Check that the url property returns the expected value
         self.assertEqual(conn.url, "https://spam-eggs.callidusondemand.com")
 
     def test_api_url(self):
+        """Test the apiUrl attribute."""
         # Create a connection instance to test
         conn = Connection(
             tenant="spam", environment="eggs", username="user", password="pass"
         )
 
         # Check that the api_url property returns the expected value
-        self.assertEqual(conn.api_url, "https://spam-eggs.callidusondemand.com/api")
+        self.assertEqual(conn.apiUrl, "https://spam-eggs.callidusondemand.com/api")
 
     def test_api_document(self):
+        """Test the apiDocument attribute."""
         # Create a connection instance to test
         conn = Connection(
             tenant="spam", environment="eggs", username="user", password="pass"
         )
 
         # Check that the api_document property returns the expected value
         self.assertEqual(
-            conn.api_document, "https://spam-eggs.callidusondemand.com/APIDocument"
+            conn.apiDocument, "https://spam-eggs.callidusondemand.com/APIDocument"
         )
 
     def test_connection_dataclass(self):
+        """Test the Connection dataclass."""
         # Check that the Connection dataclass is defined correctly
         conn_dict = {
             "tenant": "spam",
             "environment": "eggs",
             "username": "user",
             "password": "pass",
-            "verify_ssl": True,
+            "verifySsl": True,
         }
 
         # Check that the fields of the Connection instance match the values in conn_dict
         conn = Connection(**conn_dict)
         self.assertEqual(asdict(conn), conn_dict)
 
         # Check that the verify_ssl field defaults to True if not provided
-        del conn_dict["verify_ssl"]
+        del conn_dict["verifySsl"]
         conn = Connection(**conn_dict)
-        conn_dict["verify_ssl"] = True  # Verify that verify_ssl defaults to True
+        conn_dict["verifySsl"] = True  # Verify that verify_ssl defaults to True
         self.assertEqual(asdict(conn), conn_dict)
 
     def test_hidden_password(self):
+        """Test the password visibility."""
         # Create a connection instance to test
         conn = Connection(
             tenant="spam", environment="eggs", username="foo", password="barbaz"
         )
 
         # Check that the password property is hidden from the string representation.
         self.assertNotIn("barbaz", str(conn))
```

### Comparing `python-sapcommissions-1.0.1/tests/test_endpoints.py` & `python-sapcommissions-1.0.2/tests/test_endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
     def test_url(self):
         # Check that the url property returns the correct value
         self.assertEqual(self.endpoint.url, "/v2/test_resource")
 
     def test_init(self):
         # Check that the endpoint was initialized correctly
         self.assertEqual(
-            self.endpoint._client.base_url,
+            self.endpoint._client.baseUrl,
             "https://spam-eggs.callidusondemand.com/api",
         )
         self.assertEqual(self.endpoint._client.auth.username, "user")
         self.assertEqual(self.endpoint._client.auth.password, "pass")
         self.assertTrue(self.endpoint._client.verify)
```

### Comparing `python-sapcommissions-1.0.1/tests/test_resources.py` & `python-sapcommissions-1.0.2/tests/test_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,21 @@
         }
         self.resource: DummyResource = DummyResource.from_dict(self.resource_dict)
 
     def test_name_property(self):
         self.assertEqual(DummyResource._name, "test")
 
     def test_seq_attr_property(self):
-        self.assertIsNone(DummyResource._seq_attr)
+        self.assertIsNone(DummyResource._seqAttr)
 
     def test_seq_property(self):
         self.assertIsNone(self.resource._seq)
 
     def test_id_attr_property(self):
-        self.assertEqual(DummyResource._id_attr, "id")
+        self.assertEqual(DummyResource._idAttr, "id")
 
     def test_id_property(self):
         self.assertEqual(self.resource._id, "123")
 
     def test_expands_property(self):
         self.assertEqual(DummyResource._expands, ("expands",))
```

