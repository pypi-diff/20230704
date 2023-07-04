# Comparing `tmp/zamg-0.2.3.tar.gz` & `tmp/zamg-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zamg-0.2.3.tar", max compression
+gzip compressed data, was "zamg-0.2.4.tar", max compression
```

## Comparing `zamg-0.2.3.tar` & `zamg-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-02-23 21:13:58.662751 zamg-0.2.3/LICENSE
--rw-r--r--   0        0        0     4096 2023-02-23 21:13:58.662751 zamg-0.2.3/README.md
--rw-r--r--   0        0        0     4088 2023-02-23 21:13:58.662751 zamg-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      470 2023-02-23 21:13:58.662751 zamg-0.2.3/src/zamg/__init__.py
--rw-r--r--   0        0        0      400 2023-02-23 21:13:58.662751 zamg-0.2.3/src/zamg/exceptions.py
--rw-r--r--   0        0        0    10041 2023-02-23 21:13:58.662751 zamg-0.2.3/src/zamg/zamg.py
--rw-r--r--   0        0        0     5551 1970-01-01 00:00:00.000000 zamg-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-04 18:52:34.639735 zamg-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4096 2023-07-04 18:52:34.639735 zamg-0.2.4/README.md
+-rw-r--r--   0        0        0     4086 2023-07-04 18:52:34.639735 zamg-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      470 2023-07-04 18:52:34.639735 zamg-0.2.4/src/zamg/__init__.py
+-rw-r--r--   0        0        0      400 2023-07-04 18:52:34.639735 zamg-0.2.4/src/zamg/exceptions.py
+-rw-r--r--   0        0        0    10053 2023-07-04 18:52:34.639735 zamg-0.2.4/src/zamg/zamg.py
+-rw-r--r--   0        0        0     5352 1970-01-01 00:00:00.000000 zamg-0.2.4/PKG-INFO
```

### Comparing `zamg-0.2.3/LICENSE` & `zamg-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zamg-0.2.3/README.md` & `zamg-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `zamg-0.2.3/pyproject.toml` & `zamg-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zamg"
-version = "0.2.3"
+version = "0.2.4"
 description = "Asynchronous Python client for ZAMG weather data."
 authors = ["Daniel Gangl <killer007@gmx.at>"]
 maintainers = ["Daniel Gangl <killer007@gmx.at>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/killer0071234/python-zamg"
 repository = "https://github.com/killer0071234/python-zamg"
@@ -29,19 +29,19 @@
 python = "^3.8"
 aiohttp = ">=3.8.0"
 
 [tool.poetry.dev-dependencies]
 aresponses = "^2.1.5"
 black = "^22.6"
 blacken-docs = "^1.12.1"
-coverage = {version = "^6.3", extras = ["toml"]}
+coverage = {version = "^7.2", extras = ["toml"]}
 flake8 = "^4.0.1"
 flake8-docstrings = "^1.5.0"
 isort = "^5.10.1"
-mypy = "^0.971"
+mypy = "^1.3"
 pre-commit = "^2.19.0"
 pre-commit-hooks = "^4.2.0"
 pylint = "^2.13.9"
 pytest = "^7.1.2"
 pytest-asyncio = "^0.20.1"
 pytest-cov = "^3.0.0"
 yamllint = "^1.26.3"
```

### Comparing `zamg-0.2.3/src/zamg/zamg.py` & `zamg-0.2.4/src/zamg/zamg.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,19 +73,19 @@
         try:
             if self.session is None:
                 self.session = aiohttp.client.ClientSession()
 
             async with async_timeout.timeout(self.request_timeout):
                 response = await self.session.get(
                     url=self.dataset_metadata_url,
-                    allow_redirects=False,
+                    allow_redirects=True,
                     headers=self.headers,
                     verify_ssl=self.verify_ssl,
                 )
-            if response.status == 200:
+            if response.status in (200, 301):
                 contents = await response.read()
                 response.close()
                 # extract all possible parameters
                 parameter_list = json.loads(contents)["parameters"]
                 station_parameters = ""
                 for parameter in parameter_list:
                     station_parameters += parameter["name"] + ","
@@ -206,19 +206,19 @@
 
             async with async_timeout.timeout(self.request_timeout):
                 response = await self.session.get(
                     url=self.dataset_data_url
                     + self.station_parameters
                     + "&station_ids="
                     + str(self._station_id),
-                    allow_redirects=False,
+                    allow_redirects=True,
                     headers=self.headers,
                     verify_ssl=self.verify_ssl,
                 )
-            if response.status == 200:
+            if response.status in (200, 301):
                 contents = await response.read()
                 response.close()
 
                 observations = json.loads(contents)["features"][0]["properties"][
                     "parameters"
                 ]
```

### Comparing `zamg-0.2.3/PKG-INFO` & `zamg-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zamg
-Version: 0.2.3
+Version: 0.2.4
 Summary: Asynchronous Python client for ZAMG weather data.
 Home-page: https://github.com/killer0071234/python-zamg
 License: MIT
 Keywords: zamg,api,async,client
 Author: Daniel Gangl
 Author-email: killer007@gmx.at
 Maintainer: Daniel Gangl
@@ -16,18 +16,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.8.0)
 Project-URL: Bug Tracker, https://github.com/killer0071234/python-zamg/issues
 Project-URL: Changelog, https://github.com/killer0071234/python-zamg/releases
 Project-URL: Documentation, https://github.com/killer0071234/python-zamg
 Project-URL: Repository, https://github.com/killer0071234/python-zamg
 Description-Content-Type: text/markdown
```

