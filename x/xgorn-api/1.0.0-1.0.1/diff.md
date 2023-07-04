# Comparing `tmp/xgorn-api-1.0.0.tar.gz` & `tmp/xgorn-api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgorn-api-1.0.0.tar", last modified: Tue Jul  4 00:29:23 2023, max compression
+gzip compressed data, was "xgorn-api-1.0.1.tar", last modified: Tue Jul  4 03:12:10 2023, max compression
```

## Comparing `xgorn-api-1.0.0.tar` & `xgorn-api-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 00:29:23.077854 xgorn-api-1.0.0/
--rw-rw-rw-   0        0        0     1475 2023-07-04 00:29:23.076854 xgorn-api-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-04 00:26:52.000000 xgorn-api-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 00:29:23.078852 xgorn-api-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1722 2023-07-04 00:28:41.000000 xgorn-api-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 00:29:22.955844 xgorn-api-1.0.0/xgorn_api/
--rw-rw-rw-   0        0        0       49 2023-07-03 23:51:06.000000 xgorn-api-1.0.0/xgorn_api/__init__.py
--rw-rw-rw-   0        0        0     3244 2023-07-04 00:19:18.000000 xgorn-api-1.0.0/xgorn_api/api.py
-drwxrwxrwx   0        0        0        0 2023-07-04 00:29:23.070851 xgorn-api-1.0.0/xgorn_api.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-07-04 00:29:22.000000 xgorn-api-1.0.0/xgorn_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-07-04 00:29:22.000000 xgorn-api-1.0.0/xgorn_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 00:29:22.000000 xgorn-api-1.0.0/xgorn_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-04 00:29:22.000000 xgorn-api-1.0.0/xgorn_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-04 00:29:22.000000 xgorn-api-1.0.0/xgorn_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:12:10.586305 xgorn-api-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-04 03:11:40.000000 xgorn-api-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-04 03:12:10.586305 xgorn-api-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-04 03:11:40.000000 xgorn-api-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 03:12:10.586305 xgorn-api-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-04 03:11:40.000000 xgorn-api-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:12:10.586305 xgorn-api-1.0.1/xgorn_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-04 03:11:40.000000 xgorn-api-1.0.1/xgorn_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-04 03:11:40.000000 xgorn-api-1.0.1/xgorn_api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:12:10.586305 xgorn-api-1.0.1/xgorn_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-04 03:12:10.000000 xgorn-api-1.0.1/xgorn_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-04 03:12:10.000000 xgorn-api-1.0.1/xgorn_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 03:12:10.000000 xgorn-api-1.0.1/xgorn_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 03:12:10.000000 xgorn-api-1.0.1/xgorn_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 03:12:10.000000 xgorn-api-1.0.1/xgorn_api.egg-info/top_level.txt
```

### Comparing `xgorn-api-1.0.0/PKG-INFO` & `xgorn-api-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,47 @@
-Metadata-Version: 2.1
-Name: xgorn-api
-Version: 1.0.0
-Summary: API Interface for https://api.xgorn.pp.ua
-Home-page: https://api.xgorn.pp.ua
-Author: xgorn
-License: MIT
-Project-URL: Web, https://api.xgorn.pp.ua
-Project-URL: Documentation, https://api.xgorn.pp.ua/docs
-Keywords: api scraper bypasser translator client library python
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-
-# Noid API
-
-```python
-from xgorn_api import NoidAPI
-
-api = NoidAPI()
-api.api_key = 'your-api-key'
-
-api.ouo_bypass('https://ouo.io/4ZuwGMc')
-```
-
-**Everything** are based on the documentation!
-
-## Installation
-
-```
-pip install xgorn-api
-```
-
-
+Metadata-Version: 2.1
+Name: xgorn-api
+Version: 1.0.1
+Summary: API Interface for https://api.xgorn.pp.ua
+Home-page: https://github.com/api-xgorn-docs
+Author: xgorn
+License: MIT
+Project-URL: Web, https://api.xgorn.pp.ua
+Project-URL: Documentation, https://api.xgorn.pp.ua/docs
+Keywords: api scraper bypasser translator client library python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Noid API
+
+```python
+from xgorn_api import NoidAPI
+
+api = NoidAPI()
+api.api_key = 'your-api-key'
+
+api.ouo_bypass('https://ouo.io/4ZuwGMc')
+```
+
+**Everything** are based on the documentation!
+
+## Installation
+
+```
+pip install xgorn-api
+```
```

### Comparing `xgorn-api-1.0.0/xgorn_api.egg-info/PKG-INFO` & `xgorn-api-1.0.1/xgorn_api.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,47 @@
-Metadata-Version: 2.1
-Name: xgorn-api
-Version: 1.0.0
-Summary: API Interface for https://api.xgorn.pp.ua
-Home-page: https://api.xgorn.pp.ua
-Author: xgorn
-License: MIT
-Project-URL: Web, https://api.xgorn.pp.ua
-Project-URL: Documentation, https://api.xgorn.pp.ua/docs
-Keywords: api scraper bypasser translator client library python
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-
-# Noid API
-
-```python
-from xgorn_api import NoidAPI
-
-api = NoidAPI()
-api.api_key = 'your-api-key'
-
-api.ouo_bypass('https://ouo.io/4ZuwGMc')
-```
-
-**Everything** are based on the documentation!
-
-## Installation
-
-```
-pip install xgorn-api
-```
-
-
+Metadata-Version: 2.1
+Name: xgorn-api
+Version: 1.0.1
+Summary: API Interface for https://api.xgorn.pp.ua
+Home-page: https://github.com/api-xgorn-docs
+Author: xgorn
+License: MIT
+Project-URL: Web, https://api.xgorn.pp.ua
+Project-URL: Documentation, https://api.xgorn.pp.ua/docs
+Keywords: api scraper bypasser translator client library python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Noid API
+
+```python
+from xgorn_api import NoidAPI
+
+api = NoidAPI()
+api.api_key = 'your-api-key'
+
+api.ouo_bypass('https://ouo.io/4ZuwGMc')
+```
+
+**Everything** are based on the documentation!
+
+## Installation
+
+```
+pip install xgorn-api
+```
```

