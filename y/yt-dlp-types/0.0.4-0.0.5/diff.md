# Comparing `tmp/yt_dlp_types-0.0.4.tar.gz` & `tmp/yt_dlp_types-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_dlp_types-0.0.4.tar", max compression
+gzip compressed data, was "yt_dlp_types-0.0.5.tar", max compression
```

## Comparing `yt_dlp_types-0.0.4.tar` & `yt_dlp_types-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1087 2023-07-03 15:46:20.349120 yt_dlp_types-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0      128 2023-07-03 19:42:09.982181 yt_dlp_types-0.0.4/README.md
--rw-r--r--   0        0        0      699 2023-07-03 20:28:16.295618 yt_dlp_types-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      513 2023-07-03 20:27:46.133664 yt_dlp_types-0.0.4/yt_dlp-stubs/YoutubeDL.pyi
--rw-r--r--   0        0        0    27804 2023-07-03 19:37:36.027414 yt_dlp_types-0.0.4/yt_dlp-stubs/__init__.pyi
--rw-r--r--   0        0        0      286 2023-07-03 19:24:37.015987 yt_dlp_types-0.0.4/yt_dlp-stubs/_misc.pyi
--rw-r--r--   0        0        0      588 2023-07-03 19:24:38.504986 yt_dlp_types-0.0.4/yt_dlp-stubs/cookies.pyi
--rw-r--r--   0        0        0        0 2023-07-03 19:24:30.422991 yt_dlp_types-0.0.4/yt_dlp-stubs/extractor/__init__.pyi
--rw-r--r--   0        0        0     1917 2023-07-03 19:24:31.719990 yt_dlp_types-0.0.4/yt_dlp-stubs/extractor/common.pyi
--rw-r--r--   0        0        0        0 2023-07-03 19:04:47.210090 yt_dlp_types-0.0.4/yt_dlp-stubs/py.typed
--rw-r--r--   0        0        0       22 2023-07-03 19:24:33.389989 yt_dlp_types-0.0.4/yt_dlp-stubs/utils/__init__.pyi
--rw-r--r--   0        0        0     1178 2023-07-03 19:24:34.339989 yt_dlp_types-0.0.4/yt_dlp-stubs/utils/_utils.pyi
--rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 yt_dlp_types-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-07-03 15:46:20.349120 yt_dlp_types-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      128 2023-07-03 19:42:09.982181 yt_dlp_types-0.0.5/README.md
+-rw-r--r--   0        0        0      699 2023-07-04 00:02:04.258417 yt_dlp_types-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-07-03 20:27:46.133664 yt_dlp_types-0.0.5/yt_dlp-stubs/YoutubeDL.pyi
+-rw-r--r--   0        0        0    27804 2023-07-03 19:37:36.027414 yt_dlp_types-0.0.5/yt_dlp-stubs/__init__.pyi
+-rw-r--r--   0        0        0      286 2023-07-03 19:24:37.015987 yt_dlp_types-0.0.5/yt_dlp-stubs/_misc.pyi
+-rw-r--r--   0        0        0      588 2023-07-03 19:24:38.504986 yt_dlp_types-0.0.5/yt_dlp-stubs/cookies.pyi
+-rw-r--r--   0        0        0        0 2023-07-03 19:24:30.422991 yt_dlp_types-0.0.5/yt_dlp-stubs/extractor/__init__.pyi
+-rw-r--r--   0        0        0     1917 2023-07-03 19:24:31.719990 yt_dlp_types-0.0.5/yt_dlp-stubs/extractor/common.pyi
+-rw-r--r--   0        0        0        0 2023-07-03 19:04:47.210090 yt_dlp_types-0.0.5/yt_dlp-stubs/py.typed
+-rw-r--r--   0        0        0       22 2023-07-03 19:24:33.389989 yt_dlp_types-0.0.5/yt_dlp-stubs/utils/__init__.pyi
+-rw-r--r--   0        0        0     1310 2023-07-04 00:01:26.911435 yt_dlp_types-0.0.5/yt_dlp-stubs/utils/_utils.pyi
+-rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 yt_dlp_types-0.0.5/PKG-INFO
```

### Comparing `yt_dlp_types-0.0.4/LICENSE.txt` & `yt_dlp_types-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yt_dlp_types-0.0.4/pyproject.toml` & `yt_dlp_types-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 authors = ["Andrew Udvare <audvare@gmail.com>"]
 classifiers = ['Typing :: Typed']
 description = "Typing stubs for yt-dlp"
 license = "MIT"
 name = "yt-dlp-types"
 packages = [{ include = "yt_dlp-stubs" }]
 readme = "README.md"
-version = "0.0.4"
+version = "0.0.5"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `yt_dlp_types-0.0.4/yt_dlp-stubs/YoutubeDL.pyi` & `yt_dlp_types-0.0.5/yt_dlp-stubs/YoutubeDL.pyi`

 * *Files identical despite different names*

### Comparing `yt_dlp_types-0.0.4/yt_dlp-stubs/__init__.pyi` & `yt_dlp_types-0.0.5/yt_dlp-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `yt_dlp_types-0.0.4/yt_dlp-stubs/cookies.pyi` & `yt_dlp_types-0.0.5/yt_dlp-stubs/cookies.pyi`

 * *Files identical despite different names*

### Comparing `yt_dlp_types-0.0.4/yt_dlp-stubs/extractor/common.pyi` & `yt_dlp_types-0.0.5/yt_dlp-stubs/extractor/common.pyi`

 * *Files identical despite different names*

### Comparing `yt_dlp_types-0.0.4/PKG-INFO` & `yt_dlp_types-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-dlp-types
-Version: 0.0.4
+Version: 0.0.5
 Summary: Typing stubs for yt-dlp
 License: MIT
 Author: Andrew Udvare
 Author-email: audvare@gmail.com
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

