# Comparing `tmp/ra2mix-0.0.6.tar.gz` & `tmp/ra2mix-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ra2mix-0.0.6.tar", last modified: Mon Jul  3 01:04:28 2023, max compression
+gzip compressed data, was "ra2mix-0.0.7.tar", last modified: Mon Jul  3 22:06:27 2023, max compression
```

## Comparing `ra2mix-0.0.6.tar` & `ra2mix-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:04:28.823609 ra2mix-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 01:04:19.000000 ra2mix-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-03 01:04:28.823609 ra2mix-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-03 01:04:19.000000 ra2mix-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 01:04:19.000000 ra2mix-0.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:04:28.823609 ra2mix-0.0.6/ra2mix/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 01:04:19.000000 ra2mix-0.0.6/ra2mix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-03 01:04:19.000000 ra2mix-0.0.6/ra2mix/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-03 01:04:19.000000 ra2mix-0.0.6/ra2mix/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-03 01:04:19.000000 ra2mix-0.0.6/ra2mix/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-03 01:04:19.000000 ra2mix-0.0.6/ra2mix/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:04:28.823609 ra2mix-0.0.6/ra2mix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-03 01:04:28.000000 ra2mix-0.0.6/ra2mix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 01:04:28.000000 ra2mix-0.0.6/ra2mix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:04:28.000000 ra2mix-0.0.6/ra2mix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-03 01:04:28.000000 ra2mix-0.0.6/ra2mix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 01:04:28.000000 ra2mix-0.0.6/ra2mix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 01:04:28.823609 ra2mix-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:06:27.561769 ra2mix-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 22:06:16.000000 ra2mix-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-03 22:06:27.561769 ra2mix-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-03 22:06:16.000000 ra2mix-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 22:06:16.000000 ra2mix-0.0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:06:27.557769 ra2mix-0.0.7/ra2mix/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 22:06:16.000000 ra2mix-0.0.7/ra2mix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-03 22:06:16.000000 ra2mix-0.0.7/ra2mix/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-03 22:06:16.000000 ra2mix-0.0.7/ra2mix/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-03 22:06:16.000000 ra2mix-0.0.7/ra2mix/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-03 22:06:16.000000 ra2mix-0.0.7/ra2mix/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:06:27.561769 ra2mix-0.0.7/ra2mix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-03 22:06:27.000000 ra2mix-0.0.7/ra2mix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 22:06:27.000000 ra2mix-0.0.7/ra2mix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:06:27.000000 ra2mix-0.0.7/ra2mix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-03 22:06:27.000000 ra2mix-0.0.7/ra2mix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 22:06:27.000000 ra2mix-0.0.7/ra2mix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:06:27.561769 ra2mix-0.0.7/setup.cfg
```

### Comparing `ra2mix-0.0.6/LICENSE` & `ra2mix-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ra2mix-0.0.6/pyproject.toml` & `ra2mix-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "ra2mix"
 authors = [
     {name = "nyte_owl", email = "nyteowldev@gmail.com"}
 ]
 description = "ra2mix is a python library for working with Red Alert 2 / Yuri's Revenge *.mix files"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
     "crc"
 ]
 classifiers = [
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

### Comparing `ra2mix-0.0.6/ra2mix/checksum.py` & `ra2mix-0.0.7/ra2mix/checksum.py`

 * *Files identical despite different names*

### Comparing `ra2mix-0.0.6/ra2mix/reader.py` & `ra2mix-0.0.7/ra2mix/reader.py`

 * *Files identical despite different names*

### Comparing `ra2mix-0.0.6/ra2mix/writer.py` & `ra2mix-0.0.7/ra2mix/writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,26 +88,26 @@
     flags = 0
     file_count = len(file_map)
     data_size = sum(len(data) for data in file_map.values())
 
     print(f"Writing {file_count} files to mix file; total size = {data_size}")
 
     header = struct.pack("=I H I", flags, file_count, data_size)
-    print(f"Header: {header}")
 
     return header
 
 
 def write(
     mix_filepath: str | None,
     game: const.XCCGame = const.XCCGame.RA2,
     file_map: dict[str, bytes] | None = None,
     folder_path: str | None = None,
     filepaths: list[str] | None = None,
 ) -> bytes:
+    print("---")
     file_map = coalesce_input_files(game, file_map, folder_path, filepaths)
 
     file_information_list = [
         FileInfo(file_id=ra2_crc(filename), data=data)
         for filename, data in file_map.items()
     ]
     sorted_file_info_list = sorted(
```

