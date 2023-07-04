# Comparing `tmp/pyPreservica-2.0.2.tar.gz` & `tmp/pyPreservica-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPreservica-2.0.2.tar", last modified: Tue Jun 27 11:39:03 2023, max compression
+gzip compressed data, was "pyPreservica-2.0.3.tar", last modified: Tue Jul  4 09:08:45 2023, max compression
```

## Comparing `pyPreservica-2.0.2.tar` & `pyPreservica-2.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 11:39:03.627097 pyPreservica-2.0.2/
--rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-2.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2581 2023-06-27 11:39:03.626100 pyPreservica-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 11:39:03.587595 pyPreservica-2.0.2/pyPreservica/
--rw-rw-rw-   0        0        0     1096 2023-06-27 11:38:36.000000 pyPreservica-2.0.2/pyPreservica/__init__.py
--rw-rw-rw-   0        0        0    37685 2023-05-03 10:58:47.000000 pyPreservica-2.0.2/pyPreservica/adminAPI.py
--rw-rw-rw-   0        0        0    34848 2023-06-27 11:35:07.000000 pyPreservica-2.0.2/pyPreservica/common.py
--rw-rw-rw-   0        0        0    16257 2023-05-24 17:32:04.000000 pyPreservica-2.0.2/pyPreservica/contentAPI.py
--rw-rw-rw-   0        0        0   105700 2023-05-25 09:37:03.000000 pyPreservica-2.0.2/pyPreservica/entityAPI.py
--rw-rw-rw-   0        0        0     6258 2023-05-16 11:37:54.000000 pyPreservica-2.0.2/pyPreservica/monitorAPI.py
--rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-2.0.2/pyPreservica/opex.py
--rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-2.0.2/pyPreservica/parAPI.py
--rw-rw-rw-   0        0        0    23612 2023-05-24 17:32:04.000000 pyPreservica-2.0.2/pyPreservica/retentionAPI.py
--rw-rw-rw-   0        0        0    92455 2023-06-06 12:57:35.000000 pyPreservica-2.0.2/pyPreservica/uploadAPI.py
--rw-rw-rw-   0        0        0     5729 2023-05-26 10:55:42.000000 pyPreservica-2.0.2/pyPreservica/vocabularyAPI.py
--rw-rw-rw-   0        0        0     6736 2023-05-24 08:15:02.000000 pyPreservica-2.0.2/pyPreservica/webHooksAPI.py
--rw-rw-rw-   0        0        0    17862 2023-05-24 17:32:04.000000 pyPreservica-2.0.2/pyPreservica/workflowAPI.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:39:03.620150 pyPreservica-2.0.2/pyPreservica.egg-info/
--rw-rw-rw-   0        0        0     2581 2023-06-27 11:39:02.000000 pyPreservica-2.0.2/pyPreservica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-06-27 11:39:02.000000 pyPreservica-2.0.2/pyPreservica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 11:39:02.000000 pyPreservica-2.0.2/pyPreservica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-06-27 11:39:02.000000 pyPreservica-2.0.2/pyPreservica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-27 11:39:02.000000 pyPreservica-2.0.2/pyPreservica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 11:39:03.629538 pyPreservica-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1654 2023-06-27 11:38:36.000000 pyPreservica-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:08:45.198521 pyPreservica-2.0.3/
+-rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-2.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2581 2023-07-04 09:08:45.198521 pyPreservica-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 09:08:45.160763 pyPreservica-2.0.3/pyPreservica/
+-rw-rw-rw-   0        0        0     1084 2023-07-04 08:59:07.000000 pyPreservica-2.0.3/pyPreservica/__init__.py
+-rw-rw-rw-   0        0        0    37685 2023-05-03 10:58:47.000000 pyPreservica-2.0.3/pyPreservica/adminAPI.py
+-rw-rw-rw-   0        0        0     9142 2023-07-04 08:59:07.000000 pyPreservica-2.0.3/pyPreservica/authorityAPI.py
+-rw-rw-rw-   0        0        0    34848 2023-07-03 10:50:28.000000 pyPreservica-2.0.3/pyPreservica/common.py
+-rw-rw-rw-   0        0        0    16257 2023-05-24 17:32:04.000000 pyPreservica-2.0.3/pyPreservica/contentAPI.py
+-rw-rw-rw-   0        0        0   105700 2023-05-25 09:37:03.000000 pyPreservica-2.0.3/pyPreservica/entityAPI.py
+-rw-rw-rw-   0        0        0     6258 2023-05-16 11:37:54.000000 pyPreservica-2.0.3/pyPreservica/monitorAPI.py
+-rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-2.0.3/pyPreservica/opex.py
+-rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-2.0.3/pyPreservica/parAPI.py
+-rw-rw-rw-   0        0        0    23612 2023-05-24 17:32:04.000000 pyPreservica-2.0.3/pyPreservica/retentionAPI.py
+-rw-rw-rw-   0        0        0    92455 2023-06-06 12:57:35.000000 pyPreservica-2.0.3/pyPreservica/uploadAPI.py
+-rw-rw-rw-   0        0        0     6736 2023-05-24 08:15:02.000000 pyPreservica-2.0.3/pyPreservica/webHooksAPI.py
+-rw-rw-rw-   0        0        0    17862 2023-05-24 17:32:04.000000 pyPreservica-2.0.3/pyPreservica/workflowAPI.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:08:45.192005 pyPreservica-2.0.3/pyPreservica.egg-info/
+-rw-rw-rw-   0        0        0     2581 2023-07-04 09:08:44.000000 pyPreservica-2.0.3/pyPreservica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      546 2023-07-04 09:08:44.000000 pyPreservica-2.0.3/pyPreservica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 09:08:44.000000 pyPreservica-2.0.3/pyPreservica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-04 09:08:44.000000 pyPreservica-2.0.3/pyPreservica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-04 09:08:44.000000 pyPreservica-2.0.3/pyPreservica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 09:08:45.198521 pyPreservica-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1654 2023-07-03 15:13:51.000000 pyPreservica-2.0.3/setup.py
```

### Comparing `pyPreservica-2.0.2/LICENSE.txt` & `pyPreservica-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.2/PKG-INFO` & `pyPreservica-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-2.0.2/README.md` & `pyPreservica-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.2/pyPreservica/__init__.py` & `pyPreservica-2.0.3/pyPreservica/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,16 +13,16 @@
                     cvs_to_cmis_xslt, csv_to_search_xml, generic_asset_package, upload_config, multi_asset_package
 from .workflowAPI import WorkflowAPI, WorkflowContext, WorkflowInstance
 from .retentionAPI import RetentionAPI, RetentionAssignment, RetentionPolicy
 from .parAPI import PreservationActionRegistry
 from .adminAPI import AdminAPI
 from .monitorAPI import MonitorAPI, MonitorCategory, MonitorStatus, MessageStatus
 from .webHooksAPI import WebHooksAPI, TriggerType, WebHookHandler
-from .vocabularyAPI import ControlledVocabularyAPI, Table
+from .authorityAPI import AuthorityAPI, Table
 
 
 __author__ = "James Carr (drjamescarr@gmail.com)"
 
 # Version of the Preservica API package
-__version__ = "2.0.2"
+__version__ = "2.0.3"
 
 __license__ = "Apache License Version 2.0"
```

### Comparing `pyPreservica-2.0.2/pyPreservica/adminAPI.py` & `pyPreservica-2.0.3/pyPreservica/adminAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.2/pyPreservica/common.py` & `pyPreservica-2.0.3/pyPreservica/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -729,15 +729,15 @@
             return self.__version_number__()
         else:
             logger.error(f"version number failed with http response {request.status_code}")
             logger.error(str(request.content))
             RuntimeError(request.status_code, "version number failed")
 
     def __str__(self):
-        return f"pyPreservica version: {pyPreservica.__version__}  (Preservica 6.6 Compatible) " \
+        return f"pyPreservica version: {pyPreservica.__version__}  (Preservica 6.9 Compatible) " \
                f"Connected to: {self.server} Preservica version: {self.version} as {self.username} " \
                f"in tenancy {self.tenant}"
 
     def __repr__(self):
         return self.__str__()
 
     def save_config(self):
```

### Comparing `pyPreservica-2.0.2/pyPreservica/contentAPI.py` & `pyPreservica-2.0.3/pyPreservica/contentAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.2/pyPreservica/entityAPI.py` & `pyPreservica-2.0.3/pyPreservica/entityAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.2/pyPreservica/monitorAPI.py` & `pyPreservica-2.0.3/pyPreservica/monitorAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.2/pyPreservica/opex.py` & `pyPreservica-2.0.3/pyPreservica/opex.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.2/pyPreservica/parAPI.py` & `pyPreservica-2.0.3/pyPreservica/parAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.2/pyPreservica/retentionAPI.py` & `pyPreservica-2.0.3/pyPreservica/retentionAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.2/pyPreservica/uploadAPI.py` & `pyPreservica-2.0.3/pyPreservica/uploadAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.2/pyPreservica/vocabularyAPI.py` & `pyPreservica-2.0.3/pyPreservica/authorityAPI.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 A client library for the Preservica Repository web services Webhook API
 https://us.preservica.com/api/reference-metadata/documentation.html
 
 author:     James Carr
 licence:    Apache License 2.0
 
 """
+import json
+import csv
+import requests
 
 from pyPreservica.common import *
 
 logger = logging.getLogger(__name__)
 
 BASE_ENDPOINT = '/api/reference-metadata'
 
@@ -30,34 +33,106 @@
                f"Name:\t\t\t{self.name}\n" \
                f"Security Tag:\t{self.security_tag}\n" \
                f"Display Field:\t\t\t{self.displayField}\n" \
                f"Metadata Connections:\t\t\t{self.metadataConnections}\n" \
                f"Fields:\t\t\t{self.fields}\n"
 
 
-class ControlledVocabularyAPI(AuthenticatedAPI):
+class AuthorityAPI(AuthenticatedAPI):
 
-
-    def load_skos(self, uri):
+    def delete_record(self, reference: str):
         """
-        Load a SKOS controlled vocabulary in skos RDF format
+          Delete a record from a table by its reference
+
+          :param reference:    The reference of the record to delete
+          :type: reference:    str
 
-        Simple Knowledge Organization System (SKOS)
+          """
+        headers = {HEADER_TOKEN: self.token, 'accept': 'application/json;charset=UTF-8'}
+        response = self.session.delete(f'{self.protocol}://{self.server}{BASE_ENDPOINT}/records/{reference}',
+                                       headers=headers)
+        if response.status_code == requests.codes.unauthorized:
+            self.token = self.__token__()
+            return self.delete_record(reference)
+        if response.status_code == requests.codes.no_content:
+            return
+        else:
+            exception = HTTPException("", response.status_code, response.url, "delete_record",
+                                      response.content.decode('utf-8'))
+            logger.error(exception)
+            raise exception
 
-        :param uri:
-        :return:
+    def add_records(self, table: Table, csv_file, encoding=None):
         """
-        pass
+         Add new records to an existing table from a CSV document
+
+         :param table:    The Table to add the record to
+         :type: table:    Table
 
-    def record(self, reference: str):
+         :param csv_file:    The path to the CSV document
+         :type: csv_file:    str
+
+         :param encoding:    The encoding used to open the csv document
+         :type: encoding:    str
+
+         """
+        with open(csv_file, newline='', encoding=encoding) as csvfile:
+            reader = csv.DictReader(csvfile)
+            for row in reader:
+                if ('ID' in row) or ('id' in row):
+                    pass
+                else:
+                    row['id'] = reader.line_num
+                self.add_record(table, row)
+
+    def add_record(self, table: Table, record: dict):
         """
-        Get individual record by its ref.
-        :param reference:
-        :return:
+         Add a new record to an existing table
+
+         :param table:    The Table to add the record to
+         :type: table:    Table
+
+         :param record:    The record
+         :type: record:    dict
+
+         :return: A single record
+         :rtype: dict
+
+         """
+        headers = {HEADER_TOKEN: self.token, 'accept': 'application/json;charset=UTF-8'}
+
+        body = {"securityDescriptor": "open", "fieldValues": []}
+        for key, val in record.items():
+            body["fieldValues"].append({"name": str(key).lower(), "value": val})
+
+        response = self.session.post(f'{self.protocol}://{self.server}{BASE_ENDPOINT}/tables/{table.reference}/records',
+                                     headers=headers, json=body)
+
+        if response.status_code == requests.codes.unauthorized:
+            self.token = self.__token__()
+            return self.add_record(table, record)
+        if response.status_code == requests.codes.created:
+            return str(response.content.decode('utf-8'))
+        else:
+            exception = HTTPException("", response.status_code, response.url, "add_record",
+                                      response.content.decode('utf-8'))
+            logger.error(exception)
+            raise exception
+
+    def record(self, reference: str) -> dict:
         """
+         Return a record by its reference
+
+         :param reference:    The record reference
+         :type: reference:    str
+
+         :return: A single record
+         :rtype: dict
+
+         """
         headers = {HEADER_TOKEN: self.token, 'accept': 'application/json;charset=UTF-8'}
         response = self.session.get(f'{self.protocol}://{self.server}{BASE_ENDPOINT}/records/{reference}',
                                     headers=headers)
         if response.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.record(reference)
         if response.status_code == requests.codes.ok:
@@ -65,40 +140,50 @@
             return json.loads(json_response)
         else:
             exception = HTTPException("", response.status_code, response.url, "record",
                                       response.content.decode('utf-8'))
             logger.error(exception)
             raise exception
 
-    def records(self, table: Table):
-        """
-        Get all records from a table.
-        :return:
+    def records(self, table: Table) -> list[dict]:
         """
+         Return all records from a table
+
+         :param table:    The authority table
+         :type: table:    Table
+
+         :return: List of records
+         :rtype: list[dict]
+
+         """
         headers = {HEADER_TOKEN: self.token, 'accept': 'application/json;charset=UTF-8'}
         response = self.session.get(f'{self.protocol}://{self.server}{BASE_ENDPOINT}/tables/{table.reference}/records',
-                                    headers=headers)
+                                    headers=headers, params={"expand": "true"})
         if response.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.records(table)
         if response.status_code == requests.codes.ok:
             json_response = str(response.content.decode('utf-8'))
             return json.loads(json_response)['records']
         else:
             exception = HTTPException("", response.status_code, response.url, "records",
                                       response.content.decode('utf-8'))
             logger.error(exception)
             raise exception
 
-    def table(self, reference: str):
+    def table(self, reference: str) -> Table:
         """
-        fetch a metadata table by id
+        fetch an authority table by its reference
+
+        :param reference:    The reference for the authority table
+        :type: reference:    str
+
+        :return: An authority table
+        :rtype: Table
 
-        :param reference:
-        :return:
         """
         headers = {HEADER_TOKEN: self.token, 'accept': 'application/json;charset=UTF-8'}
         response = self.session.get(f'{self.protocol}://{self.server}{BASE_ENDPOINT}/tables/{reference}',
                                     headers=headers)
         if response.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.table(reference)
@@ -111,18 +196,21 @@
             return table
         else:
             exception = HTTPException("", response.status_code, response.url, "table",
                                       response.content.decode('utf-8'))
             logger.error(exception)
             raise exception
 
-    def tables(self):
+    def tables(self) -> set[Table]:
         """
-        List reference metadata tables, optionally filtering by metadata connections.
-        :return:
+        List reference metadata tables
+
+        :return: Set of authority tables
+        :rtype: set(Table)
+
         """
         headers = {HEADER_TOKEN: self.token, 'accept': 'application/json;charset=UTF-8'}
         response = self.session.get(f'{self.protocol}://{self.server}{BASE_ENDPOINT}/tables', headers=headers)
         if response.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.tables()
         if response.status_code == requests.codes.ok:
```

### Comparing `pyPreservica-2.0.2/pyPreservica/webHooksAPI.py` & `pyPreservica-2.0.3/pyPreservica/webHooksAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.2/pyPreservica/workflowAPI.py` & `pyPreservica-2.0.3/pyPreservica/workflowAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.2/pyPreservica.egg-info/PKG-INFO` & `pyPreservica-2.0.3/pyPreservica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-2.0.2/pyPreservica.egg-info/SOURCES.txt` & `pyPreservica-2.0.3/pyPreservica.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 LICENSE.txt
 README.md
 setup.py
 pyPreservica/__init__.py
 pyPreservica/adminAPI.py
+pyPreservica/authorityAPI.py
 pyPreservica/common.py
 pyPreservica/contentAPI.py
 pyPreservica/entityAPI.py
 pyPreservica/monitorAPI.py
 pyPreservica/opex.py
 pyPreservica/parAPI.py
 pyPreservica/retentionAPI.py
 pyPreservica/uploadAPI.py
-pyPreservica/vocabularyAPI.py
 pyPreservica/webHooksAPI.py
 pyPreservica/workflowAPI.py
 pyPreservica.egg-info/PKG-INFO
 pyPreservica.egg-info/SOURCES.txt
 pyPreservica.egg-info/dependency_links.txt
 pyPreservica.egg-info/requires.txt
 pyPreservica.egg-info/top_level.txt
```

### Comparing `pyPreservica-2.0.2/setup.py` & `pyPreservica-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     os.system('twine upload dist/*')
     sys.exit()
 
 
 # This call to setup() does all the work
 setup(
     name=PKG,
-    version="2.0.2",
+    version="2.0.3",
     description="Python library for the Preservica API",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://pypreservica.readthedocs.io/",
     author="James Carr",
     author_email="drjamescarr@gmail.com",
     license="Apache License 2.0",
```

