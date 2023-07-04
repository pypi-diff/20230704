# Comparing `tmp/fast-webflow-0.4.1.tar.gz` & `tmp/fast-webflow-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-webflow-0.4.1.tar", last modified: Mon Jul  3 20:19:38 2023, max compression
+gzip compressed data, was "fast-webflow-0.5.0.tar", last modified: Tue Jul  4 20:34:29 2023, max compression
```

## Comparing `fast-webflow-0.4.1.tar` & `fast-webflow-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:19:38.331749 fast-webflow-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-03 20:19:38.331749 fast-webflow-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-03 20:19:38.331749 fast-webflow-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:19:38.327749 fast-webflow-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:19:38.331749 fast-webflow-0.4.1/src/fast_webflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-03 20:19:38.000000 fast-webflow-0.4.1/src/fast_webflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-03 20:19:38.000000 fast-webflow-0.4.1/src/fast_webflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:19:38.000000 fast-webflow-0.4.1/src/fast_webflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 20:19:38.000000 fast-webflow-0.4.1/src/fast_webflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:19:38.331749 fast-webflow-0.4.1/src/webflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/src/webflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:19:38.331749 fast-webflow-0.4.1/src/webflow/cms/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/src/webflow/cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/src/webflow/cms/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/src/webflow/cms/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/src/webflow/cms/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/src/webflow/cms/site.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/src/webflow/cms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:19:38.331749 fast-webflow-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:34:29.146427 fast-webflow-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-04 20:34:29.146427 fast-webflow-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-04 20:34:29.146427 fast-webflow-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:34:29.142427 fast-webflow-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:34:29.146427 fast-webflow-0.5.0/src/fast_webflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-04 20:34:29.000000 fast-webflow-0.5.0/src/fast_webflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-04 20:34:29.000000 fast-webflow-0.5.0/src/fast_webflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 20:34:29.000000 fast-webflow-0.5.0/src/fast_webflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 20:34:29.000000 fast-webflow-0.5.0/src/fast_webflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:34:29.146427 fast-webflow-0.5.0/src/webflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/src/webflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:34:29.146427 fast-webflow-0.5.0/src/webflow/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/src/webflow/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/src/webflow/cms/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/src/webflow/cms/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/src/webflow/cms/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/src/webflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/src/webflow/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/src/webflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:34:29.146427 fast-webflow-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/tests/test_authentication.py
```

### Comparing `fast-webflow-0.4.1/LICENSE` & `fast-webflow-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.4.1/PKG-INFO` & `fast-webflow-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-webflow
-Version: 0.4.1
+Version: 0.5.0
 Summary: A client library to communicate with the WebFlow API
 Home-page: https://github.com/tcilloni/fast-webflow
 Author: Thomas Cilloni
 Author-email: tcilloni@outlook.com
 Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fast-webflow-0.4.1/README.md` & `fast-webflow-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.4.1/setup.cfg` & `fast-webflow-0.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fast-webflow
-version = 0.4.1
+version = 0.5.0
 author = Thomas Cilloni
 author_email = tcilloni@outlook.com
 description = A client library to communicate with the WebFlow API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tcilloni/fast-webflow
 project_urls =
```

### Comparing `fast-webflow-0.4.1/src/fast_webflow.egg-info/PKG-INFO` & `fast-webflow-0.5.0/src/fast_webflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-webflow
-Version: 0.4.1
+Version: 0.5.0
 Summary: A client library to communicate with the WebFlow API
 Home-page: https://github.com/tcilloni/fast-webflow
 Author: Thomas Cilloni
 Author-email: tcilloni@outlook.com
 Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fast-webflow-0.4.1/src/webflow/cms/collection.py` & `fast-webflow-0.5.0/src/webflow/cms/collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,101 +1,77 @@
 import requests
 from collections import UserDict
 from functools import partial
 from itertools import repeat
 
-from .utils import string_to_dict, slugify, try_request, parallelize
-from .config import make_headers
+from ..utils import try_request, parallelize, parallelize_multiargs
+from ..config import make_headers
+from ..entity import Entity
 
 
-class Collection(UserDict):
+class Collection(Entity):
     """
     A Collection object connects with WebFlow's CMS API.
 
     Upon initialization, the object behaves like a dictionary, where its keys are the fields
     returned by the API's `get` method on the collection. The object allows getting, removing, and
     publishing lists of items concurrently.
     
     Attributes:
         id (str): ID field (often `_id`) of the collection in the CMS.
         delay (float): number of seconds to wait after a request hits the rate limit.
         max_retries (int): number of times failed requests are retried (including after hitting rate limits).
         data (dict): dictionary representation of the collection's data.
     """
 
-    def __init__(self, collection_id: str, max_retries: int = 50, throttle_delay: float = 10):
+    def __init__(self, id: str, *args, **kwargs):
         """
         Create a new Collection object.
 
         Args:
             collection_id (str): ID field (often `_id`) of the collection in the CMS.
             throttle_delay (float, optional): number of seconds to wait after a request hits the 
                 rate limit. Defaults to 10.
             max_retries (int, optional): number of times failed requests are retried (including 
                 after hitting rate limits). Defaults to 50.
         """
-        self.id = collection_id
-        self.delay = throttle_delay
-        self.max_retries = max_retries
-
-        self._url = f'https://api.webflow.com/collections/{collection_id}'
-        self._items_url = f'https://api.webflow.com/collections/{collection_id}/items?live="true"'
-        self._headers = make_headers()
+        super(Collection, self).__init__(id, *args, **kwargs)
+        self._url = f'https://api.webflow.com/collections/{id}'
+        self._items_url = f'https://api.webflow.com/collections/{id}/items'
         self._max_items_per_request = 100
         self.data = self.get_data()
     
 
     def get_data(self) -> dict[str, any]:
         '''
         Fetch the collection's information.
         See the `official documentation <https://developers.webflow.com/reference/get-collection>`__ 
         for more info. Upon being called, this method will also update the object's internal dictionary.
 
         Returns:
             dict[str, any]: information about this collection (name, slug, etc.).
         '''
-        self.data = self._request(requests.get, self._url)
-        return self.data
-    
-
-    def _request(self, request_fn: callable, url: str = None, data: dict = None) -> dict[str, any]:
-        '''
-        Default request method for the collection object.
+        return self._get()
 
-        Args:
-            request_fn (callable): function to call (one of requests.get/put/post/delete).
-            url (str, optional): specify to use a different URL than the default one. Defaults to `_items_url`.
-            data (dict, optional): optional JSON data to ship with the request. Defaults to None.
-
-        Returns:
-            dict[str, any]: whatever the response is, if valid, and always a dictionary.
-        '''
-        if url is None:
-            url = self._items_url
-        
-        return try_request(request_fn, url, self._headers, data, self.max_retries, self.delay)
-    
 
     def post_item(self, fields: dict[str,any], draft: bool = False) -> dict[str, any]:
         '''
         Add an item to the collection.
 
         Args:
             fields (dict[str,any]): item data (only fields' key:value pairs, not _archived and _draft)
             draft (bool, optional): draft the item or publish it directly. Defaults to False.
 
         Returns:
             dict[str, any]: if successful, information about the added item (including its slug).
         '''
         payload = {'fields': {'_archived': False, '_draft': draft}}
         payload['fields'].update(fields)
-
-        data = self._request(requests.post, self._items_url, payload)
         
-        return data
+        return self._post(self._items_url, payload)
     
 
     def post_items(self, fields_list: list[dict[str,any]], draft: bool = False) -> list[dict[str, any]]:
         '''
         Add multiple items to the collection.
         This method is a wrapper for multiple `post_item` method calls in parallel. Refer to that
         for more information.
@@ -130,16 +106,16 @@
         data = {}
 
         # split IDs into lists of max 100 items
         item_ids = [item_ids[i:i+max_items] for i in range(0, len(item_ids), max_items)]
         payloads = [{"itemIds": ids} for ids in item_ids]
 
         # send parallel requests
-        parallel_arguments = zip(repeat(url), payloads)
-        returns  = parallelize(lambda args: requests.put(*args), parallel_arguments)
+        urls_and_data = zip(repeat(url), payloads)
+        returns  = parallelize_multiargs(self._put, urls_and_data)
 
         # merge responses
         for key in ['publishedItemIds', 'errors']:
             data[key] = [item for resp in returns for item in resp[key]]
         
         return data
     
@@ -160,16 +136,16 @@
         data = {}
 
         # split IDs into lists of max 100 items
         item_ids = [item_ids[i:i+max_items] for i in range(0, len(item_ids), max_items)]
         payloads = [{"itemIds": ids} for ids in item_ids]
 
         # send parallel requests
-        delete_fn = lambda data : self._request(requests.delete, self._items_url, data)
-        returns  = parallelize(delete_fn, payloads)
+        urls_and_data = zip(repeat(self._items_url), payloads)
+        returns = parallelize_multiargs(self._delete, urls_and_data)
 
         # merge responses
         for key in ['deletedItemIds', 'errors']:
             data[key] = [item for resp in returns for item in resp[key]]
 
         return data
     
@@ -184,17 +160,16 @@
             offset (int, optional): number of items to skip. Defaults to 0.
             limit (int, optional): max number of items to return (capped at 100). Defaults to 100.
 
         Returns:
             dict[str, any]: group of items (index with the key `items` to get the actual data).
         '''
         url = self._items_url + f"&offset={offset}&limit={limit}"
-        data = self._request(requests.get, url)
-        
-        return data
+
+        return self._get(url)
     
 
     def get_all_items(self) -> list[dict]:
         '''
         Fetch all items in this collection.
         This is a convenient wrapper around the `get_items` method to automatically control pagination
         and fetch all items in parallel. Note that the method first sends a get request to get the 
@@ -202,15 +177,15 @@
         of pages and send the requests.
 
         Returns:
             list[dict]: list of each item's data.
         '''
         # update total number of items
         max_items = self._max_items_per_request  # API rule
-        initial_data = self._request(requests.get, self._items_url)
+        initial_data = self._get(self._items_url)
         total = initial_data['total']
 
         # prepare one URL request for each offset in 0..total..limit
         item_lists = parallelize(self.get_items, range(0, total, max_items))
         all_items = [item for item_list in item_lists for item in item_list['items']]
         
         return all_items
```

### Comparing `fast-webflow-0.4.1/src/webflow/cms/config.py` & `fast-webflow-0.5.0/src/webflow/config.py`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.4.1/src/webflow/cms/site.py` & `fast-webflow-0.5.0/src/webflow/cms/site.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,113 +1,87 @@
 import requests
 from collections import UserDict
 
-from .utils import string_to_dict, slugify, try_request
-from .config import make_headers
+from ..entity import Entity
+from ..utils import try_request
 
 
 def list_sites():
-    data = try_request(requests.get, 'https://api.webflow.com/sites', make_headers())
-    return data
+    return Entity(None)._get('https://api.webflow.com/sites')
 
 
-class Site(UserDict):
+class Site(Entity):
     """
     A Site object connects with WebFlow's General API.
 
     Upon initialization, the object behaves like a dictionary, where its keys are the fields
     returned by the API's `get` method on the site. The object allows all operations that the API
     allows for sites.
     
     Attributes:
         id (str): ID field (often `_id`) of the site in the CMS.
         delay (float): number of seconds to wait after a request hits the rate limit.
         max_retries (int): number of times failed requests are retried (including after hitting rate limits).
         data (dict): dictionary representation of the site's data.
     """
 
-    def __init__(self, site_id: str, max_retries: int = 50, throttle_delay: int = 10):
+    def __init__(self, id: str, *args, **kwargs):
         '''
         Create a new Site object.
 
         Args:
             site_id (str): ID field (often `_id`) of the site in the CMS.
             throttle_delay (float, optional): number of seconds to wait after a request hits the 
                 rate limit. Defaults to 10.
             max_retries (int, optional): number of times failed requests are retried (including 
                 after hitting rate limits). Defaults to 50.
         '''
-        self.id = site_id
-        self.delay = throttle_delay
-        self.max_retries = max_retries
-
-        self._url = f'https://api.webflow.com/sites/{site_id}'
-        self._headers = make_headers()
+        super(Site, self).__init__(id, *args, **kwargs)
+        self._url = f'https://api.webflow.com/sites/{id}'
         self.data = self.get_data()
     
 
     def get_data(self) -> dict[str, any]:
         '''
         Fetch the site's information.
         See the `official documentation <https://developers.webflow.com/reference/get-site>`__ 
         for more info. Upon being called, this method will also update the object's internal dictionary.
 
         Returns:
             dict[str, any]: information about this site (name, domains, etc.).
         '''
-        return self._request(requests.get)
-
-
-    def _request(self, request_fn: callable, url: str = None, data: dict = None) -> dict[str, any]:
-        '''
-        Default request method for the site object.
-
-        Args:
-            request_fn (callable): function to call (one of requests.get/put/post/delete).
-            url (str, optional): specify to use a different URL than the default one. Defaults to `_url`.
-            data (dict, optional): optional JSON data to ship with the request. Defaults to None.
+        return self._get()
 
-        Returns:
-            dict[str, any]: whatever the response is, if valid, and always a dictionary.
-        '''
-        if url is None:
-            url = self._url
-        
-        return try_request(request_fn, url, self._headers, data, self.max_retries, self.delay)
-    
 
     def publish(self, domains: list[str] = None) -> dict[str, bool]:
         '''
         Publish the website to any domain(s).
         By default, the website is published to all associated domains.
 
         Args:
             domains (list[str], optional): domain URLs to publish to. Defaults to All.
 
         Returns:
             dict[str, bool]: `{'queued': True}` if successful, `{'queued': False}` otherwise
         '''
-        # `queued`
-        if not domains:
-            domains = [domain['name'] for domain in self.get_domains()]
-
-        return self._request(requests.post, self._url + '/publish', {"domains": domains})
+        domains = domains or [domain['name'] for domain in self.get_domains()]
+        return self._post(self._url + '/publish', {"domains": domains})
     
 
     def get_domains(self) -> list[dict[str, str]]:
         '''
         Get a list of domains the site can be published to.
 
         Returns:
             list[dict[str, str]]: list of `{'id': id, 'name': name}` dictionaries.
         '''
-        return self._request(requests.get, self._url + '/domains')
+        return self._get(self._url + '/domains')
 
 
     def get_collections(self) -> list[dict[str, any]]:
         '''
         List the collections in the site's CMS.
 
         Returns:
             list[dict[str, any]]: list of collections with some basic data.
         '''
-        return self._request(requests.get, self._url + '/collections')
+        return self._get(self._url + '/collections')
```

### Comparing `fast-webflow-0.4.1/src/webflow/cms/utils.py` & `fast-webflow-0.5.0/src/webflow/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,18 @@
     '''
     executor = ThreadPoolExecutor(max_workers = threads)
     futures = executor.map(function, data)
     results = list(futures) if await_completion else futures
     return results
 
 
+def parallelize_multiargs(function: callable, data: list[any], threads: int = 50, await_completion: bool = True) -> list[any]:
+    return parallelize(lambda args: function(*args), data, threads, await_completion)
+
+
 def try_request(request_fn: callable, url: str, headers: dict[str, str], data: dict = None, 
         max_retries: int = 50, delay: float = 10) -> dict:
     '''
     Execute a request to the WebFlow API with implicit Rate Limit handling.
 
     Args:
         request_fn (callable): prepared requests function to execute.
```

