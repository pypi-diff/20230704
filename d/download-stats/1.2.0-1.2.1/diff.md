# Comparing `tmp/download_stats-1.2.0.tar.gz` & `tmp/download_stats-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "download_stats-1.2.0.tar", last modified: Sat Sep  3 05:03:52 2022, max compression
+gzip compressed data, was "download_stats-1.2.1.tar", last modified: Tue Jul  4 06:44:27 2023, max compression
```

## Comparing `download_stats-1.2.0.tar` & `download_stats-1.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-09-03 05:03:52.188094 download_stats-1.2.0/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    11357 2022-09-01 10:18:27.000000 download_stats-1.2.0/LICENSE
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      150 2022-09-02 19:00:31.000000 download_stats-1.2.0/MANIFEST.in
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3107 2022-09-03 05:03:52.188094 download_stats-1.2.0/PKG-INFO
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2340 2022-09-03 05:02:15.000000 download_stats-1.2.0/README.md
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-09-03 05:03:52.180094 download_stats-1.2.0/assets/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    15299 2022-09-02 20:45:26.000000 download_stats-1.2.0/assets/compare.png
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    68629 2022-09-02 18:34:09.000000 download_stats-1.2.0/assets/download_stats.png
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-09-03 05:03:52.180094 download_stats-1.2.0/reqs/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       55 2022-09-01 14:09:10.000000 download_stats-1.2.0/reqs/app.in
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1203 2022-09-02 18:56:22.000000 download_stats-1.2.0/reqs/app.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       22 2022-09-02 18:56:18.000000 download_stats-1.2.0/reqs/dev.in
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1840 2022-09-02 18:56:41.000000 download_stats-1.2.0/reqs/dev.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      217 2022-09-03 05:03:52.188094 download_stats-1.2.0/setup.cfg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3578 2022-09-03 05:02:50.000000 download_stats-1.2.0/setup.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-09-03 05:03:52.176094 download_stats-1.2.0/src/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-09-03 05:03:52.184094 download_stats-1.2.0/src/download_stats/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      170 2022-09-02 18:43:35.000000 download_stats-1.2.0/src/download_stats/__init__.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-09-03 05:03:52.188094 download_stats-1.2.0/src/download_stats/__pycache__/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      319 2022-09-02 18:44:30.000000 download_stats-1.2.0/src/download_stats/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2640 2022-09-03 04:54:32.000000 download_stats-1.2.0/src/download_stats/__pycache__/main.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2244 2022-09-03 04:59:43.000000 download_stats-1.2.0/src/download_stats/__pycache__/pepy.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1616 2022-09-02 17:53:23.000000 download_stats-1.2.0/src/download_stats/__pycache__/pypistats.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2812 2022-09-03 04:54:28.000000 download_stats-1.2.0/src/download_stats/main.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2216 2022-09-03 04:59:40.000000 download_stats-1.2.0/src/download_stats/pepy.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1790 2022-09-02 12:49:40.000000 download_stats-1.2.0/src/download_stats/pypistats.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-09-03 05:03:52.188094 download_stats-1.2.0/src/download_stats.egg-info/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3107 2022-09-03 05:03:52.000000 download_stats-1.2.0/src/download_stats.egg-info/PKG-INFO
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      731 2022-09-03 05:03:52.000000 download_stats-1.2.0/src/download_stats.egg-info/SOURCES.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        1 2022-09-03 05:03:52.000000 download_stats-1.2.0/src/download_stats.egg-info/dependency_links.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       60 2022-09-03 05:03:52.000000 download_stats-1.2.0/src/download_stats.egg-info/entry_points.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      410 2022-09-03 05:03:52.000000 download_stats-1.2.0/src/download_stats.egg-info/requires.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       15 2022-09-03 05:03:52.000000 download_stats-1.2.0/src/download_stats.egg-info/top_level.txt
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 06:44:27.139559 download_stats-1.2.1/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)    11357 2023-07-04 06:21:07.000000 download_stats-1.2.1/LICENSE
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      150 2023-07-04 06:21:07.000000 download_stats-1.2.1/MANIFEST.in
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     3162 2023-07-04 06:44:27.139559 download_stats-1.2.1/PKG-INFO
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2340 2023-07-04 06:21:07.000000 download_stats-1.2.1/README.md
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 06:44:27.135558 download_stats-1.2.1/assets/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)    15299 2023-07-04 06:21:07.000000 download_stats-1.2.1/assets/compare.png
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)    68629 2023-07-04 06:21:07.000000 download_stats-1.2.1/assets/download_stats.png
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 06:44:27.135558 download_stats-1.2.1/reqs/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       73 2023-07-04 06:39:03.000000 download_stats-1.2.1/reqs/app.in
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1331 2023-07-04 06:39:12.000000 download_stats-1.2.1/reqs/app.txt
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       22 2023-07-04 06:21:07.000000 download_stats-1.2.1/reqs/dev.in
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1840 2023-07-04 06:21:07.000000 download_stats-1.2.1/reqs/dev.txt
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      217 2023-07-04 06:44:27.143559 download_stats-1.2.1/setup.cfg
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     3578 2023-07-04 06:44:23.000000 download_stats-1.2.1/setup.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 06:44:27.135558 download_stats-1.2.1/src/
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 06:44:27.139559 download_stats-1.2.1/src/download_stats/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      170 2023-07-04 06:21:07.000000 download_stats-1.2.1/src/download_stats/__init__.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 06:44:27.139559 download_stats-1.2.1/src/download_stats/__pycache__/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      397 2023-07-04 06:27:00.000000 download_stats-1.2.1/src/download_stats/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     5795 2023-07-04 06:27:00.000000 download_stats-1.2.1/src/download_stats/__pycache__/main.cpython-311.pyc
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     4373 2023-07-04 06:34:45.000000 download_stats-1.2.1/src/download_stats/__pycache__/pepy.cpython-311.pyc
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2931 2023-07-04 06:27:00.000000 download_stats-1.2.1/src/download_stats/__pycache__/pypistats.cpython-311.pyc
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2812 2023-07-04 06:21:07.000000 download_stats-1.2.1/src/download_stats/main.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2352 2023-07-04 06:35:34.000000 download_stats-1.2.1/src/download_stats/pepy.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1790 2023-07-04 06:21:07.000000 download_stats-1.2.1/src/download_stats/pypistats.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 06:44:27.139559 download_stats-1.2.1/src/download_stats.egg-info/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     3162 2023-07-04 06:44:27.000000 download_stats-1.2.1/src/download_stats.egg-info/PKG-INFO
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      731 2023-07-04 06:44:27.000000 download_stats-1.2.1/src/download_stats.egg-info/SOURCES.txt
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        1 2023-07-04 06:44:27.000000 download_stats-1.2.1/src/download_stats.egg-info/dependency_links.txt
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       61 2023-07-04 06:44:27.000000 download_stats-1.2.1/src/download_stats.egg-info/entry_points.txt
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      444 2023-07-04 06:44:27.000000 download_stats-1.2.1/src/download_stats.egg-info/requires.txt
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       15 2023-07-04 06:44:27.000000 download_stats-1.2.1/src/download_stats.egg-info/top_level.txt
```

### Comparing `download_stats-1.2.0/LICENSE` & `download_stats-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `download_stats-1.2.0/PKG-INFO` & `download_stats-1.2.1/src/download_stats.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
-Name: download_stats
-Version: 1.2.0
+Name: download-stats
+Version: 1.2.1
 Summary: Download stats for Python packages
+Home-page: UNKNOWN
 Author-email: arj.python@gmail.com
+License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/Abdur-RahmaanJ/download-stats/issues
 Project-URL: Source, https://github.com/Abdur-RahmaanJ/download-stats/
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -121,7 +124,8 @@
         {"category": "Linux", "date": "2022-08-31", "downloads": 3},
     ],
     "package": "shopyo",
     "type": "system_downloads",
 }
 
 ```
+
```

### Comparing `download_stats-1.2.0/README.md` & `download_stats-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `download_stats-1.2.0/assets/compare.png` & `download_stats-1.2.1/assets/compare.png`

 * *Files identical despite different names*

### Comparing `download_stats-1.2.0/assets/download_stats.png` & `download_stats-1.2.1/assets/download_stats.png`

 * *Files identical despite different names*

### Comparing `download_stats-1.2.0/reqs/app.txt` & `download_stats-1.2.1/reqs/app.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.11
+# by the following command:
 #
 #    pip-compile --output-file=reqs/app.txt reqs/app.in
 #
+appdirs==1.4.4
+    # via latest-user-agents
 async-generator==1.10
     # via
     #   trio
     #   trio-websocket
 attrs==22.1.0
     # via
     #   outcome
@@ -16,33 +18,36 @@
     # via
     #   requests
     #   selenium
 charset-normalizer==2.1.1
     # via requests
 commonmark==0.9.1
     # via rich
-fake-useragent==0.1.11
-    # via -r reqs/app.in
 h11==0.13.0
     # via wsproto
 idna==3.3
     # via
     #   requests
     #   trio
+latest-user-agents==0.0.3
+    # via -r reqs/app.in
 outcome==1.2.0
     # via trio
+packaging==23.1
+    # via webdriver-manager
 pygments==2.13.0
     # via rich
 pysocks==1.7.1
     # via urllib3
 python-dotenv==0.20.0
     # via webdriver-manager
 requests==2.28.1
     # via
     #   -r reqs/app.in
+    #   latest-user-agents
     #   webdriver-manager
 rich==12.5.1
     # via -r reqs/app.in
 selenium==4.4.3
     # via -r reqs/app.in
 sniffio==1.3.0
     # via trio
@@ -56,11 +61,11 @@
     #   trio-websocket
 trio-websocket==0.9.2
     # via selenium
 urllib3[socks]==1.26.12
     # via
     #   requests
     #   selenium
-webdriver-manager==3.8.3
+webdriver-manager==3.8.6
     # via -r reqs/app.in
 wsproto==1.2.0
     # via trio-websocket
```

### Comparing `download_stats-1.2.0/reqs/dev.txt` & `download_stats-1.2.1/reqs/dev.txt`

 * *Files identical despite different names*

### Comparing `download_stats-1.2.0/setup.py` & `download_stats-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 setup(
     name="download_stats",  # Required
-    version="1.2.0",  # Required
+    version="1.2.1",  # Required
     description="Download stats for Python packages",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     # url="https://github.com/Abdur-RahmaanJ/greenBerry",  # Optional
     # author="Abdur-Rahmaan Janhangeer & contributors",  # Optional
     author_email="arj.python@gmail.com",  # Optional
     # Classifiers help users find your project by categorizing it.
```

### Comparing `download_stats-1.2.0/src/download_stats/main.py` & `download_stats-1.2.1/src/download_stats/main.py`

 * *Files identical despite different names*

### Comparing `download_stats-1.2.0/src/download_stats/pepy.py` & `download_stats-1.2.1/src/download_stats/pepy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from selenium.webdriver.chrome.service import Service
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.chrome.options import Options
 from selenium import webdriver
-from fake_useragent import UserAgent
+# from fake_useragent import UserAgent
+from latest_user_agents import get_random_user_agent
 from rich.console import Console
 import time
 import sys
 
 console = Console()
 
 
@@ -20,16 +21,19 @@
     options.add_argument("--window-size=1280,1280")
     options.add_argument("--no-sandbox")
     options.add_argument("--enable-javascript")
     options.add_experimental_option("excludeSwitches", ["enable-automation"])
     options.add_experimental_option('useAutomationExtension', False)
     options.add_argument('--disable-blink-features=AutomationControlled')
     driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()), options=options)
-    ua = UserAgent()
-    userAgent = ua.random
+    
+    #ua = UserAgent()
+    #ua = get_random_user_agent()
+    #userAgent = ua.random
+    userAgent = get_random_user_agent()
     driver.execute_script("Object.defineProperty(navigator, 'webdriver', {get: () => undefined})")
     driver.execute_cdp_cmd('Network.setUserAgentOverride', {"userAgent": userAgent})
     with console.status("[bold green]Getting content...") as status:
         driver.get(f'https://pepy.tech/project/{project}')
         time.sleep(5)
 
     try:
```

### Comparing `download_stats-1.2.0/src/download_stats/pypistats.py` & `download_stats-1.2.1/src/download_stats/pypistats.py`

 * *Files identical despite different names*

### Comparing `download_stats-1.2.0/src/download_stats.egg-info/PKG-INFO` & `download_stats-1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
-Name: download-stats
-Version: 1.2.0
+Name: download_stats
+Version: 1.2.1
 Summary: Download stats for Python packages
+Home-page: UNKNOWN
 Author-email: arj.python@gmail.com
+License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/Abdur-RahmaanJ/download-stats/issues
 Project-URL: Source, https://github.com/Abdur-RahmaanJ/download-stats/
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -121,7 +124,8 @@
         {"category": "Linux", "date": "2022-08-31", "downloads": 3},
     ],
     "package": "shopyo",
     "type": "system_downloads",
 }
 
 ```
+
```

### Comparing `download_stats-1.2.0/src/download_stats.egg-info/SOURCES.txt` & `download_stats-1.2.1/src/download_stats.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,11 +15,11 @@
 src/download_stats/pypistats.py
 src/download_stats.egg-info/PKG-INFO
 src/download_stats.egg-info/SOURCES.txt
 src/download_stats.egg-info/dependency_links.txt
 src/download_stats.egg-info/entry_points.txt
 src/download_stats.egg-info/requires.txt
 src/download_stats.egg-info/top_level.txt
-src/download_stats/__pycache__/__init__.cpython-310.pyc
-src/download_stats/__pycache__/main.cpython-310.pyc
-src/download_stats/__pycache__/pepy.cpython-310.pyc
-src/download_stats/__pycache__/pypistats.cpython-310.pyc
+src/download_stats/__pycache__/__init__.cpython-311.pyc
+src/download_stats/__pycache__/main.cpython-311.pyc
+src/download_stats/__pycache__/pepy.cpython-311.pyc
+src/download_stats/__pycache__/pypistats.cpython-311.pyc
```

