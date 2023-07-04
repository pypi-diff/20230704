# Comparing `tmp/pocx-0.2.2.tar.gz` & `tmp/pocx-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocx-0.2.2.tar", max compression
+gzip compressed data, was "pocx-0.2.3.tar", max compression
```

## Comparing `pocx-0.2.2.tar` & `pocx-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1061 2022-07-29 06:18:41.570224 pocx-0.2.2/LICENSE
--rw-r--r--   0        0        0     4585 2022-07-29 06:18:41.570224 pocx-0.2.2/README.md
--rw-r--r--   0        0        0       83 2022-07-29 06:20:40.191065 pocx-0.2.2/pocx/__init__.py
--rw-r--r--   0        0        0     2780 2022-07-29 06:18:41.570224 pocx-0.2.2/pocx/aio_poc.py
--rw-r--r--   0        0        0     2565 2022-07-29 06:18:41.570224 pocx-0.2.2/pocx/basic_poc.py
--rw-r--r--   0        0        0       46 2022-07-29 06:18:41.570224 pocx-0.2.2/pocx/funcs/__init__.py
--rw-r--r--   0        0        0     1821 2022-07-29 06:18:41.570224 pocx-0.2.2/pocx/funcs/ceye.py
--rw-r--r--   0        0        0     4229 2022-07-29 06:21:49.614869 pocx-0.2.2/pocx/funcs/fofa.py
--rw-r--r--   0        0        0     2598 2022-07-29 06:18:41.570224 pocx-0.2.2/pocx/funcs/snow_flake.py
--rw-r--r--   0        0        0      783 2022-07-29 06:22:27.485120 pocx-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5641 2022-07-29 06:22:28.763748 pocx-0.2.2/setup.py
--rw-r--r--   0        0        0     5397 2022-07-29 06:22:28.764091 pocx-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-04 01:06:08.440840 pocx-0.2.3/LICENSE
+-rw-r--r--   0        0        0     5850 2023-07-04 02:07:17.497530 pocx-0.2.3/README.md
+-rw-r--r--   0        0        0       83 2023-07-04 02:09:36.921977 pocx-0.2.3/pocx/__init__.py
+-rw-r--r--   0        0        0     3305 2023-07-04 02:06:49.370627 pocx-0.2.3/pocx/aio_poc.py
+-rw-r--r--   0        0        0     3080 2023-07-04 02:06:49.383961 pocx-0.2.3/pocx/basic_poc.py
+-rw-r--r--   0        0        0       46 2023-07-04 01:06:08.440840 pocx-0.2.3/pocx/funcs/__init__.py
+-rw-r--r--   0        0        0     1821 2023-07-04 01:06:08.440840 pocx-0.2.3/pocx/funcs/ceye.py
+-rw-r--r--   0        0        0     4229 2023-07-04 01:06:08.440840 pocx-0.2.3/pocx/funcs/fofa.py
+-rw-r--r--   0        0        0     2598 2023-07-04 01:06:08.440840 pocx-0.2.3/pocx/funcs/snow_flake.py
+-rw-r--r--   0        0        0      789 2023-07-04 02:17:41.438670 pocx-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6713 1970-01-01 00:00:00.000000 pocx-0.2.3/PKG-INFO
```

### Comparing `pocx-0.2.2/LICENSE` & `pocx-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pocx-0.2.2/pocx/aio_poc.py` & `pocx-0.2.3/pocx/aio_poc.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,20 +23,31 @@
         self.cve = ''
         self.example = ''
         try:
             self.session = httpx.AsyncClient(verify=False)
         except Exception as e:
             self.session = httpx.AsyncClient(verify=ssl_context)
         self.session.headers = {"User-Agent": "Mozilla/5.0 (Windows NT 6.1; rv:2.0.1) Gecko/20100101 Firefox/4.0.1"}
+        self.headers = {"User-Agent": "Mozilla/5.0 (Windows NT 6.1; rv:2.0.1) Gecko/20100101 Firefox/4.0.1"}
         logger.info(f'Testing {self.name} with {self.mode}.')
 
     @logger.catch(level='ERROR')
     def set_headers(self, headers: dict = None):
         if headers is not None:
             self.session.headers = headers
+            self.headers = headers
+
+    @logger.catch(level='ERROR')
+    def set_proxies(self, proxies: dict = None):
+        if proxies is not None:
+            try:
+                self.session = httpx.AsyncClient(proxies=proxies, verify=False)
+            except Exception as e:
+                self.session = httpx.AsyncClient(proxies=proxies, verify=ssl_context)
+            self.session.headers = self.headers
 
     @logger.catch(level='ERROR')
     async def aio_request(self, url: str, method: str = 'get', timeout: int = 10, **kwargs) -> httpx.Response:
         try:
             resp = await self.session.request(method, url, timeout=timeout, **kwargs)
         except Exception:
             logger.error(f'[-] Run Poc [{self.cve} - {self.name}] Connection Error => {url} was not reachable.')
```

### Comparing `pocx-0.2.2/pocx/basic_poc.py` & `pocx-0.2.3/pocx/basic_poc.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,20 +22,31 @@
         self.cve = ''
         self.example = ''
         try:
             self.session = httpx.Client(verify=False)
         except Exception as e:
             self.session = httpx.Client(verify=ssl_context)
         self.session.headers = {"User-Agent": "Mozilla/5.0 (Windows NT 6.1; rv:2.0.1) Gecko/20100101 Firefox/4.0.1"}
+        self.headers = {"User-Agent": "Mozilla/5.0 (Windows NT 6.1; rv:2.0.1) Gecko/20100101 Firefox/4.0.1"}
         logger.info(f'Testing {self.name} with {self.mode}.')
 
     @logger.catch(level='ERROR')
     def set_headers(self, headers: dict = None):
         if headers is not None:
             self.session.headers = headers
+            self.headers = headers
+
+    @logger.catch(level='ERROR')
+    def set_proxies(self, proxies: dict = None):
+        if proxies is not None:
+            try:
+                self.session = httpx.Client(proxies=proxies, verify=False)
+            except Exception as e:
+                self.session = httpx.Client(proxies=proxies, verify=ssl_context)
+            self.session.headers = self.headers
 
     @logger.catch(level='ERROR')
     def request(self, url: str, method: str = 'get', timeout: int = 10, **kwargs) -> httpx.Response:
         try:
             resp = self.session.request(method, url, timeout=timeout, **kwargs)
         except Exception:
             logger.error(f'[-] Run Poc [{self.cve} - {self.name}] Connection Error => {url} was not reachable.')
```

### Comparing `pocx-0.2.2/pocx/funcs/ceye.py` & `pocx-0.2.3/pocx/funcs/ceye.py`

 * *Files identical despite different names*

### Comparing `pocx-0.2.2/pocx/funcs/fofa.py` & `pocx-0.2.3/pocx/funcs/fofa.py`

 * *Files identical despite different names*

### Comparing `pocx-0.2.2/pocx/funcs/snow_flake.py` & `pocx-0.2.3/pocx/funcs/snow_flake.py`

 * *Files identical despite different names*

### Comparing `pocx-0.2.2/pyproject.toml` & `pocx-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "pocx"
-version = "0.2.2"
+version = "0.2.3"
 description = "A Simple, Fast and Powerful poc engine tools was built by antx, which support synchronous mode and asynchronous mode."
 authors = ["antx <wkaifeng2007@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/antx-code/pocx"
 repository = "https://github.com/antx-code/pocx"
 keywords = ["async", "poc", "engine", "pocx"]
 
 [[tool.poetry.source]]
 name = "aliyun"
 url = "https://mirrors.aliyun.com/pypi/simple"
-default = true
+priority = "primary"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-httpx = "^0.22.0"
-loguru = "^0.6.0"
 urllib3 = "^1.26.9"
+httpx = "^0.24.1"
+loguru = "^0.7.0"
 
 [tool.poetry.dev-dependencies]
-httpx = "^0.22.0"
-loguru = "^0.6.0"
 urllib3 = "^1.26.9"
+httpx = "^0.24.1"
+loguru = "^0.7.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

