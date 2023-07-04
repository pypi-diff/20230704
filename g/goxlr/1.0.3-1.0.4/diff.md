# Comparing `tmp/goxlr-1.0.3.tar.gz` & `tmp/goxlr-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlr-1.0.3.tar", last modified: Tue Jul  4 11:26:49 2023, max compression
+gzip compressed data, was "goxlr-1.0.4.tar", last modified: Tue Jul  4 16:04:15 2023, max compression
```

## Comparing `goxlr-1.0.3.tar` & `goxlr-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 11:26:49.834499 goxlr-1.0.3/
--rw-rw-rw-   0        0        0     1089 2023-07-04 11:05:46.000000 goxlr-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2278 2023-07-04 11:26:49.834499 goxlr-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1938 2023-07-04 11:26:03.000000 goxlr-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 11:26:49.830495 goxlr-1.0.3/goxlr/
--rw-rw-rw-   0        0        0       26 2023-07-03 21:36:56.000000 goxlr-1.0.3/goxlr/__init__.py
--rw-rw-rw-   0        0        0       41 2023-07-03 22:14:52.000000 goxlr-1.0.3/goxlr/error.py
--rw-rw-rw-   0        0        0    27172 2023-07-04 01:14:35.000000 goxlr-1.0.3/goxlr/goxlr.py
--rw-rw-rw-   0        0        0    11669 2023-07-04 00:56:11.000000 goxlr-1.0.3/goxlr/types.py
--rw-rw-rw-   0        0        0     2171 2023-07-03 22:52:03.000000 goxlr-1.0.3/goxlr/ws.py
-drwxrwxrwx   0        0        0        0 2023-07-04 11:26:49.833996 goxlr-1.0.3/goxlr.egg-info/
--rw-rw-rw-   0        0        0     2278 2023-07-04 11:26:49.000000 goxlr-1.0.3/goxlr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-07-04 11:26:49.000000 goxlr-1.0.3/goxlr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 11:26:49.000000 goxlr-1.0.3/goxlr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-04 11:26:49.000000 goxlr-1.0.3/goxlr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-04 11:26:49.000000 goxlr-1.0.3/goxlr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-04 11:26:49.834996 goxlr-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      534 2023-07-04 11:26:25.000000 goxlr-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 16:04:15.638918 goxlr-1.0.4/
+-rw-rw-rw-   0        0        0     1089 2023-07-04 11:05:46.000000 goxlr-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2218 2023-07-04 16:04:15.639419 goxlr-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1901 2023-07-04 16:00:21.000000 goxlr-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 16:04:15.633916 goxlr-1.0.4/goxlr/
+-rw-rw-rw-   0        0        0       26 2023-07-03 21:36:56.000000 goxlr-1.0.4/goxlr/__init__.py
+-rw-rw-rw-   0        0        0       41 2023-07-03 22:14:52.000000 goxlr-1.0.4/goxlr/error.py
+-rw-rw-rw-   0        0        0    27172 2023-07-04 01:14:35.000000 goxlr-1.0.4/goxlr/goxlr.py
+-rw-rw-rw-   0        0        0    11669 2023-07-04 00:56:11.000000 goxlr-1.0.4/goxlr/types.py
+-rw-rw-rw-   0        0        0     2171 2023-07-03 22:52:03.000000 goxlr-1.0.4/goxlr/ws.py
+drwxrwxrwx   0        0        0        0 2023-07-04 16:04:15.637917 goxlr-1.0.4/goxlr.egg-info/
+-rw-rw-rw-   0        0        0     2218 2023-07-04 16:04:15.000000 goxlr-1.0.4/goxlr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-07-04 16:04:15.000000 goxlr-1.0.4/goxlr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 16:04:15.000000 goxlr-1.0.4/goxlr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-04 16:04:15.000000 goxlr-1.0.4/goxlr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-04 16:04:15.000000 goxlr-1.0.4/goxlr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-07-04 15:57:33.000000 goxlr-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-04 16:04:15.639918 goxlr-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      508 2023-07-04 15:59:27.000000 goxlr-1.0.4/setup.py
```

### Comparing `goxlr-1.0.3/LICENSE.txt` & `goxlr-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.0.3/PKG-INFO` & `goxlr-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # GoXLR Utility API Python Wrapper
 
  [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/goxlr.svg)](https://badge.fury.io/py/goxlr) ![PyPI - Downloads](https://img.shields.io/pypi/dm/goxlr) ![GitHub issues](https://img.shields.io/github/issues/samcarsonx/goxlr)
@@ -29,15 +28,14 @@
 ```
 
 ## Getting Started
 Here's some sample code to get started with this package that pings the utility's daemon.
 ```py
 import asyncio
 from goxlr import GoXLR
-from goxlr.types import ChannelName
 
 async def main():
     async with GoXLR() as xlr:
         print(await xlr.ping())
 
 if __name__ == "__main__":
     asyncio.run(main())
@@ -52,9 +50,7 @@
 ```
 
 ## Documentation
 Coming soon. For now, please refer to [goxlr.py](https://github.com/samcarsonx/goxlr/blob/main/goxlr/goxlr.py) to see all of the daemon and GoXLR commands, and refer to [types.py](https://github.com/samcarsonx/goxlr/blob/main/goxlr/types.py) to see all of the enums. You may find it very useful to have an IntelliSense-style plugin in your IDE.
 
 ## Contributing
 Coming soon. As there isn't a CONTRIBUTING.md yet, please try to emulate the style of the rest of the code. Using snake_case and descriptive method argument names with type hints wherever possible.
-
-
```

### Comparing `goxlr-1.0.3/README.md` & `goxlr-1.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 ```
 
 ## Getting Started
 Here's some sample code to get started with this package that pings the utility's daemon.
 ```py
 import asyncio
 from goxlr import GoXLR
-from goxlr.types import ChannelName
 
 async def main():
     async with GoXLR() as xlr:
         print(await xlr.ping())
 
 if __name__ == "__main__":
     asyncio.run(main())
```

### Comparing `goxlr-1.0.3/goxlr/goxlr.py` & `goxlr-1.0.4/goxlr/goxlr.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.0.3/goxlr/types.py` & `goxlr-1.0.4/goxlr/types.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.0.3/goxlr/ws.py` & `goxlr-1.0.4/goxlr/ws.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.0.3/goxlr.egg-info/PKG-INFO` & `goxlr-1.0.4/goxlr.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # GoXLR Utility API Python Wrapper
 
  [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/goxlr.svg)](https://badge.fury.io/py/goxlr) ![PyPI - Downloads](https://img.shields.io/pypi/dm/goxlr) ![GitHub issues](https://img.shields.io/github/issues/samcarsonx/goxlr)
@@ -29,15 +28,14 @@
 ```
 
 ## Getting Started
 Here's some sample code to get started with this package that pings the utility's daemon.
 ```py
 import asyncio
 from goxlr import GoXLR
-from goxlr.types import ChannelName
 
 async def main():
     async with GoXLR() as xlr:
         print(await xlr.ping())
 
 if __name__ == "__main__":
     asyncio.run(main())
@@ -52,9 +50,7 @@
 ```
 
 ## Documentation
 Coming soon. For now, please refer to [goxlr.py](https://github.com/samcarsonx/goxlr/blob/main/goxlr/goxlr.py) to see all of the daemon and GoXLR commands, and refer to [types.py](https://github.com/samcarsonx/goxlr/blob/main/goxlr/types.py) to see all of the enums. You may find it very useful to have an IntelliSense-style plugin in your IDE.
 
 ## Contributing
 Coming soon. As there isn't a CONTRIBUTING.md yet, please try to emulate the style of the rest of the code. Using snake_case and descriptive method argument names with type hints wherever possible.
-
-
```

