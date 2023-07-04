# Comparing `tmp/elimity-insights-client-9.0.0b1.tar.gz` & `tmp/elimity-insights-client-9.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elimity-insights-client-9.0.0b1.tar", max compression
+gzip compressed data, was "elimity-insights-client-9.0.0b2.tar", max compression
```

## Comparing `elimity-insights-client-9.0.0b1.tar` & `elimity-insights-client-9.0.0b2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11338 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/LICENSE.txt
--rw-r--r--   0        0        0     2006 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/README.md
--rw-r--r--   0        0        0      928 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     1116 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/__init__.py
--rw-r--r--   0        0        0     3378 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/_decode_domain_graph_schema.py
--rw-r--r--   0        0        0     1121 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/_domain_graph_schema.py
--rw-r--r--   0        0        0     8683 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/_elimity_insights_client.py
--rw-r--r--   0        0        0      741 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/_util.py
--rw-r--r--   0        0        0      162 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/__init__.py
--rw-r--r--   0        0        0     1990 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/_api.py
--rw-r--r--   0        0        0     3370 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/_decode_query_results_page.py
--rw-r--r--   0        0        0     1367 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/_decode_source.py
--rw-r--r--   0        0        0    13483 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/_encode_expression.py
--rw-r--r--   0        0        0     5902 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/_encode_query.py
--rw-r--r--   0        0        0      180 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/entities/__init__.py
--rw-r--r--   0        0        0     1031 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/entities/_entities.py
--rw-r--r--   0        0        0      512 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/entities/_entity.py
--rw-r--r--   0        0        0     2527 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/entities/_parse_query_results_page.py
--rw-r--r--   0        0        0     3856 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/entities/_query.py
--rw-r--r--   0        0        0      521 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/entities/_schema.py
--rw-r--r--   0        0        0     9303 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/expression.py
--rw-r--r--   0        0        0     3528 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/query.py
--rw-r--r--   0        0        0     1678 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/query_results_page.py
--rw-r--r--   0        0        0      801 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/source.py
--rw-r--r--   0        0        0        0 2022-10-18 15:07:24.816597 elimity-insights-client-9.0.0b1/src/elimity_insights_client/py.typed
--rw-r--r--   0        0        0     3089 1970-01-01 00:00:00.000000 elimity-insights-client-9.0.0b1/setup.py
--rw-r--r--   0        0        0     2991 1970-01-01 00:00:00.000000 elimity-insights-client-9.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0    11338 2022-10-21 14:47:45.634588 elimity-insights-client-9.0.0b2/LICENSE.txt
+-rw-r--r--   0        0        0     2006 2022-10-21 14:47:45.634588 elimity-insights-client-9.0.0b2/README.md
+-rw-r--r--   0        0        0      928 2022-10-21 14:47:45.634588 elimity-insights-client-9.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     1116 2022-10-21 14:47:45.634588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/__init__.py
+-rw-r--r--   0        0        0     3378 2022-10-21 14:47:45.634588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/_decode_domain_graph_schema.py
+-rw-r--r--   0        0        0     1121 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/_domain_graph_schema.py
+-rw-r--r--   0        0        0     8683 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/_elimity_insights_client.py
+-rw-r--r--   0        0        0      741 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/_util.py
+-rw-r--r--   0        0        0      162 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/__init__.py
+-rw-r--r--   0        0        0     1990 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/_api.py
+-rw-r--r--   0        0        0     3402 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/_decode_query_results_page.py
+-rw-r--r--   0        0        0     1367 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/_decode_source.py
+-rw-r--r--   0        0        0    13483 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/_encode_expression.py
+-rw-r--r--   0        0        0     5902 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/_encode_query.py
+-rw-r--r--   0        0        0      180 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/entities/__init__.py
+-rw-r--r--   0        0        0     1031 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/entities/_entities.py
+-rw-r--r--   0        0        0      512 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/entities/_entity.py
+-rw-r--r--   0        0        0     2527 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/entities/_parse_query_results_page.py
+-rw-r--r--   0        0        0     3856 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/entities/_query.py
+-rw-r--r--   0        0        0      521 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/entities/_schema.py
+-rw-r--r--   0        0        0     9303 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/expression.py
+-rw-r--r--   0        0        0     3528 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/query.py
+-rw-r--r--   0        0        0     1678 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/query_results_page.py
+-rw-r--r--   0        0        0      801 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/source.py
+-rw-r--r--   0        0        0        0 2022-10-21 14:47:45.638588 elimity-insights-client-9.0.0b2/src/elimity_insights_client/py.typed
+-rw-r--r--   0        0        0     3089 1970-01-01 00:00:00.000000 elimity-insights-client-9.0.0b2/setup.py
+-rw-r--r--   0        0        0     2991 1970-01-01 00:00:00.000000 elimity-insights-client-9.0.0b2/PKG-INFO
```

### Comparing `elimity-insights-client-9.0.0b1/LICENSE.txt` & `elimity-insights-client-9.0.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/README.md` & `elimity-insights-client-9.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/pyproject.toml` & `elimity-insights-client-9.0.0b2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry]
 authors = ["Elimity development team <dev@elimity.com>"]
 description = "Client for connector interactions with an Elimity Insights server"
 license = "Apache-2.0"
 name = "elimity-insights-client"
 readme = "README.md"
 repository = "https://github.com/elimity-com/insights-client-python"
-version = "9.0.0b1"
+version = "9.0.0b2"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 python-dateutil = "^2.8.2"
 requests = "^2.28.1"
 simplejson = "^3.17.6"
 typing-extensions = "^4.3.0"
```

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/__init__.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/__init__.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/_decode_domain_graph_schema.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/_decode_domain_graph_schema.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/_domain_graph_schema.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/_domain_graph_schema.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/_elimity_insights_client.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/_elimity_insights_client.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/_util.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/_util.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/_api.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/_api.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/_decode_query_results_page.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/_decode_query_results_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from datetime import date, time
+from datetime import date
 from json import loads
 from typing import List
 
-from dateutil.parser import isoparse
+from dateutil.parser import isoparse, isoparser
 from typing_extensions import TypedDict
 
 from elimity_insights_client._util import map_list
 from elimity_insights_client.api.query_results_page import (
     BooleanValue,
     DateTimeValue,
     DateValue,
@@ -115,9 +115,10 @@
     if type == "number":
         number_value = loads(value)
         return NumberValue(number_value)
 
     if type == "string":
         return StringValue(value)
 
-    time_value = time.fromisoformat(value)
+    parser = isoparser()
+    time_value = parser.parse_isotime(value)
     return TimeValue(time_value)
```

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/_decode_source.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/_decode_source.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/_encode_expression.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/_encode_expression.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/_encode_query.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/_encode_query.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/entities/_entities.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/entities/_entities.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/entities/_entity.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/entities/_entity.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/entities/_parse_query_results_page.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/entities/_parse_query_results_page.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/entities/_query.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/entities/_query.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/entities/_schema.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/entities/_schema.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/expression.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/expression.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/query.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/query.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/query_results_page.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/query_results_page.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/src/elimity_insights_client/api/source.py` & `elimity-insights-client-9.0.0b2/src/elimity_insights_client/api/source.py`

 * *Files identical despite different names*

### Comparing `elimity-insights-client-9.0.0b1/setup.py` & `elimity-insights-client-9.0.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'python-dateutil>=2.8.2,<3.0.0',
  'requests>=2.28.1,<3.0.0',
  'simplejson>=3.17.6,<4.0.0',
  'typing-extensions>=4.3.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'elimity-insights-client',
-    'version': '9.0.0b1',
+    'version': '9.0.0b2',
     'description': 'Client for connector interactions with an Elimity Insights server',
     'long_description': '# Elimity Insights Python client\n\nThis Python module provides a client for connector interactions with an Elimity\nInsights server.\n\n## Usage\n\n### Importing data to custom sources\n\nThe following snippet shows how to authenticate as a custom source and create a connector log at an Elimity Insights\nserver. You can generate a source identifier and token by visiting the custom source\'s detail page in Elimity Insights\nand clicking the \'GENERATE CREDENTIALS\' button, which can be found under the \'SETTINGS\' tab.\n\n```python3\nfrom datetime import datetime\n\nfrom elimity_insights_client import Client, Config, ConnectorLog, Level\n\nif __name__ == "__main__":\n    config = Config(id=1, url="https://local.elimity.com:8081", token="token")\n    client = Client(config)\n\n    timestamp = datetime.now()\n    log = ConnectorLog(level=Level.INFO, message="Hello world!", timestamp=timestamp)\n    logs = [log]\n    client.create_connector_logs(logs)\n```\n\n### Other API interactions\n\nThis module also provides a client for other API interactions with Elimity Insights. The snippet below shows how to\nauthenticate with an API token and list sources at an Elimity Insights server. You can generate a token identifier and\nsecret by visiting the \'API tokens\' page in Elimity Insights and clicking the \'CREATE API TOKEN\' button.\n\n```python3\nfrom elimity_insights_client.api import Config, sources\n\nif __name__ == "__main__":\n    config = Config(token_id="1", token_secret="my-secret-value", url="https://example.elimity.com", verify_ssl=True)\n    my_sources = sources(config)\n    print(my_sources)\n```\n\n## Installation\n\n```sh\n$ pip install elimity-insights-client\n```\n\n## Compatibility\n\n| Client version | Insights version |\n| -------------- | ---------------- |\n| 1              | 2.8 - 2.10       |\n| 2 - 3          | 2.11 - 3.0       |\n| 4              | 3.1 - 3.3        |\n| 5 - 6          | 3.4 - 3.5        |\n| 7              | 3.6 - 3.7        |\n| 8              | 3.8 - 3.15       |\n| 9              | ^3.16            |\n',
     'author': 'Elimity development team',
     'author_email': 'dev@elimity.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/elimity-com/insights-client-python',
```

### Comparing `elimity-insights-client-9.0.0b1/PKG-INFO` & `elimity-insights-client-9.0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elimity-insights-client
-Version: 9.0.0b1
+Version: 9.0.0b2
 Summary: Client for connector interactions with an Elimity Insights server
 Home-page: https://github.com/elimity-com/insights-client-python
 License: Apache-2.0
 Author: Elimity development team
 Author-email: dev@elimity.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

