# Comparing `tmp/ytdld-0.0.2.tar.gz` & `tmp/ytdld-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdld-0.0.2.tar", max compression
+gzip compressed data, was "ytdld-0.0.3.tar", max compression
```

## Comparing `ytdld-0.0.2.tar` & `ytdld-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2023-07-04 03:34:15.085856 ytdld-0.0.2/LICENSE
--rw-r--r--   0        0        0     2649 2023-07-04 11:01:18.880854 ytdld-0.0.2/README.md
--rw-r--r--   0        0        0      614 2023-07-04 10:57:26.364162 ytdld-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    10831 2023-07-04 11:00:09.116074 ytdld-0.0.2/ytdld.py
--rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 ytdld-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-04 03:34:15.085856 ytdld-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2649 2023-07-04 11:01:18.880854 ytdld-0.0.3/README.md
+-rw-r--r--   0        0        0      615 2023-07-04 11:08:37.977173 ytdld-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    10831 2023-07-04 11:00:09.116074 ytdld-0.0.3/ytdld.py
+-rw-r--r--   0        0        0     3322 1970-01-01 00:00:00.000000 ytdld-0.0.3/PKG-INFO
```

### Comparing `ytdld-0.0.2/LICENSE` & `ytdld-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdld-0.0.2/README.md` & `ytdld-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ytdld-0.0.2/pyproject.toml` & `ytdld-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,26 @@
     "setuptools>=58.0.4",
     "wheel>=0.37.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "ytdld"
-version = "0.0.2"
+version = "0.0.3"
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/KasRoudra/ytdld/"
 include = ["README.md", "LICENSE", "ytdld.py"]
 description = "Just another youtube downloader"
 authors = ["KasRoudra <kasroudrakrd@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pytube = "^14.0.0"
-questionary = "^1.9.0"
+pytube = "^15.0.0"
+questionary = "^1.10.0"
 
 [tool.poetry.scripts]
 ytdld = "ytdld:main"
 
 [build-system.sdist]
 formats = ["gztar"]
```

### Comparing `ytdld-0.0.2/ytdld.py` & `ytdld-0.0.3/ytdld.py`

 * *Files identical despite different names*

### Comparing `ytdld-0.0.2/PKG-INFO` & `ytdld-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ytdld
-Version: 0.0.2
+Version: 0.0.3
 Summary: Just another youtube downloader
 Home-page: https://github.com/KasRoudra/ytdld/
 License: MIT
 Author: KasRoudra
 Author-email: kasroudrakrd@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pytube (>=14.0.0,<15.0.0)
-Requires-Dist: questionary (>=1.9.0,<2.0.0)
+Requires-Dist: pytube (>=15.0.0,<16.0.0)
+Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Project-URL: Repository, https://github.com/KasRoudra/ytdld/
 Description-Content-Type: text/markdown
 
 # YT-DLD
 
 ### Just another youtube downloader
```

