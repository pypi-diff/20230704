# Comparing `tmp/asyncioget-0.10.tar.gz` & `tmp/asyncioget-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncioget-0.10.tar", last modified: Mon Jul  3 04:14:33 2023, max compression
+gzip compressed data, was "asyncioget-0.11.tar", last modified: Mon Jul  3 22:38:48 2023, max compression
```

## Comparing `asyncioget-0.10.tar` & `asyncioget-0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 04:14:33.881078 asyncioget-0.10/
--rw-rw-rw-   0        0        0     1148 2023-07-03 04:14:27.000000 asyncioget-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      101 2023-07-03 04:14:25.000000 asyncioget-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0    12936 2023-07-03 04:14:33.882074 asyncioget-0.10/PKG-INFO
--rw-rw-rw-   0        0        0    12220 2023-07-03 04:12:15.000000 asyncioget-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 04:14:33.856144 asyncioget-0.10/asyncioget/
--rw-rw-rw-   0        0        0    12220 2023-07-03 04:12:15.000000 asyncioget-0.10/asyncioget/README.MD
--rw-rw-rw-   0        0        0     3372 2023-07-03 04:11:55.000000 asyncioget-0.10/asyncioget/__init__.py
--rw-rw-rw-   0        0        0        8 2023-07-03 04:14:32.000000 asyncioget-0.10/asyncioget/requirements.txt
--rw-rw-rw-   0        0        0    10447 2023-07-03 04:14:32.000000 asyncioget-0.10/asyncioget/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-03 04:14:33.872101 asyncioget-0.10/asyncioget.egg-info/
--rw-rw-rw-   0        0        0    12936 2023-07-03 04:14:33.000000 asyncioget-0.10/asyncioget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-03 04:14:33.000000 asyncioget-0.10/asyncioget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 04:14:33.000000 asyncioget-0.10/asyncioget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-03 04:14:33.000000 asyncioget-0.10/asyncioget.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-03 04:14:33.000000 asyncioget-0.10/asyncioget.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-03 04:14:33.891051 asyncioget-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1372 2023-07-03 04:14:32.000000 asyncioget-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 22:38:48.416157 asyncioget-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-07-03 22:38:36.000000 asyncioget-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      101 2023-07-03 22:38:34.000000 asyncioget-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0    12936 2023-07-03 22:38:48.417155 asyncioget-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0    12220 2023-07-03 04:17:28.000000 asyncioget-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 22:38:48.408178 asyncioget-0.11/asyncioget/
+-rw-rw-rw-   0        0        0    12220 2023-07-03 04:17:28.000000 asyncioget-0.11/asyncioget/README.MD
+-rw-rw-rw-   0        0        0     1891 2023-07-03 22:37:30.000000 asyncioget-0.11/asyncioget/__init__.py
+-rw-rw-rw-   0        0        0        8 2023-07-03 22:38:47.000000 asyncioget-0.11/asyncioget/requirements.txt
+-rw-rw-rw-   0        0        0    10447 2023-07-03 22:38:47.000000 asyncioget-0.11/asyncioget/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-03 22:38:48.416157 asyncioget-0.11/asyncioget.egg-info/
+-rw-rw-rw-   0        0        0    12936 2023-07-03 22:38:48.000000 asyncioget-0.11/asyncioget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-03 22:38:48.000000 asyncioget-0.11/asyncioget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 22:38:48.000000 asyncioget-0.11/asyncioget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-03 22:38:48.000000 asyncioget-0.11/asyncioget.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-03 22:38:48.000000 asyncioget-0.11/asyncioget.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-03 22:38:48.418151 asyncioget-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1372 2023-07-03 22:38:47.000000 asyncioget-0.11/setup.py
```

### Comparing `asyncioget-0.10/LICENSE.rst` & `asyncioget-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `asyncioget-0.10/PKG-INFO` & `asyncioget-0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncioget
-Version: 0.10
+Version: 0.11
 Summary: simplifies the process of downloading multiple URLs concurrently, provides control over concurrency, and offers flexibility for customization
 Home-page: https://github.com/hansalemaos/asyncioget
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: requests,asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `asyncioget-0.10/README.md` & `asyncioget-0.11/README.md`

 * *Files identical despite different names*

### Comparing `asyncioget-0.10/asyncioget/README.MD` & `asyncioget-0.11/asyncioget/README.MD`

 * *Files identical despite different names*

### Comparing `asyncioget-0.10/asyncioget/__init__.py` & `asyncioget-0.11/asyncioget/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,55 @@
-import asyncio
 from random import uniform
 import requests
-
-
-async def get_with_requests(url, verbose, sleeptime, *args, **kwargs):
-    """Perform a download using requests.get() with a random sleep time.
-
-    Args:
-        url (str): The URL to download.
-        verbose (bool): If True, print the progress of each download.
-        sleeptime (tuple[int|float, int|float]): A tuple representing the range of random sleep times in seconds before each download.
-        *args: Additional positional arguments to pass to the requests.get() function.
-        **kwargs: Additional keyword arguments to pass to the requests.get() function.
-
-    Returns:
-        A tuple containing the URL and the downloaded data, or None if the download failed.
-
-    """
-    if verbose:
-        print(f"Downloading: {url}")
-    if sleeptime:
-        await asyncio.sleep(uniform(*sleeptime))
-    data = None
-    try:
-        with requests.get(url, *args, **kwargs) as res:
-            data = res
-    except Exception as fe:
-        if verbose:
-            print(fe)
-    return url, data
-
-
-async def start_all_downloads(urls, semaphore, verbose, sleeptime, *args, **kwargs):
-    """Start all downloads with limited concurrency using a semaphore.
-
-    Args:
-        urls (list or tuple): A list or tuple of URLs to download.
-        semaphore (asyncio.Semaphore): Semaphore to limit the number of concurrent tasks.
-        verbose (bool): If True, print the progress of each download.
-        sleeptime (tuple[int|float, int|float]): A tuple representing the range of random sleep times in seconds before each download.
-        *args: Additional positional arguments to pass to the requests.get() function.
-        **kwargs: Additional keyword arguments to pass to the requests.get() function.
-
-    Returns:
-        A list of tuples containing the URL and the downloaded data for each successful download.
-
-    """
-    results = []
-    for url in urls:
-        async with semaphore:
-            result = await get_with_requests(url, verbose, sleeptime, *args, **kwargs)
-            results.append(result)
-    return results
+import asyncio
 
 
 def downloadlinks(
     urls: list | tuple,
     threads: int = 10,
     sleeptime: tuple[int | float, int | float] = (0.01, 0.02),
     verbose: bool = True,
     *args,
     **kwargs,
 ):
-    """Download multiple URLs asynchronously using asyncio and requests.
+    """Perform a download using requests.get() with a random sleep time.
 
     Args:
-        urls (list or tuple): A list or tuple of URLs to download.
-        threads (int, optional): The maximum number of concurrent downloads (default: 10).
-        sleeptime (tuple[int|float, int|float], optional): A tuple representing the range of random sleep times in seconds before each download (default: (.01, .02)).
-        verbose (bool, optional): If True, print the progress of each download (default: True).
+        url (str): The URL to download.
+        verbose (bool): If True, print the progress of each download.
+        sleeptime (tuple[int|float, int|float]): A tuple representing the range of random sleep times in seconds before each download.
         *args: Additional positional arguments to pass to the requests.get() function.
         **kwargs: Additional keyword arguments to pass to the requests.get() function.
 
     Returns:
-        A list of tuples containing the URL and the downloaded data for each successful download.
+        A tuple containing the URL and the downloaded data, or None if the download failed.
 
     """
+    background_tasks = list()
     semaphore = asyncio.Semaphore(threads)
-    loop = asyncio.get_event_loop()
-    return loop.run_until_complete(
-        start_all_downloads(urls, semaphore, verbose, sleeptime, *args, **kwargs)
-    )
+
+    async def _downloadlinks():
+        async def get_with_requests(url, verbose, sleeptime, *args, **kwargs):
+            async with semaphore:
+                if verbose:
+                    print(f"Downloading: {url}")
+                if sleeptime:
+                    await asyncio.sleep(uniform(*sleeptime))
+                data = None
+                try:
+                    with requests.get(url, *args, **kwargs) as res:
+                        data = res
+                except Exception as fe:
+                    if verbose:
+                        print(fe)
+                return url, data
+
+        for url in urls:
+            task = asyncio.create_task(
+                get_with_requests(url, verbose, sleeptime, *args, **kwargs)
+            )
+            background_tasks.append(task)
+
+        return await asyncio.gather(*background_tasks)
+
+    return asyncio.run(_downloadlinks())
```

### Comparing `asyncioget-0.10/asyncioget/thirdparty.json` & `asyncioget-0.11/asyncioget/thirdparty.json`

 * *Files identical despite different names*

### Comparing `asyncioget-0.10/asyncioget.egg-info/PKG-INFO` & `asyncioget-0.11/asyncioget.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncioget
-Version: 0.10
+Version: 0.11
 Summary: simplifies the process of downloading multiple URLs concurrently, provides control over concurrency, and offers flexibility for customization
 Home-page: https://github.com/hansalemaos/asyncioget
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: requests,asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `asyncioget-0.10/setup.py` & `asyncioget-0.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''simplifies the process of downloading multiple URLs concurrently, provides control over concurrency, and offers flexibility for customization'''
 
 # Setting up
 setup(
     name="asyncioget",
     version=VERSION,
     license='MIT',
```

