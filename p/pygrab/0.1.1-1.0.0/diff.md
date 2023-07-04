# Comparing `tmp/pygrab-0.1.1.tar.gz` & `tmp/pygrab-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrab-0.1.1.tar", last modified: Mon Jun 12 05:44:03 2023, max compression
+gzip compressed data, was "pygrab-1.0.0.tar", last modified: Tue Jul  4 21:18:28 2023, max compression
```

## Comparing `pygrab-0.1.1.tar` & `pygrab-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 05:44:03.458000 pygrab-0.1.1/
--rw-rw-rw-   0        0        0      262 2023-06-12 05:44:03.451000 pygrab-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-05-31 05:39:20.000000 pygrab-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 05:44:03.394000 pygrab-0.1.1/pygrab/
--rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-0.1.1/pygrab/__init__.py
--rw-rw-rw-   0        0        0    12049 2023-06-12 05:33:10.000000 pygrab-0.1.1/pygrab/pygrab.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:44:03.444000 pygrab-0.1.1/pygrab.egg-info/
--rw-rw-rw-   0        0        0      262 2023-06-12 05:44:03.000000 pygrab-0.1.1/pygrab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-06-12 05:44:03.000000 pygrab-0.1.1/pygrab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 05:44:03.000000 pygrab-0.1.1/pygrab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-12 05:44:03.000000 pygrab-0.1.1/pygrab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-12 05:44:03.000000 pygrab-0.1.1/pygrab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 05:44:03.456000 pygrab-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      338 2023-06-12 05:41:49.000000 pygrab-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 21:18:28.639000 pygrab-1.0.0/
+-rw-rw-rw-   0        0        0      262 2023-07-04 21:18:28.630000 pygrab-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-31 05:39:20.000000 pygrab-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 21:18:28.555000 pygrab-1.0.0/pygrab/
+-rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-1.0.0/pygrab/__init__.py
+-rw-rw-rw-   0        0        0    11177 2023-07-04 21:13:44.000000 pygrab-1.0.0/pygrab/pygrab.py
+drwxrwxrwx   0        0        0        0 2023-07-04 21:18:28.620000 pygrab-1.0.0/pygrab.egg-info/
+-rw-rw-rw-   0        0        0      262 2023-07-04 21:18:28.000000 pygrab-1.0.0/pygrab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-07-04 21:18:28.000000 pygrab-1.0.0/pygrab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 21:18:28.000000 pygrab-1.0.0/pygrab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-04 21:18:28.000000 pygrab-1.0.0/pygrab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-04 21:18:28.000000 pygrab-1.0.0/pygrab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 21:18:28.637000 pygrab-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      338 2023-07-04 21:16:14.000000 pygrab-1.0.0/setup.py
```

### Comparing `pygrab-0.1.1/pygrab/pygrab.py` & `pygrab-1.0.0/pygrab/pygrab.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                     
                 cls.PROXY_LIST.append(lst[i].split(':'))
         raise Exception("Incorrect formatting for setting proxies. Must be [['23.144.56.65', '8080'], ...] or ['23.144.56.65:8080', ...]")
 
 
 
 
-def get(url: str, use_proxy=False, retries=5, encoding='utf-8', enable_js=False, *args, **kwargs): 
+def get(url: str, use_proxy=False, retries=5, enable_js=False, *args, **kwargs) -> str: 
     """
     Gets the content at the specified URL.
 
     Parameters:
     url (str): The URL to get.
     use_proxy (bool, optional): Whether to use a proxy. Defaults to False.
     retries (int, optional): The number of times to retry the request if it fails. Defaults to 5.
@@ -100,19 +100,16 @@
 
     Returns:
     requests.Response: The response from the server.
     """
     local_file_starts = ['./', 'C:', '/'] 
     url_file_starts = ['http', 'ftp:', 'mailto:']
     if any([url.startswith(i) for i in local_file_starts]):
-        return __local_grab(url, encoding=encoding)
-    elif any([url.startswith(i) for i in url_file_starts]):
-        if encoding != 'utf-8':
-            raise Exception("'encoding' argument is only relevent to grabbing local files.")
-        
+        raise ValueError ("Url must start with http. use get_local() for local requests.")
+    elif any([url.startswith(i) for i in url_file_starts]):        
         if enable_js:
             return __grab_enable_js(url)
         else:
             session = _requests.Session()
             retry = _requests.packages.urllib3.util.retry.Retry(total=retries, backoff_factor=0.1, status_forcelist=[500, 502, 503, 504])
             adapter = _requests.adapters.HTTPAdapter(max_retries=retry)
             session.mount('http://', adapter)
@@ -127,18 +124,18 @@
                     'https': f'https://{temp_prox[0]}:{temp_prox[1]}'
                 }
                 try:
                     return session.get(url, *args, **kwargs, proxies=proxies)
                 except Exception as err:
                     raise Exception(f'{err}\n\nThere seems to have been an error with the proxy IP. Please note that free proxies may not be reliable.')
 
-            return session.get(url, *args, **kwargs)
+            return str(session.get(url, *args, **kwargs).text)
     raise Exception(f"Invalid url: {url}")
     
-def get_async(urls, use_proxy=False, retries=5, encoding='utf-8', enable_js=False, time_rest=0, *args, **kwargs) -> list:
+def get_async(urls, use_proxy=False, retries=5, enable_js=False, time_rest=0, *args, **kwargs) -> list:
     """
     Gets multiple URLs asynchronously.
 
     This function sends HTTP requests to a list of URLs in separate threads, allowing for concurrent HTTP requests.
     The function returns a list of responses from the grabbed URLs.
 
     Args:
@@ -152,28 +149,33 @@
     Returns:
         list: A list of responses from the grabbed URLs.
     """
     # only import if async functionality is needed
     import threading as _threading
     import time as _time
     if type(urls) == str:
-        return [get(urls, use_proxy=use_proxy, retries=retries, encoding=encoding, enable_js=enable_js, *args, **kwargs)]
+        return [get(urls, use_proxy=use_proxy, retries=retries, enable_js=enable_js, *args, **kwargs)]
 
     result = []
     threads = []
     for url in urls:
         threads.append(_threading.Thread(target=__grab_thread_wrapper, args=[url, result, args, kwargs, use_proxy, retries, enable_js]))
         threads[-1].start()
         _time.sleep(time_rest)
     
     for thread in threads:
         thread.join()
         
     return result
 
+def get_local(filename:str, local_read_type:str='r', encoding:str='utf-8'):
+    with open(filename, local_read_type, encoding=encoding) as f:
+        data = f.read()
+    return data
+
 def download(url: str, name:str=None, use_proxy=False, retries=5) -> None:
     if '.' not in url:
         raise Exception("Argument 'url' needs a filepath extention")
     
 
     if name is not None:
         if '.' not in name:
@@ -215,27 +217,24 @@
     for thread in threads:
         thread.join()
     
 
 def head(url, **kwargs):
     return _requests.head(url, **kwargs)
 
-def post(url:str, data=None, json=None, local_save_type:str=None, encoding:str='utf-8', **kwargs):
+def post(url:str, data=None, json=None, **kwargs):
     local_file_starts = ['./', 'C:', '/'] 
-    
     if any([url.startswith(i) for i in local_file_starts]):
-        if local_save_type is None: local_save_type = 'w'
-        
-        with open(url, local_save_type, encoding=encoding) as f:
-            f.write(data)
-    else:
-        if (local_save_type is not None or encoding != 'utf-8'):
-            raise Exception("Arguments 'local_save_type' and 'encoding' are only relevent for posting to local files.")
+        raise ValueError("use post_local() for creation of local files.")
         
-        return _requests.post(url, data=data, json=json, **kwargs)
+    return _requests.post(url, data=data, json=json, **kwargs)
+
+def post_local(filepath:str, data:str, local_save_type:str="w", encoding:str='utf-8') -> None:
+    with open(filepath, local_save_type, encoding=encoding) as f:
+        f.write(str(data))
 
 def put(url, data=None, **kwargs):
     return _requests.put(url, data=data, **kwargs)
 
 def patch(url, data=None, **kwargs):
     return _requests.patch(url, data=data, **kwargs)
 
@@ -270,34 +269,14 @@
         only working proxies.
 
     Returns:
         None
     """
     ProxyList.update_proxies()
 
-def __local_grab(dir: str, encoding='utf-8'):
-    acceptableRegFiles = ['.txt', '.py', '.js', '.c', '.html', '.css', '.xml', '.md', '.yaml', '.yml', '.ipynb']
-    acceptableImgFiles = ['.png', '.jpg']
-    
-    if any([dir.endswith(i) for i in acceptableRegFiles]):
-        with open(dir, 'r', encoding=encoding) as f:
-            data = f.read()
-        return data
-    elif dir.endswith('.csv'):
-        with open(dir, 'r', encoding=encoding) as f:
-            data = f.read().strip().split("\n")
-        data = [i.split(",") for i in data ]
-        return data
-    if any([dir.endswith(i) for i in acceptableImgFiles]):
-        with open(dir, 'rb') as f:
-            data = f.read()
-        return data
-
-    raise Exception(f"File type not supported: {dir}")
-
 def __grab_thread_wrapper(url:str, payload:list, args, kwargs, use_proxy=False, retries=5, enable_js=False):
     res = get(url, use_proxy=use_proxy, retries=retries, enable_js=enable_js, *args, **kwargs)
     payload.append(res)
 
 def __grab_enable_js(url):
     return _asyncio.get_event_loop().run_until_complete(__grab_enable_js_async(url))
```

