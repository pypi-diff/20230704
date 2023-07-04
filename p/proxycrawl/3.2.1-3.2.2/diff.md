# Comparing `tmp/proxycrawl-3.2.1.tar.gz` & `tmp/proxycrawl-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxycrawl-3.2.1.tar", last modified: Tue Sep 14 13:39:38 2021, max compression
+gzip compressed data, was "dist/proxycrawl-3.2.2.tar", last modified: Tue Jul  4 13:49:02 2023, max compression
```

## Comparing `proxycrawl-3.2.1.tar` & `proxycrawl-3.2.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 adria      (501) staff       (20)        0 2021-09-14 13:39:38.088285 proxycrawl-3.2.1/
--rw-r--r--   0 adria      (501) staff       (20)    11357 2018-05-31 08:04:47.000000 proxycrawl-3.2.1/LICENSE
--rw-r--r--   0 adria      (501) staff       (20)     9103 2021-09-14 13:39:38.087808 proxycrawl-3.2.1/PKG-INFO
--rw-r--r--   0 adria      (501) staff       (20)     8202 2021-09-10 14:47:07.000000 proxycrawl-3.2.1/README.md
-drwxr-xr-x   0 adria      (501) staff       (20)        0 2021-09-14 13:39:38.085538 proxycrawl-3.2.1/proxycrawl/
--rw-r--r--   0 adria      (501) staff       (20)      314 2021-09-10 14:47:07.000000 proxycrawl-3.2.1/proxycrawl/__init__.py
--rw-r--r--   0 adria      (501) staff       (20)     4267 2021-09-14 13:37:43.000000 proxycrawl-3.2.1/proxycrawl/base_api.py
--rw-r--r--   0 adria      (501) staff       (20)      796 2020-12-19 08:10:02.000000 proxycrawl-3.2.1/proxycrawl/crawling_api.py
--rw-r--r--   0 adria      (501) staff       (20)      437 2020-12-19 08:59:26.000000 proxycrawl-3.2.1/proxycrawl/leads_api.py
--rw-r--r--   0 adria      (501) staff       (20)      171 2020-12-19 05:24:26.000000 proxycrawl-3.2.1/proxycrawl/proxycrawl_api.py
--rw-r--r--   0 adria      (501) staff       (20)      525 2020-12-19 08:10:22.000000 proxycrawl-3.2.1/proxycrawl/scraper_api.py
--rw-r--r--   0 adria      (501) staff       (20)     1562 2021-09-14 13:37:43.000000 proxycrawl-3.2.1/proxycrawl/screenshots_api.py
--rw-r--r--   0 adria      (501) staff       (20)     2768 2021-09-14 13:37:43.000000 proxycrawl-3.2.1/proxycrawl/storage_api.py
-drwxr-xr-x   0 adria      (501) staff       (20)        0 2021-09-14 13:39:38.087071 proxycrawl-3.2.1/proxycrawl.egg-info/
--rw-r--r--   0 adria      (501) staff       (20)     9103 2021-09-14 13:39:38.000000 proxycrawl-3.2.1/proxycrawl.egg-info/PKG-INFO
--rw-r--r--   0 adria      (501) staff       (20)      370 2021-09-14 13:39:38.000000 proxycrawl-3.2.1/proxycrawl.egg-info/SOURCES.txt
--rw-r--r--   0 adria      (501) staff       (20)        1 2021-09-14 13:39:38.000000 proxycrawl-3.2.1/proxycrawl.egg-info/dependency_links.txt
--rw-r--r--   0 adria      (501) staff       (20)       11 2021-09-14 13:39:38.000000 proxycrawl-3.2.1/proxycrawl.egg-info/top_level.txt
--rw-r--r--   0 adria      (501) staff       (20)       38 2021-09-14 13:39:38.088374 proxycrawl-3.2.1/setup.cfg
--rw-r--r--   0 adria      (501) staff       (20)     1255 2021-09-14 13:38:42.000000 proxycrawl-3.2.1/setup.py
+drwxr-xr-x   0 jamal      (501) staff       (20)        0 2023-07-04 13:49:02.000000 proxycrawl-3.2.2/
+-rw-r--r--   0 jamal      (501) staff       (20)    11638 2023-07-04 13:49:02.000000 proxycrawl-3.2.2/PKG-INFO
+drwxr-xr-x   0 jamal      (501) staff       (20)        0 2023-07-04 13:49:02.000000 proxycrawl-3.2.2/proxycrawl/
+-rw-r--r--   0 jamal      (501) staff       (20)     4267 2022-01-05 11:08:04.000000 proxycrawl-3.2.2/proxycrawl/base_api.py
+-rw-r--r--   0 jamal      (501) staff       (20)      796 2022-01-05 11:08:04.000000 proxycrawl-3.2.2/proxycrawl/crawling_api.py
+-rw-r--r--   0 jamal      (501) staff       (20)      908 2023-07-04 13:46:03.000000 proxycrawl-3.2.2/proxycrawl/__init__.py
+-rw-r--r--   0 jamal      (501) staff       (20)      437 2022-01-05 11:08:04.000000 proxycrawl-3.2.2/proxycrawl/leads_api.py
+-rw-r--r--   0 jamal      (501) staff       (20)      525 2022-01-05 11:08:04.000000 proxycrawl-3.2.2/proxycrawl/scraper_api.py
+-rw-r--r--   0 jamal      (501) staff       (20)      171 2022-01-05 11:08:04.000000 proxycrawl-3.2.2/proxycrawl/proxycrawl_api.py
+-rw-r--r--   0 jamal      (501) staff       (20)     2768 2022-01-05 11:08:04.000000 proxycrawl-3.2.2/proxycrawl/storage_api.py
+-rw-r--r--   0 jamal      (501) staff       (20)     1562 2022-01-05 11:08:04.000000 proxycrawl-3.2.2/proxycrawl/screenshots_api.py
+-rw-r--r--   0 jamal      (501) staff       (20)     8436 2023-07-04 13:33:19.000000 proxycrawl-3.2.2/README.md
+drwxr-xr-x   0 jamal      (501) staff       (20)        0 2023-07-04 13:49:02.000000 proxycrawl-3.2.2/proxycrawl.egg-info/
+-rw-r--r--   0 jamal      (501) staff       (20)    11638 2023-07-04 13:49:02.000000 proxycrawl-3.2.2/proxycrawl.egg-info/PKG-INFO
+-rw-r--r--   0 jamal      (501) staff       (20)      362 2023-07-04 13:49:02.000000 proxycrawl-3.2.2/proxycrawl.egg-info/SOURCES.txt
+-rw-r--r--   0 jamal      (501) staff       (20)       11 2023-07-04 13:49:02.000000 proxycrawl-3.2.2/proxycrawl.egg-info/top_level.txt
+-rw-r--r--   0 jamal      (501) staff       (20)        1 2023-07-04 13:49:02.000000 proxycrawl-3.2.2/proxycrawl.egg-info/dependency_links.txt
+-rw-r--r--   0 jamal      (501) staff       (20)     1255 2023-07-04 13:46:48.000000 proxycrawl-3.2.2/setup.py
+-rw-r--r--   0 jamal      (501) staff       (20)       38 2023-07-04 13:49:02.000000 proxycrawl-3.2.2/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `proxycrawl-3.2.1/PKG-INFO` & `proxycrawl-3.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-Metadata-Version: 2.1
-Name: proxycrawl
-Version: 3.2.1
-Summary: A Python class that acts as wrapper for ProxyCrawl scraping and crawling API
-Home-page: https://github.com/proxycrawl/proxycrawl-python
-Author: ProxyCrawl
-Author-email: info@proxycrawl.com
-License: Apache-2.0
-Keywords: scraping scraper crawler crawling proxycrawl api
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# DEPRECATION NOTICE
+
+> :warning: **IMPORTANT:** This package is no longer maintained or supported. For the latest updates, please use our new package at [crawlbase-python](https://github.com/crawlbase-source/crawlbase-python).
+
+---
 
 # ProxyCrawl API Python class
 
 A lightweight, dependency free Python class that acts as wrapper for ProxyCrawl API.
 
 ## Installing
 
@@ -299,10 +282,8 @@
 api = CrawlingAPI({ 'token': 'TOKEN', 'timeout': 120 })
 ```
 
 Timeout is in seconds.
 
 ---
 
-Copyright 2021 ProxyCrawl
-
-
+Copyright 2023 ProxyCrawl
```

### Comparing `proxycrawl-3.2.1/README.md` & `proxycrawl-3.2.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,283 +1,311 @@
-# ProxyCrawl API Python class
-
-A lightweight, dependency free Python class that acts as wrapper for ProxyCrawl API.
-
-## Installing
-
-Choose a way of installing:
-
-- Download the python class from Github.
-- Or use [PyPi](https://pypi.org/project/proxycrawl/) Python package manager. `pip install proxycrawl`
-
-Then import the CrawlingAPI, ScraperAPI, etc as needed.
-
-```python
-from proxycrawl import CrawlingAPI, ScraperAPI, LeadsAPI, ScreenshotsAPI, StorageAPI
-```
-
-### Upgrading to version 3
-
-Version 3 deprecates the usage of ProxyCrawlAPI in favour of CrawlingAPI (although is still usable). Please test the upgrade before deploying to production.
-
-## Crawling API
-
-First initialize the CrawlingAPI class.
-
-```python
-api = CrawlingAPI({ 'token': 'YOUR_PROXYCRAWL_TOKEN' })
-```
-
-### GET requests
-
-Pass the url that you want to scrape plus any options from the ones available in the [API documentation](https://proxycrawl.com/docs).
-
-```python
-api.get(url, options = {})
-```
-
-Example:
-
-```python
-response = api.get('https://www.facebook.com/britneyspears')
-if response['status_code'] == 200:
-    print(response['body'])
-```
-
-You can pass any options from ProxyCrawl API.
-
-Example:
-
-```python
-response = api.get('https://www.reddit.com/r/pics/comments/5bx4bx/thanks_obama/', {
-    'user_agent': 'Mozilla/5.0 (Windows NT 6.2; rv:20.0) Gecko/20121202 Firefox/30.0',
-    'format': 'json'
-})
-if response['status_code'] == 200:
-    print(response['body'])
-```
-
-### POST requests
-
-Pass the url that you want to scrape, the data that you want to send which can be either a json or a string, plus any options from the ones available in the [API documentation](https://proxycrawl.com/docs).
-
-```python
-api.post(url, dictionary or string data, options = {})
-```
-
-Example:
-
-```python
-response = api.post('https://producthunt.com/search', { 'text': 'example search' })
-if response['status_code'] == 200:
-    print(response['body'])
-```
-
-You can send the data as `application/json` instead of `x-www-form-urlencoded` by setting option `post_content_type` as json.
-
-```python
-import json
-response = api.post('https://httpbin.org/post', json.dumps({ 'some_json': 'with some value' }), { 'post_content_type': 'json' })
-if response['status_code'] == 200:
-    print(response['body'])
-```
-
-### Javascript requests
-
-If you need to scrape any website built with Javascript like React, Angular, Vue, etc. You just need to pass your javascript token and use the same calls. Note that only `.get` is available for javascript and not `.post`.
-
-```python
-api = CrawlingAPI({ 'token': 'YOUR_JAVASCRIPT_TOKEN' })
-```
-
-```python
-response = api.get('https://www.nfl.com')
-if response['status_code'] == 200:
-    print(response['body'])
-```
-
-Same way you can pass javascript additional options.
-
-```python
-response = api.get('https://www.freelancer.com', { 'page_wait': 5000 })
-if response['status_code'] == 200:
-    print(response['body'])
-```
-
-## Original status
-
-You can always get the original status and proxycrawl status from the response. Read the [ProxyCrawl documentation](https://proxycrawl.com/docs) to learn more about those status.
-
-```python
-response = api.get('https://craiglist.com')
-print(response['headers']['original_status'])
-print(response['headers']['pc_status'])
-```
-
-If you have questions or need help using the library, please open an issue or [contact us](https://proxycrawl.com/contact).
-
-## Scraper API
-
-The usage of the Scraper API is very similar, just change the class name to initialize.
-
-```python
-scraper_api = ScraperAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
-
-response = scraper_api.get('https://www.amazon.com/DualSense-Wireless-Controller-PlayStation-5/dp/B08FC6C75Y/')
-if response['status_code'] == 200:
-    print(response['json']['name']) # Will print the name of the Amazon product
-```
-
-## Leads API
-
-To find email leads you can use the leads API, you can check the full [API documentation](https://proxycrawl.com/docs/leads-api/) if needed.
-
-```python
-leads_api = LeadsAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
-
-response = leads_api.get_from_domain('microsoft.com')
-
-if response['status_code'] == 200:
-    print(response['json']['leads'])
-```
-
-## Screenshots API
-
-Initialize with your Screenshots API token and call the `get` method.
-
-```python
-screenshots_api = ScreenshotsAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
-response = screenshots_api.get('https://www.apple.com')
-if response['status_code'] == 200:
-    print(response['headers']['success'])
-    print(response['headers']['url'])
-    print(response['headers']['remaining_requests'])
-    print(response['file'])
-```
-
-or specifying a file path
-
-```python
-screenshots_api = ScreenshotsAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
-response = screenshots_api.get('https://www.apple.com', { 'save_to_path': 'apple.jpg' })
-if response['status_code'] == 200:
-    print(response['headers']['success'])
-    print(response['headers']['url'])
-    print(response['headers']['remaining_requests'])
-    print(response['file'])
-```
-
-or if you set `store=true` then `screenshot_url` is set in the returned headers 
-
-```python
-screenshots_api = ScreenshotsAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
-response = screenshots_api.get('https://www.apple.com', { 'store': 'true' })
-if response['status_code'] == 200:
-    print(response['headers']['success'])
-    print(response['headers']['url'])
-    print(response['headers']['remaining_requests'])
-    print(response['file'])
-    print(response['headers']['screenshot_url'])
-```
-
-Note that `screenshots_api.get(url, options)` method accepts an [options](https://proxycrawl.com/docs/screenshots-api/parameters)
-
-## Storage API
-
-Initialize the Storage API using your private token.
-
-```python
-storage_api = StorageAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
-```
-
-Pass the [url](https://proxycrawl.com/docs/storage-api/parameters/#url) that you want to get from [Proxycrawl Storage](https://proxycrawl.com/dashboard/storage).
-
-```python
-response = storage_api.get('https://www.apple.com')
-if response['status_code'] == 200:
-    print(response['headers']['original_status'])
-    print(response['headers']['pc_status'])
-    print(response['headers']['url'])
-    print(response['headers']['rid'])
-    print(response['headers']['stored_at'])
-    print(response['body'])
-```
-
-or you can use the [RID](https://proxycrawl.com/docs/storage-api/parameters/#rid)
-
-```python
-response = storage_api.get('RID_REPLACE')
-if response['status_code'] == 200:
-    print(response['headers']['original_status'])
-    print(response['headers']['pc_status'])
-    print(response['headers']['url'])
-    print(response['headers']['rid'])
-    print(response['headers']['stored_at'])
-    print(response['body'])
-```
-
-Note: One of the two RID or URL must be sent. So both are optional but it's mandatory to send one of the two.
-
-### [Delete](https://proxycrawl.com/docs/storage-api/delete/) request
-
-To delete a storage item from your storage area, use the correct RID
-
-```python
-if storage_api.delete('RID_REPLACE'):
-  print('delete success')
-else:
-  print('Unable to delete')
-```
-
-### [Bulk](https://proxycrawl.com/docs/storage-api/bulk/) request
-
-To do a bulk request with a list of RIDs, please send the list of rids as an array
-
-```python
-response = storage_api.bulk(['RID1', 'RID2', 'RID3', ...])
-if response['status_code'] == 200:
-    for item in response['json']:
-        print(item['original_status'])
-        print(item['pc_status'])
-        print(item['url'])
-        print(item['rid'])
-        print(item['stored_at'])
-        print(item['body'])
-```
-
-### [RIDs](https://proxycrawl.com/docs/storage-api/rids) request
-
-To request a bulk list of RIDs from your storage area
-
-```python
-rids = storage_api.rids()
-print(rids)
-```
-
-You can also specify a limit as a parameter
-
-```python
-storage_api.rids(100)
-```
-
-### [Total Count](https://proxycrawl.com/docs/storage-api/total_count)
-
-To get the total number of documents in your storage area
-
-```python
-total_count = storage_api.totalCount()
-print(total_count)
-```
-
-## Custom timeout
-
-If you need to use a custom timeout, you can pass it to the class instance creation like the following:
-
-```python
-api = CrawlingAPI({ 'token': 'TOKEN', 'timeout': 120 })
-```
-
-Timeout is in seconds.
-
----
-
-Copyright 2021 ProxyCrawl
+Metadata-Version: 2.1
+Name: proxycrawl
+Version: 3.2.2
+Summary: A Python class that acts as wrapper for ProxyCrawl scraping and crawling API
+Home-page: https://github.com/proxycrawl/proxycrawl-python
+Author: ProxyCrawl
+Author-email: info@proxycrawl.com
+License: Apache-2.0
+Description: # DEPRECATION NOTICE
+        
+        > :warning: **IMPORTANT:** This package is no longer maintained or supported. For the latest updates, please use our new package at [crawlbase-python](https://github.com/crawlbase-source/crawlbase-python).
+        
+        ---
+        
+        # ProxyCrawl API Python class
+        
+        A lightweight, dependency free Python class that acts as wrapper for ProxyCrawl API.
+        
+        ## Installing
+        
+        Choose a way of installing:
+        
+        - Download the python class from Github.
+        - Or use [PyPi](https://pypi.org/project/proxycrawl/) Python package manager. `pip install proxycrawl`
+        
+        Then import the CrawlingAPI, ScraperAPI, etc as needed.
+        
+        ```python
+        from proxycrawl import CrawlingAPI, ScraperAPI, LeadsAPI, ScreenshotsAPI, StorageAPI
+        ```
+        
+        ### Upgrading to version 3
+        
+        Version 3 deprecates the usage of ProxyCrawlAPI in favour of CrawlingAPI (although is still usable). Please test the upgrade before deploying to production.
+        
+        ## Crawling API
+        
+        First initialize the CrawlingAPI class.
+        
+        ```python
+        api = CrawlingAPI({ 'token': 'YOUR_PROXYCRAWL_TOKEN' })
+        ```
+        
+        ### GET requests
+        
+        Pass the url that you want to scrape plus any options from the ones available in the [API documentation](https://proxycrawl.com/docs).
+        
+        ```python
+        api.get(url, options = {})
+        ```
+        
+        Example:
+        
+        ```python
+        response = api.get('https://www.facebook.com/britneyspears')
+        if response['status_code'] == 200:
+            print(response['body'])
+        ```
+        
+        You can pass any options from ProxyCrawl API.
+        
+        Example:
+        
+        ```python
+        response = api.get('https://www.reddit.com/r/pics/comments/5bx4bx/thanks_obama/', {
+            'user_agent': 'Mozilla/5.0 (Windows NT 6.2; rv:20.0) Gecko/20121202 Firefox/30.0',
+            'format': 'json'
+        })
+        if response['status_code'] == 200:
+            print(response['body'])
+        ```
+        
+        ### POST requests
+        
+        Pass the url that you want to scrape, the data that you want to send which can be either a json or a string, plus any options from the ones available in the [API documentation](https://proxycrawl.com/docs).
+        
+        ```python
+        api.post(url, dictionary or string data, options = {})
+        ```
+        
+        Example:
+        
+        ```python
+        response = api.post('https://producthunt.com/search', { 'text': 'example search' })
+        if response['status_code'] == 200:
+            print(response['body'])
+        ```
+        
+        You can send the data as `application/json` instead of `x-www-form-urlencoded` by setting option `post_content_type` as json.
+        
+        ```python
+        import json
+        response = api.post('https://httpbin.org/post', json.dumps({ 'some_json': 'with some value' }), { 'post_content_type': 'json' })
+        if response['status_code'] == 200:
+            print(response['body'])
+        ```
+        
+        ### Javascript requests
+        
+        If you need to scrape any website built with Javascript like React, Angular, Vue, etc. You just need to pass your javascript token and use the same calls. Note that only `.get` is available for javascript and not `.post`.
+        
+        ```python
+        api = CrawlingAPI({ 'token': 'YOUR_JAVASCRIPT_TOKEN' })
+        ```
+        
+        ```python
+        response = api.get('https://www.nfl.com')
+        if response['status_code'] == 200:
+            print(response['body'])
+        ```
+        
+        Same way you can pass javascript additional options.
+        
+        ```python
+        response = api.get('https://www.freelancer.com', { 'page_wait': 5000 })
+        if response['status_code'] == 200:
+            print(response['body'])
+        ```
+        
+        ## Original status
+        
+        You can always get the original status and proxycrawl status from the response. Read the [ProxyCrawl documentation](https://proxycrawl.com/docs) to learn more about those status.
+        
+        ```python
+        response = api.get('https://craiglist.com')
+        print(response['headers']['original_status'])
+        print(response['headers']['pc_status'])
+        ```
+        
+        If you have questions or need help using the library, please open an issue or [contact us](https://proxycrawl.com/contact).
+        
+        ## Scraper API
+        
+        The usage of the Scraper API is very similar, just change the class name to initialize.
+        
+        ```python
+        scraper_api = ScraperAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
+        
+        response = scraper_api.get('https://www.amazon.com/DualSense-Wireless-Controller-PlayStation-5/dp/B08FC6C75Y/')
+        if response['status_code'] == 200:
+            print(response['json']['name']) # Will print the name of the Amazon product
+        ```
+        
+        ## Leads API
+        
+        To find email leads you can use the leads API, you can check the full [API documentation](https://proxycrawl.com/docs/leads-api/) if needed.
+        
+        ```python
+        leads_api = LeadsAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
+        
+        response = leads_api.get_from_domain('microsoft.com')
+        
+        if response['status_code'] == 200:
+            print(response['json']['leads'])
+        ```
+        
+        ## Screenshots API
+        
+        Initialize with your Screenshots API token and call the `get` method.
+        
+        ```python
+        screenshots_api = ScreenshotsAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
+        response = screenshots_api.get('https://www.apple.com')
+        if response['status_code'] == 200:
+            print(response['headers']['success'])
+            print(response['headers']['url'])
+            print(response['headers']['remaining_requests'])
+            print(response['file'])
+        ```
+        
+        or specifying a file path
+        
+        ```python
+        screenshots_api = ScreenshotsAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
+        response = screenshots_api.get('https://www.apple.com', { 'save_to_path': 'apple.jpg' })
+        if response['status_code'] == 200:
+            print(response['headers']['success'])
+            print(response['headers']['url'])
+            print(response['headers']['remaining_requests'])
+            print(response['file'])
+        ```
+        
+        or if you set `store=true` then `screenshot_url` is set in the returned headers 
+        
+        ```python
+        screenshots_api = ScreenshotsAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
+        response = screenshots_api.get('https://www.apple.com', { 'store': 'true' })
+        if response['status_code'] == 200:
+            print(response['headers']['success'])
+            print(response['headers']['url'])
+            print(response['headers']['remaining_requests'])
+            print(response['file'])
+            print(response['headers']['screenshot_url'])
+        ```
+        
+        Note that `screenshots_api.get(url, options)` method accepts an [options](https://proxycrawl.com/docs/screenshots-api/parameters)
+        
+        ## Storage API
+        
+        Initialize the Storage API using your private token.
+        
+        ```python
+        storage_api = StorageAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
+        ```
+        
+        Pass the [url](https://proxycrawl.com/docs/storage-api/parameters/#url) that you want to get from [Proxycrawl Storage](https://proxycrawl.com/dashboard/storage).
+        
+        ```python
+        response = storage_api.get('https://www.apple.com')
+        if response['status_code'] == 200:
+            print(response['headers']['original_status'])
+            print(response['headers']['pc_status'])
+            print(response['headers']['url'])
+            print(response['headers']['rid'])
+            print(response['headers']['stored_at'])
+            print(response['body'])
+        ```
+        
+        or you can use the [RID](https://proxycrawl.com/docs/storage-api/parameters/#rid)
+        
+        ```python
+        response = storage_api.get('RID_REPLACE')
+        if response['status_code'] == 200:
+            print(response['headers']['original_status'])
+            print(response['headers']['pc_status'])
+            print(response['headers']['url'])
+            print(response['headers']['rid'])
+            print(response['headers']['stored_at'])
+            print(response['body'])
+        ```
+        
+        Note: One of the two RID or URL must be sent. So both are optional but it's mandatory to send one of the two.
+        
+        ### [Delete](https://proxycrawl.com/docs/storage-api/delete/) request
+        
+        To delete a storage item from your storage area, use the correct RID
+        
+        ```python
+        if storage_api.delete('RID_REPLACE'):
+          print('delete success')
+        else:
+          print('Unable to delete')
+        ```
+        
+        ### [Bulk](https://proxycrawl.com/docs/storage-api/bulk/) request
+        
+        To do a bulk request with a list of RIDs, please send the list of rids as an array
+        
+        ```python
+        response = storage_api.bulk(['RID1', 'RID2', 'RID3', ...])
+        if response['status_code'] == 200:
+            for item in response['json']:
+                print(item['original_status'])
+                print(item['pc_status'])
+                print(item['url'])
+                print(item['rid'])
+                print(item['stored_at'])
+                print(item['body'])
+        ```
+        
+        ### [RIDs](https://proxycrawl.com/docs/storage-api/rids) request
+        
+        To request a bulk list of RIDs from your storage area
+        
+        ```python
+        rids = storage_api.rids()
+        print(rids)
+        ```
+        
+        You can also specify a limit as a parameter
+        
+        ```python
+        storage_api.rids(100)
+        ```
+        
+        ### [Total Count](https://proxycrawl.com/docs/storage-api/total_count)
+        
+        To get the total number of documents in your storage area
+        
+        ```python
+        total_count = storage_api.totalCount()
+        print(total_count)
+        ```
+        
+        ## Custom timeout
+        
+        If you need to use a custom timeout, you can pass it to the class instance creation like the following:
+        
+        ```python
+        api = CrawlingAPI({ 'token': 'TOKEN', 'timeout': 120 })
+        ```
+        
+        Timeout is in seconds.
+        
+        ---
+        
+        Copyright 2023 ProxyCrawl
+        
+Keywords: scraping scraper crawler crawling proxycrawl api
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
```

### Comparing `proxycrawl-3.2.1/proxycrawl/base_api.py` & `proxycrawl-3.2.2/proxycrawl/base_api.py`

 * *Files identical despite different names*

### Comparing `proxycrawl-3.2.1/proxycrawl/crawling_api.py` & `proxycrawl-3.2.2/proxycrawl/crawling_api.py`

 * *Files identical despite different names*

### Comparing `proxycrawl-3.2.1/proxycrawl/scraper_api.py` & `proxycrawl-3.2.2/proxycrawl/scraper_api.py`

 * *Files identical despite different names*

### Comparing `proxycrawl-3.2.1/proxycrawl/screenshots_api.py` & `proxycrawl-3.2.2/proxycrawl/screenshots_api.py`

 * *Files identical despite different names*

### Comparing `proxycrawl-3.2.1/proxycrawl/storage_api.py` & `proxycrawl-3.2.2/proxycrawl/storage_api.py`

 * *Files identical despite different names*

### Comparing `proxycrawl-3.2.1/proxycrawl.egg-info/PKG-INFO` & `proxycrawl-3.2.2/proxycrawl.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,308 +1,311 @@
 Metadata-Version: 2.1
 Name: proxycrawl
-Version: 3.2.1
+Version: 3.2.2
 Summary: A Python class that acts as wrapper for ProxyCrawl scraping and crawling API
 Home-page: https://github.com/proxycrawl/proxycrawl-python
 Author: ProxyCrawl
 Author-email: info@proxycrawl.com
 License: Apache-2.0
+Description: # DEPRECATION NOTICE
+        
+        > :warning: **IMPORTANT:** This package is no longer maintained or supported. For the latest updates, please use our new package at [crawlbase-python](https://github.com/crawlbase-source/crawlbase-python).
+        
+        ---
+        
+        # ProxyCrawl API Python class
+        
+        A lightweight, dependency free Python class that acts as wrapper for ProxyCrawl API.
+        
+        ## Installing
+        
+        Choose a way of installing:
+        
+        - Download the python class from Github.
+        - Or use [PyPi](https://pypi.org/project/proxycrawl/) Python package manager. `pip install proxycrawl`
+        
+        Then import the CrawlingAPI, ScraperAPI, etc as needed.
+        
+        ```python
+        from proxycrawl import CrawlingAPI, ScraperAPI, LeadsAPI, ScreenshotsAPI, StorageAPI
+        ```
+        
+        ### Upgrading to version 3
+        
+        Version 3 deprecates the usage of ProxyCrawlAPI in favour of CrawlingAPI (although is still usable). Please test the upgrade before deploying to production.
+        
+        ## Crawling API
+        
+        First initialize the CrawlingAPI class.
+        
+        ```python
+        api = CrawlingAPI({ 'token': 'YOUR_PROXYCRAWL_TOKEN' })
+        ```
+        
+        ### GET requests
+        
+        Pass the url that you want to scrape plus any options from the ones available in the [API documentation](https://proxycrawl.com/docs).
+        
+        ```python
+        api.get(url, options = {})
+        ```
+        
+        Example:
+        
+        ```python
+        response = api.get('https://www.facebook.com/britneyspears')
+        if response['status_code'] == 200:
+            print(response['body'])
+        ```
+        
+        You can pass any options from ProxyCrawl API.
+        
+        Example:
+        
+        ```python
+        response = api.get('https://www.reddit.com/r/pics/comments/5bx4bx/thanks_obama/', {
+            'user_agent': 'Mozilla/5.0 (Windows NT 6.2; rv:20.0) Gecko/20121202 Firefox/30.0',
+            'format': 'json'
+        })
+        if response['status_code'] == 200:
+            print(response['body'])
+        ```
+        
+        ### POST requests
+        
+        Pass the url that you want to scrape, the data that you want to send which can be either a json or a string, plus any options from the ones available in the [API documentation](https://proxycrawl.com/docs).
+        
+        ```python
+        api.post(url, dictionary or string data, options = {})
+        ```
+        
+        Example:
+        
+        ```python
+        response = api.post('https://producthunt.com/search', { 'text': 'example search' })
+        if response['status_code'] == 200:
+            print(response['body'])
+        ```
+        
+        You can send the data as `application/json` instead of `x-www-form-urlencoded` by setting option `post_content_type` as json.
+        
+        ```python
+        import json
+        response = api.post('https://httpbin.org/post', json.dumps({ 'some_json': 'with some value' }), { 'post_content_type': 'json' })
+        if response['status_code'] == 200:
+            print(response['body'])
+        ```
+        
+        ### Javascript requests
+        
+        If you need to scrape any website built with Javascript like React, Angular, Vue, etc. You just need to pass your javascript token and use the same calls. Note that only `.get` is available for javascript and not `.post`.
+        
+        ```python
+        api = CrawlingAPI({ 'token': 'YOUR_JAVASCRIPT_TOKEN' })
+        ```
+        
+        ```python
+        response = api.get('https://www.nfl.com')
+        if response['status_code'] == 200:
+            print(response['body'])
+        ```
+        
+        Same way you can pass javascript additional options.
+        
+        ```python
+        response = api.get('https://www.freelancer.com', { 'page_wait': 5000 })
+        if response['status_code'] == 200:
+            print(response['body'])
+        ```
+        
+        ## Original status
+        
+        You can always get the original status and proxycrawl status from the response. Read the [ProxyCrawl documentation](https://proxycrawl.com/docs) to learn more about those status.
+        
+        ```python
+        response = api.get('https://craiglist.com')
+        print(response['headers']['original_status'])
+        print(response['headers']['pc_status'])
+        ```
+        
+        If you have questions or need help using the library, please open an issue or [contact us](https://proxycrawl.com/contact).
+        
+        ## Scraper API
+        
+        The usage of the Scraper API is very similar, just change the class name to initialize.
+        
+        ```python
+        scraper_api = ScraperAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
+        
+        response = scraper_api.get('https://www.amazon.com/DualSense-Wireless-Controller-PlayStation-5/dp/B08FC6C75Y/')
+        if response['status_code'] == 200:
+            print(response['json']['name']) # Will print the name of the Amazon product
+        ```
+        
+        ## Leads API
+        
+        To find email leads you can use the leads API, you can check the full [API documentation](https://proxycrawl.com/docs/leads-api/) if needed.
+        
+        ```python
+        leads_api = LeadsAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
+        
+        response = leads_api.get_from_domain('microsoft.com')
+        
+        if response['status_code'] == 200:
+            print(response['json']['leads'])
+        ```
+        
+        ## Screenshots API
+        
+        Initialize with your Screenshots API token and call the `get` method.
+        
+        ```python
+        screenshots_api = ScreenshotsAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
+        response = screenshots_api.get('https://www.apple.com')
+        if response['status_code'] == 200:
+            print(response['headers']['success'])
+            print(response['headers']['url'])
+            print(response['headers']['remaining_requests'])
+            print(response['file'])
+        ```
+        
+        or specifying a file path
+        
+        ```python
+        screenshots_api = ScreenshotsAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
+        response = screenshots_api.get('https://www.apple.com', { 'save_to_path': 'apple.jpg' })
+        if response['status_code'] == 200:
+            print(response['headers']['success'])
+            print(response['headers']['url'])
+            print(response['headers']['remaining_requests'])
+            print(response['file'])
+        ```
+        
+        or if you set `store=true` then `screenshot_url` is set in the returned headers 
+        
+        ```python
+        screenshots_api = ScreenshotsAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
+        response = screenshots_api.get('https://www.apple.com', { 'store': 'true' })
+        if response['status_code'] == 200:
+            print(response['headers']['success'])
+            print(response['headers']['url'])
+            print(response['headers']['remaining_requests'])
+            print(response['file'])
+            print(response['headers']['screenshot_url'])
+        ```
+        
+        Note that `screenshots_api.get(url, options)` method accepts an [options](https://proxycrawl.com/docs/screenshots-api/parameters)
+        
+        ## Storage API
+        
+        Initialize the Storage API using your private token.
+        
+        ```python
+        storage_api = StorageAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
+        ```
+        
+        Pass the [url](https://proxycrawl.com/docs/storage-api/parameters/#url) that you want to get from [Proxycrawl Storage](https://proxycrawl.com/dashboard/storage).
+        
+        ```python
+        response = storage_api.get('https://www.apple.com')
+        if response['status_code'] == 200:
+            print(response['headers']['original_status'])
+            print(response['headers']['pc_status'])
+            print(response['headers']['url'])
+            print(response['headers']['rid'])
+            print(response['headers']['stored_at'])
+            print(response['body'])
+        ```
+        
+        or you can use the [RID](https://proxycrawl.com/docs/storage-api/parameters/#rid)
+        
+        ```python
+        response = storage_api.get('RID_REPLACE')
+        if response['status_code'] == 200:
+            print(response['headers']['original_status'])
+            print(response['headers']['pc_status'])
+            print(response['headers']['url'])
+            print(response['headers']['rid'])
+            print(response['headers']['stored_at'])
+            print(response['body'])
+        ```
+        
+        Note: One of the two RID or URL must be sent. So both are optional but it's mandatory to send one of the two.
+        
+        ### [Delete](https://proxycrawl.com/docs/storage-api/delete/) request
+        
+        To delete a storage item from your storage area, use the correct RID
+        
+        ```python
+        if storage_api.delete('RID_REPLACE'):
+          print('delete success')
+        else:
+          print('Unable to delete')
+        ```
+        
+        ### [Bulk](https://proxycrawl.com/docs/storage-api/bulk/) request
+        
+        To do a bulk request with a list of RIDs, please send the list of rids as an array
+        
+        ```python
+        response = storage_api.bulk(['RID1', 'RID2', 'RID3', ...])
+        if response['status_code'] == 200:
+            for item in response['json']:
+                print(item['original_status'])
+                print(item['pc_status'])
+                print(item['url'])
+                print(item['rid'])
+                print(item['stored_at'])
+                print(item['body'])
+        ```
+        
+        ### [RIDs](https://proxycrawl.com/docs/storage-api/rids) request
+        
+        To request a bulk list of RIDs from your storage area
+        
+        ```python
+        rids = storage_api.rids()
+        print(rids)
+        ```
+        
+        You can also specify a limit as a parameter
+        
+        ```python
+        storage_api.rids(100)
+        ```
+        
+        ### [Total Count](https://proxycrawl.com/docs/storage-api/total_count)
+        
+        To get the total number of documents in your storage area
+        
+        ```python
+        total_count = storage_api.totalCount()
+        print(total_count)
+        ```
+        
+        ## Custom timeout
+        
+        If you need to use a custom timeout, you can pass it to the class instance creation like the following:
+        
+        ```python
+        api = CrawlingAPI({ 'token': 'TOKEN', 'timeout': 120 })
+        ```
+        
+        Timeout is in seconds.
+        
+        ---
+        
+        Copyright 2023 ProxyCrawl
+        
 Keywords: scraping scraper crawler crawling proxycrawl api
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ProxyCrawl API Python class
-
-A lightweight, dependency free Python class that acts as wrapper for ProxyCrawl API.
-
-## Installing
-
-Choose a way of installing:
-
-- Download the python class from Github.
-- Or use [PyPi](https://pypi.org/project/proxycrawl/) Python package manager. `pip install proxycrawl`
-
-Then import the CrawlingAPI, ScraperAPI, etc as needed.
-
-```python
-from proxycrawl import CrawlingAPI, ScraperAPI, LeadsAPI, ScreenshotsAPI, StorageAPI
-```
-
-### Upgrading to version 3
-
-Version 3 deprecates the usage of ProxyCrawlAPI in favour of CrawlingAPI (although is still usable). Please test the upgrade before deploying to production.
-
-## Crawling API
-
-First initialize the CrawlingAPI class.
-
-```python
-api = CrawlingAPI({ 'token': 'YOUR_PROXYCRAWL_TOKEN' })
-```
-
-### GET requests
-
-Pass the url that you want to scrape plus any options from the ones available in the [API documentation](https://proxycrawl.com/docs).
-
-```python
-api.get(url, options = {})
-```
-
-Example:
-
-```python
-response = api.get('https://www.facebook.com/britneyspears')
-if response['status_code'] == 200:
-    print(response['body'])
-```
-
-You can pass any options from ProxyCrawl API.
-
-Example:
-
-```python
-response = api.get('https://www.reddit.com/r/pics/comments/5bx4bx/thanks_obama/', {
-    'user_agent': 'Mozilla/5.0 (Windows NT 6.2; rv:20.0) Gecko/20121202 Firefox/30.0',
-    'format': 'json'
-})
-if response['status_code'] == 200:
-    print(response['body'])
-```
-
-### POST requests
-
-Pass the url that you want to scrape, the data that you want to send which can be either a json or a string, plus any options from the ones available in the [API documentation](https://proxycrawl.com/docs).
-
-```python
-api.post(url, dictionary or string data, options = {})
-```
-
-Example:
-
-```python
-response = api.post('https://producthunt.com/search', { 'text': 'example search' })
-if response['status_code'] == 200:
-    print(response['body'])
-```
-
-You can send the data as `application/json` instead of `x-www-form-urlencoded` by setting option `post_content_type` as json.
-
-```python
-import json
-response = api.post('https://httpbin.org/post', json.dumps({ 'some_json': 'with some value' }), { 'post_content_type': 'json' })
-if response['status_code'] == 200:
-    print(response['body'])
-```
-
-### Javascript requests
-
-If you need to scrape any website built with Javascript like React, Angular, Vue, etc. You just need to pass your javascript token and use the same calls. Note that only `.get` is available for javascript and not `.post`.
-
-```python
-api = CrawlingAPI({ 'token': 'YOUR_JAVASCRIPT_TOKEN' })
-```
-
-```python
-response = api.get('https://www.nfl.com')
-if response['status_code'] == 200:
-    print(response['body'])
-```
-
-Same way you can pass javascript additional options.
-
-```python
-response = api.get('https://www.freelancer.com', { 'page_wait': 5000 })
-if response['status_code'] == 200:
-    print(response['body'])
-```
-
-## Original status
-
-You can always get the original status and proxycrawl status from the response. Read the [ProxyCrawl documentation](https://proxycrawl.com/docs) to learn more about those status.
-
-```python
-response = api.get('https://craiglist.com')
-print(response['headers']['original_status'])
-print(response['headers']['pc_status'])
-```
-
-If you have questions or need help using the library, please open an issue or [contact us](https://proxycrawl.com/contact).
-
-## Scraper API
-
-The usage of the Scraper API is very similar, just change the class name to initialize.
-
-```python
-scraper_api = ScraperAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
-
-response = scraper_api.get('https://www.amazon.com/DualSense-Wireless-Controller-PlayStation-5/dp/B08FC6C75Y/')
-if response['status_code'] == 200:
-    print(response['json']['name']) # Will print the name of the Amazon product
-```
-
-## Leads API
-
-To find email leads you can use the leads API, you can check the full [API documentation](https://proxycrawl.com/docs/leads-api/) if needed.
-
-```python
-leads_api = LeadsAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
-
-response = leads_api.get_from_domain('microsoft.com')
-
-if response['status_code'] == 200:
-    print(response['json']['leads'])
-```
-
-## Screenshots API
-
-Initialize with your Screenshots API token and call the `get` method.
-
-```python
-screenshots_api = ScreenshotsAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
-response = screenshots_api.get('https://www.apple.com')
-if response['status_code'] == 200:
-    print(response['headers']['success'])
-    print(response['headers']['url'])
-    print(response['headers']['remaining_requests'])
-    print(response['file'])
-```
-
-or specifying a file path
-
-```python
-screenshots_api = ScreenshotsAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
-response = screenshots_api.get('https://www.apple.com', { 'save_to_path': 'apple.jpg' })
-if response['status_code'] == 200:
-    print(response['headers']['success'])
-    print(response['headers']['url'])
-    print(response['headers']['remaining_requests'])
-    print(response['file'])
-```
-
-or if you set `store=true` then `screenshot_url` is set in the returned headers 
-
-```python
-screenshots_api = ScreenshotsAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
-response = screenshots_api.get('https://www.apple.com', { 'store': 'true' })
-if response['status_code'] == 200:
-    print(response['headers']['success'])
-    print(response['headers']['url'])
-    print(response['headers']['remaining_requests'])
-    print(response['file'])
-    print(response['headers']['screenshot_url'])
-```
-
-Note that `screenshots_api.get(url, options)` method accepts an [options](https://proxycrawl.com/docs/screenshots-api/parameters)
-
-## Storage API
-
-Initialize the Storage API using your private token.
-
-```python
-storage_api = StorageAPI({ 'token': 'YOUR_NORMAL_TOKEN' })
-```
-
-Pass the [url](https://proxycrawl.com/docs/storage-api/parameters/#url) that you want to get from [Proxycrawl Storage](https://proxycrawl.com/dashboard/storage).
-
-```python
-response = storage_api.get('https://www.apple.com')
-if response['status_code'] == 200:
-    print(response['headers']['original_status'])
-    print(response['headers']['pc_status'])
-    print(response['headers']['url'])
-    print(response['headers']['rid'])
-    print(response['headers']['stored_at'])
-    print(response['body'])
-```
-
-or you can use the [RID](https://proxycrawl.com/docs/storage-api/parameters/#rid)
-
-```python
-response = storage_api.get('RID_REPLACE')
-if response['status_code'] == 200:
-    print(response['headers']['original_status'])
-    print(response['headers']['pc_status'])
-    print(response['headers']['url'])
-    print(response['headers']['rid'])
-    print(response['headers']['stored_at'])
-    print(response['body'])
-```
-
-Note: One of the two RID or URL must be sent. So both are optional but it's mandatory to send one of the two.
-
-### [Delete](https://proxycrawl.com/docs/storage-api/delete/) request
-
-To delete a storage item from your storage area, use the correct RID
-
-```python
-if storage_api.delete('RID_REPLACE'):
-  print('delete success')
-else:
-  print('Unable to delete')
-```
-
-### [Bulk](https://proxycrawl.com/docs/storage-api/bulk/) request
-
-To do a bulk request with a list of RIDs, please send the list of rids as an array
-
-```python
-response = storage_api.bulk(['RID1', 'RID2', 'RID3', ...])
-if response['status_code'] == 200:
-    for item in response['json']:
-        print(item['original_status'])
-        print(item['pc_status'])
-        print(item['url'])
-        print(item['rid'])
-        print(item['stored_at'])
-        print(item['body'])
-```
-
-### [RIDs](https://proxycrawl.com/docs/storage-api/rids) request
-
-To request a bulk list of RIDs from your storage area
-
-```python
-rids = storage_api.rids()
-print(rids)
-```
-
-You can also specify a limit as a parameter
-
-```python
-storage_api.rids(100)
-```
-
-### [Total Count](https://proxycrawl.com/docs/storage-api/total_count)
-
-To get the total number of documents in your storage area
-
-```python
-total_count = storage_api.totalCount()
-print(total_count)
-```
-
-## Custom timeout
-
-If you need to use a custom timeout, you can pass it to the class instance creation like the following:
-
-```python
-api = CrawlingAPI({ 'token': 'TOKEN', 'timeout': 120 })
-```
-
-Timeout is in seconds.
-
----
-
-Copyright 2021 ProxyCrawl
-
-
```

### Comparing `proxycrawl-3.2.1/setup.py` & `proxycrawl-3.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     from distutils.core import setup, find_packages
 
 readme = open('README.md').read()
 
 setup(
     name = 'proxycrawl',
     license = 'Apache-2.0',
-    version = '3.2.1',
+    version = '3.2.2',
     description = 'A Python class that acts as wrapper for ProxyCrawl scraping and crawling API',
     long_description = readme,
     long_description_content_type = 'text/markdown',
     author = 'ProxyCrawl',
     author_email = 'info@proxycrawl.com',
     url = 'https://github.com/proxycrawl/proxycrawl-python',
     keywords = 'scraping scraper crawler crawling proxycrawl api',
```

