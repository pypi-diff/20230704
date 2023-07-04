# Comparing `tmp/libarchive-c-4.0.tar.gz` & `tmp/libarchive-c-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libarchive-c-4.0.tar", last modified: Sat Jan 22 17:34:08 2022, max compression
+gzip compressed data, was "libarchive-c-5.0.tar", last modified: Tue Jul  4 08:24:25 2023, max compression
```

## Comparing `libarchive-c-4.0.tar` & `libarchive-c-5.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 changaco  (1142) users      (100)        0 2022-01-22 17:34:08.467252 libarchive-c-4.0/
--rw-r--r--   0 changaco  (1142) users      (100)       25 2016-11-29 18:03:26.000000 libarchive-c-4.0/.gitattributes
-drwxr-xr-x   0 changaco  (1142) users      (100)        0 2022-01-22 17:34:08.463919 libarchive-c-4.0/.github/
--rw-r--r--   0 changaco  (1142) users      (100)       20 2021-05-24 14:29:37.000000 libarchive-c-4.0/.github/FUNDING.yml
-drwxr-xr-x   0 changaco  (1142) users      (100)        0 2022-01-22 17:34:08.463919 libarchive-c-4.0/.github/workflows/
--rw-r--r--   0 changaco  (1142) users      (100)      877 2022-01-22 17:28:18.000000 libarchive-c-4.0/.github/workflows/main.yml
--rw-r--r--   0 changaco  (1142) users      (100)       65 2016-11-29 18:03:29.000000 libarchive-c-4.0/.gitignore
--rw-r--r--   0 changaco  (1142) users      (100)       51 2018-06-10 12:43:23.000000 libarchive-c-4.0/LICENSE.md
--rw-r--r--   0 changaco  (1142) users      (100)       19 2016-11-29 18:03:22.000000 libarchive-c-4.0/MANIFEST.in
--rw-r--r--   0 changaco  (1142) users      (100)     4728 2022-01-22 17:34:08.470586 libarchive-c-4.0/PKG-INFO
--rw-r--r--   0 changaco  (1142) users      (100)     4377 2022-01-22 17:28:18.000000 libarchive-c-4.0/README.rst
-drwxr-xr-x   0 changaco  (1142) users      (100)        0 2022-01-22 17:34:08.463919 libarchive-c-4.0/libarchive/
--rw-r--r--   0 changaco  (1142) users      (100)      601 2021-05-24 15:08:51.000000 libarchive-c-4.0/libarchive/__init__.py
--rw-r--r--   0 changaco  (1142) users      (100)    12807 2022-01-22 17:28:18.000000 libarchive-c-4.0/libarchive/entry.py
--rw-r--r--   0 changaco  (1142) users      (100)      370 2021-05-24 15:09:05.000000 libarchive-c-4.0/libarchive/exception.py
--rw-r--r--   0 changaco  (1142) users      (100)     2694 2022-01-22 17:28:18.000000 libarchive-c-4.0/libarchive/extract.py
--rw-r--r--   0 changaco  (1142) users      (100)    12247 2022-01-22 17:28:18.000000 libarchive-c-4.0/libarchive/ffi.py
--rw-r--r--   0 changaco  (1142) users      (100)      211 2018-06-10 13:27:14.000000 libarchive-c-4.0/libarchive/flags.py
--rw-r--r--   0 changaco  (1142) users      (100)     5514 2022-01-22 17:28:18.000000 libarchive-c-4.0/libarchive/read.py
--rw-r--r--   0 changaco  (1142) users      (100)     9900 2022-01-22 17:28:18.000000 libarchive-c-4.0/libarchive/write.py
-drwxr-xr-x   0 changaco  (1142) users      (100)        0 2022-01-22 17:34:08.467252 libarchive-c-4.0/libarchive_c.egg-info/
--rw-r--r--   0 changaco  (1142) users      (100)     4728 2022-01-22 17:34:08.000000 libarchive-c-4.0/libarchive_c.egg-info/PKG-INFO
--rw-r--r--   0 changaco  (1142) users      (100)     1010 2022-01-22 17:34:08.000000 libarchive-c-4.0/libarchive_c.egg-info/SOURCES.txt
--rw-r--r--   0 changaco  (1142) users      (100)        1 2022-01-22 17:34:08.000000 libarchive-c-4.0/libarchive_c.egg-info/dependency_links.txt
--rw-r--r--   0 changaco  (1142) users      (100)       11 2022-01-22 17:34:08.000000 libarchive-c-4.0/libarchive_c.egg-info/top_level.txt
--rw-r--r--   0 changaco  (1142) users      (100)      136 2022-01-22 17:34:08.470586 libarchive-c-4.0/setup.cfg
--rw-r--r--   0 changaco  (1142) users      (100)      617 2019-11-22 09:30:52.000000 libarchive-c-4.0/setup.py
-drwxr-xr-x   0 changaco  (1142) users      (100)        0 2022-01-22 17:34:08.467252 libarchive-c-4.0/tests/
--rw-r--r--   0 changaco  (1142) users      (100)     4297 2021-05-24 15:09:05.000000 libarchive-c-4.0/tests/__init__.py
-drwxr-xr-x   0 changaco  (1142) users      (100)        0 2022-01-22 17:34:08.467252 libarchive-c-4.0/tests/data/
--rw-r--r--   0 changaco  (1142) users      (100)    10240 2018-06-10 11:44:59.000000 libarchive-c-4.0/tests/data/flags.tar
--rw-r--r--   0 changaco  (1142) users      (100)   112640 2016-11-29 18:03:26.000000 libarchive-c-4.0/tests/data/special.tar
--rw-r--r--   0 changaco  (1142) users      (100)    10240 2016-11-29 18:03:26.000000 libarchive-c-4.0/tests/data/tar_relative.tar
--rw-r--r--   0 changaco  (1142) users      (100)      195 2016-11-29 18:03:26.000000 libarchive-c-4.0/tests/data/testtar.README
--rw-r--r--   0 changaco  (1142) users      (100)   435200 2016-11-29 18:03:26.000000 libarchive-c-4.0/tests/data/testtar.tar
--rw-r--r--   0 changaco  (1142) users      (100)    16670 2018-06-10 13:01:15.000000 libarchive-c-4.0/tests/data/testtar.tar.json
--rw-r--r--   0 changaco  (1142) users      (100)    10240 2016-11-29 18:03:26.000000 libarchive-c-4.0/tests/data/unicode.tar
--rw-r--r--   0 changaco  (1142) users      (100)     1036 2018-06-10 11:44:59.000000 libarchive-c-4.0/tests/data/unicode.tar.json
--rw-r--r--   0 changaco  (1142) users      (100)      668 2016-11-29 18:03:26.000000 libarchive-c-4.0/tests/data/unicode.zip
--rw-r--r--   0 changaco  (1142) users      (100)      660 2018-06-10 11:44:59.000000 libarchive-c-4.0/tests/data/unicode.zip.json
--rw-r--r--   0 changaco  (1142) users      (100)      636 2016-11-29 18:03:26.000000 libarchive-c-4.0/tests/data/unicode2.zip
--rw-r--r--   0 changaco  (1142) users      (100)      649 2018-06-10 11:44:59.000000 libarchive-c-4.0/tests/data/unicode2.zip.json
--rw-r--r--   0 changaco  (1142) users      (100)      183 2016-11-29 18:03:26.000000 libarchive-c-4.0/tests/data/프로그램.README
--rw-r--r--   0 changaco  (1142) users      (100)      355 2016-11-29 18:03:26.000000 libarchive-c-4.0/tests/data/프로그램.zip
--rw-r--r--   0 changaco  (1142) users      (100)      676 2018-06-10 11:44:59.000000 libarchive-c-4.0/tests/data/프로그램.zip.json
--rw-r--r--   0 changaco  (1142) users      (100)     4713 2021-05-24 15:09:05.000000 libarchive-c-4.0/tests/test_atime_mtime_ctime.py
--rw-r--r--   0 changaco  (1142) users      (100)      717 2021-05-24 15:09:05.000000 libarchive-c-4.0/tests/test_convert.py
--rw-r--r--   0 changaco  (1142) users      (100)     4486 2022-01-22 17:28:18.000000 libarchive-c-4.0/tests/test_entry.py
--rw-r--r--   0 changaco  (1142) users      (100)     1206 2021-05-24 15:09:05.000000 libarchive-c-4.0/tests/test_errors.py
--rw-r--r--   0 changaco  (1142) users      (100)     5776 2022-01-22 17:28:18.000000 libarchive-c-4.0/tests/test_rwx.py
--rw-r--r--   0 changaco  (1142) users      (100)      917 2022-01-22 17:28:18.000000 libarchive-c-4.0/tests/test_security_flags.py
--rw-r--r--   0 changaco  (1142) users      (100)      294 2022-01-22 17:28:18.000000 libarchive-c-4.0/tox.ini
--rw-r--r--   0 changaco  (1142) users      (100)     1318 2016-11-29 18:03:26.000000 libarchive-c-4.0/version.py
+drwxr-xr-x   0 changaco  (1142) users      (100)        0 2023-07-04 08:24:25.007115 libarchive-c-5.0/
+-rw-r--r--   0 changaco  (1142) users      (100)       25 2016-11-29 18:03:26.000000 libarchive-c-5.0/.gitattributes
+drwxr-xr-x   0 changaco  (1142) users      (100)        0 2023-07-04 08:24:25.003781 libarchive-c-5.0/.github/
+-rw-r--r--   0 changaco  (1142) users      (100)       20 2021-05-24 14:29:37.000000 libarchive-c-5.0/.github/FUNDING.yml
+drwxr-xr-x   0 changaco  (1142) users      (100)        0 2023-07-04 08:24:25.003781 libarchive-c-5.0/.github/workflows/
+-rw-r--r--   0 changaco  (1142) users      (100)      998 2023-06-29 08:33:58.000000 libarchive-c-5.0/.github/workflows/main.yml
+-rw-r--r--   0 changaco  (1142) users      (100)       65 2016-11-29 18:03:29.000000 libarchive-c-5.0/.gitignore
+-rw-r--r--   0 changaco  (1142) users      (100)       51 2018-06-10 12:43:23.000000 libarchive-c-5.0/LICENSE.md
+-rw-r--r--   0 changaco  (1142) users      (100)       19 2016-11-29 18:03:22.000000 libarchive-c-5.0/MANIFEST.in
+-rw-r--r--   0 changaco  (1142) users      (100)     5308 2023-07-04 08:24:25.007115 libarchive-c-5.0/PKG-INFO
+-rw-r--r--   0 changaco  (1142) users      (100)     4977 2023-07-04 08:05:38.000000 libarchive-c-5.0/README.rst
+drwxr-xr-x   0 changaco  (1142) users      (100)        0 2023-07-04 08:24:25.003781 libarchive-c-5.0/libarchive/
+-rw-r--r--   0 changaco  (1142) users      (100)      601 2021-05-24 15:08:51.000000 libarchive-c-5.0/libarchive/__init__.py
+-rw-r--r--   0 changaco  (1142) users      (100)    14524 2023-07-04 08:05:38.000000 libarchive-c-5.0/libarchive/entry.py
+-rw-r--r--   0 changaco  (1142) users      (100)      370 2021-05-24 15:09:05.000000 libarchive-c-5.0/libarchive/exception.py
+-rw-r--r--   0 changaco  (1142) users      (100)     2694 2022-01-22 17:28:18.000000 libarchive-c-5.0/libarchive/extract.py
+-rw-r--r--   0 changaco  (1142) users      (100)    12593 2023-07-04 08:05:38.000000 libarchive-c-5.0/libarchive/ffi.py
+-rw-r--r--   0 changaco  (1142) users      (100)      211 2018-06-10 13:27:14.000000 libarchive-c-5.0/libarchive/flags.py
+-rw-r--r--   0 changaco  (1142) users      (100)     5835 2023-07-04 08:05:38.000000 libarchive-c-5.0/libarchive/read.py
+-rw-r--r--   0 changaco  (1142) users      (100)    10444 2023-07-04 08:05:38.000000 libarchive-c-5.0/libarchive/write.py
+drwxr-xr-x   0 changaco  (1142) users      (100)        0 2023-07-04 08:24:25.003781 libarchive-c-5.0/libarchive_c.egg-info/
+-rw-r--r--   0 changaco  (1142) users      (100)     5308 2023-07-04 08:24:24.000000 libarchive-c-5.0/libarchive_c.egg-info/PKG-INFO
+-rw-r--r--   0 changaco  (1142) users      (100)     1010 2023-07-04 08:24:24.000000 libarchive-c-5.0/libarchive_c.egg-info/SOURCES.txt
+-rw-r--r--   0 changaco  (1142) users      (100)        1 2023-07-04 08:24:24.000000 libarchive-c-5.0/libarchive_c.egg-info/dependency_links.txt
+-rw-r--r--   0 changaco  (1142) users      (100)       11 2023-07-04 08:24:24.000000 libarchive-c-5.0/libarchive_c.egg-info/top_level.txt
+-rw-r--r--   0 changaco  (1142) users      (100)      136 2023-07-04 08:24:25.007115 libarchive-c-5.0/setup.cfg
+-rw-r--r--   0 changaco  (1142) users      (100)      669 2023-06-29 08:33:58.000000 libarchive-c-5.0/setup.py
+drwxr-xr-x   0 changaco  (1142) users      (100)        0 2023-07-04 08:24:25.003781 libarchive-c-5.0/tests/
+-rw-r--r--   0 changaco  (1142) users      (100)     4297 2021-05-24 15:09:05.000000 libarchive-c-5.0/tests/__init__.py
+drwxr-xr-x   0 changaco  (1142) users      (100)        0 2023-07-04 08:24:25.007115 libarchive-c-5.0/tests/data/
+-rw-r--r--   0 changaco  (1142) users      (100)    10240 2018-06-10 11:44:59.000000 libarchive-c-5.0/tests/data/flags.tar
+-rw-r--r--   0 changaco  (1142) users      (100)   112640 2016-11-29 18:03:26.000000 libarchive-c-5.0/tests/data/special.tar
+-rw-r--r--   0 changaco  (1142) users      (100)    10240 2016-11-29 18:03:26.000000 libarchive-c-5.0/tests/data/tar_relative.tar
+-rw-r--r--   0 changaco  (1142) users      (100)      195 2016-11-29 18:03:26.000000 libarchive-c-5.0/tests/data/testtar.README
+-rw-r--r--   0 changaco  (1142) users      (100)   435200 2016-11-29 18:03:26.000000 libarchive-c-5.0/tests/data/testtar.tar
+-rw-r--r--   0 changaco  (1142) users      (100)    16670 2018-06-10 13:01:15.000000 libarchive-c-5.0/tests/data/testtar.tar.json
+-rw-r--r--   0 changaco  (1142) users      (100)    10240 2016-11-29 18:03:26.000000 libarchive-c-5.0/tests/data/unicode.tar
+-rw-r--r--   0 changaco  (1142) users      (100)     1036 2018-06-10 11:44:59.000000 libarchive-c-5.0/tests/data/unicode.tar.json
+-rw-r--r--   0 changaco  (1142) users      (100)      668 2016-11-29 18:03:26.000000 libarchive-c-5.0/tests/data/unicode.zip
+-rw-r--r--   0 changaco  (1142) users      (100)      660 2018-06-10 11:44:59.000000 libarchive-c-5.0/tests/data/unicode.zip.json
+-rw-r--r--   0 changaco  (1142) users      (100)      636 2016-11-29 18:03:26.000000 libarchive-c-5.0/tests/data/unicode2.zip
+-rw-r--r--   0 changaco  (1142) users      (100)      649 2018-06-10 11:44:59.000000 libarchive-c-5.0/tests/data/unicode2.zip.json
+-rw-r--r--   0 changaco  (1142) users      (100)      183 2016-11-29 18:03:26.000000 libarchive-c-5.0/tests/data/프로그램.README
+-rw-r--r--   0 changaco  (1142) users      (100)      355 2016-11-29 18:03:26.000000 libarchive-c-5.0/tests/data/프로그램.zip
+-rw-r--r--   0 changaco  (1142) users      (100)      676 2018-06-10 11:44:59.000000 libarchive-c-5.0/tests/data/프로그램.zip.json
+-rw-r--r--   0 changaco  (1142) users      (100)     4713 2021-05-24 15:09:05.000000 libarchive-c-5.0/tests/test_atime_mtime_ctime.py
+-rw-r--r--   0 changaco  (1142) users      (100)      717 2021-05-24 15:09:05.000000 libarchive-c-5.0/tests/test_convert.py
+-rw-r--r--   0 changaco  (1142) users      (100)     5018 2023-07-04 08:05:38.000000 libarchive-c-5.0/tests/test_entry.py
+-rw-r--r--   0 changaco  (1142) users      (100)     1206 2021-05-24 15:09:05.000000 libarchive-c-5.0/tests/test_errors.py
+-rw-r--r--   0 changaco  (1142) users      (100)     5785 2023-06-29 08:33:58.000000 libarchive-c-5.0/tests/test_rwx.py
+-rw-r--r--   0 changaco  (1142) users      (100)      917 2022-01-22 17:28:18.000000 libarchive-c-5.0/tests/test_security_flags.py
+-rw-r--r--   0 changaco  (1142) users      (100)      286 2023-07-04 08:23:03.000000 libarchive-c-5.0/tox.ini
+-rw-r--r--   0 changaco  (1142) users      (100)     1354 2023-06-29 08:33:58.000000 libarchive-c-5.0/version.py
```

### Comparing `libarchive-c-4.0/PKG-INFO` & `libarchive-c-5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: libarchive-c
-Version: 4.0
+Version: 5.0
 Summary: Python interface to libarchive
 Home-page: https://github.com/Changaco/python-libarchive-c
 Author: Changaco
 Author-email: changaco@changaco.oy.lc
 License: CC0
 Keywords: archive libarchive 7z tar bz2 zip gz
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 
 A Python interface to libarchive. It uses the standard ctypes_ module to
 dynamically load and access the C library.
 
 .. _ctypes: https://docs.python.org/3/library/ctypes.html
@@ -23,15 +22,15 @@
 
 Compatibility
 =============
 
 python
 ------
 
-python-libarchive-c is currently tested with python 3.7, 3.8, and 3.9.
+python-libarchive-c is currently tested with python 3.8, 3.9, 3.10 and 3.11.
 
 If you find an incompatibility with older versions you can send us a small patch,
 but we won't accept big changes.
 
 libarchive
 ----------
 
@@ -123,13 +122,26 @@
 ``fd_writer`` to a file descriptor, and ``custom_writer`` to a callback function.
 
 For each of those functions, the mandatory second argument is the archive format,
 and the optional third argument is the compression format (called “filter” in
 libarchive). The acceptable values are listed in ``libarchive.ffi.WRITE_FORMATS``
 and ``libarchive.ffi.WRITE_FILTERS``.
 
+File metadata codecs
+--------------------
+
+By default, UTF-8 is used to read and write file attributes from and to archives.
+A different codec can be specified through the ``header_codec`` arguments of the
+``*_reader`` and ``*_writer`` functions. Example::
+
+    with libarchive.file_writer('test.tar', 'ustar', header_codec='cp037') as archive:
+        ...
+    with file_reader('test.tar', header_codec='cp037') as archive:
+        ...
+
+In addition to file paths (``pathname`` and ``linkpath``), the specified codec is
+used to encode and decode user and group names (``uname`` and ``gname``).
+
 License
 =======
 
 `CC0 Public Domain Dedication <http://creativecommons.org/publicdomain/zero/1.0/>`_
-
-
```

### Comparing `libarchive-c-4.0/README.rst` & `libarchive-c-5.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Compatibility
 =============
 
 python
 ------
 
-python-libarchive-c is currently tested with python 3.7, 3.8, and 3.9.
+python-libarchive-c is currently tested with python 3.8, 3.9, 3.10 and 3.11.
 
 If you find an incompatibility with older versions you can send us a small patch,
 but we won't accept big changes.
 
 libarchive
 ----------
 
@@ -110,11 +110,26 @@
 ``fd_writer`` to a file descriptor, and ``custom_writer`` to a callback function.
 
 For each of those functions, the mandatory second argument is the archive format,
 and the optional third argument is the compression format (called “filter” in
 libarchive). The acceptable values are listed in ``libarchive.ffi.WRITE_FORMATS``
 and ``libarchive.ffi.WRITE_FILTERS``.
 
+File metadata codecs
+--------------------
+
+By default, UTF-8 is used to read and write file attributes from and to archives.
+A different codec can be specified through the ``header_codec`` arguments of the
+``*_reader`` and ``*_writer`` functions. Example::
+
+    with libarchive.file_writer('test.tar', 'ustar', header_codec='cp037') as archive:
+        ...
+    with file_reader('test.tar', header_codec='cp037') as archive:
+        ...
+
+In addition to file paths (``pathname`` and ``linkpath``), the specified codec is
+used to encode and decode user and group names (``uname`` and ``gname``).
+
 License
 =======
 
 `CC0 Public Domain Dedication <http://creativecommons.org/publicdomain/zero/1.0/>`_
```

### Comparing `libarchive-c-4.0/libarchive/__init__.py` & `libarchive-c-5.0/libarchive/__init__.py`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/libarchive/entry.py` & `libarchive-c-5.0/libarchive/entry.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from contextlib import contextmanager
-from ctypes import c_char_p, create_string_buffer
+from ctypes import create_string_buffer
 from enum import IntEnum
 import math
 
 from . import ffi
 
 
 class FileType(IntEnum):
@@ -30,35 +30,39 @@
     if nanos:
         return float(seconds) + float(nanos) / 1000000000.0
     return int(seconds)
 
 
 class ArchiveEntry:
 
-    __slots__ = ('_archive_p', '_entry_p')
+    __slots__ = ('_archive_p', '_entry_p', 'header_codec')
 
-    def __init__(self, archive_p=None, **attributes):
+    def __init__(self, archive_p=None, header_codec='utf-8', **attributes):
         """Allocate memory for an `archive_entry` struct.
 
-        The attributes are passed to the `modify` method.
+        The `header_codec` is used to decode and encode file paths and other
+        attributes.
+
+        The `**attributes` are passed to the `modify` method.
         """
         self._archive_p = archive_p
         self._entry_p = ffi.entry_new()
+        self.header_codec = header_codec
         if attributes:
             self.modify(**attributes)
 
     def __del__(self):
         """Free the C struct"""
         ffi.entry_free(self._entry_p)
 
     def __str__(self):
         """Returns the file's path"""
         return self.pathname
 
-    def modify(self, **attributes):
+    def modify(self, header_codec=None, **attributes):
         """Convenience method to modify the entry's attributes.
 
         Args:
             filetype (int): the file's type, see the `FileType` class for values
             pathname (str): the file's path
             linkpath (str): the other path of the file, if the file is a link
             size (int | None): the file's size, in bytes
@@ -79,14 +83,16 @@
             birthtime (int | Tuple[int, int] | float | None):
                 the file's creation time (for archive formats that support it),
                 either in seconds or as a tuple (seconds, nanoseconds)
             rdev (int | Tuple[int, int]): device number, if the file is a device
             rdevmajor (int): major part of the device number
             rdevminor (int): minor part of the device number
         """
+        if header_codec:
+            self.header_codec = header_codec
         for name, value in attributes.items():
             setattr(self, name, value)
 
     @property
     def filetype(self):
         return ffi.entry_filetype(self._entry_p)
 
@@ -108,31 +114,53 @@
 
     @gid.setter
     def gid(self, gid):
         ffi.entry_set_gid(self._entry_p, gid)
 
     @property
     def uname(self):
-        return ffi.entry_uname_w(self._entry_p)
+        uname = ffi.entry_uname_w(self._entry_p)
+        if not uname:
+            uname = ffi.entry_uname(self._entry_p)
+            if uname is not None:
+                try:
+                    uname = uname.decode(self.header_codec)
+                except UnicodeError:
+                    pass
+        return uname
 
     @uname.setter
     def uname(self, value):
         if not isinstance(value, bytes):
-            value = value.encode('utf8')
-        ffi.entry_update_uname_utf8(self._entry_p, value)
+            value = value.encode(self.header_codec)
+        if self.header_codec == 'utf-8':
+            ffi.entry_update_uname_utf8(self._entry_p, value)
+        else:
+            ffi.entry_copy_uname(self._entry_p, value)
 
     @property
     def gname(self):
-        return ffi.entry_gname_w(self._entry_p)
+        gname = ffi.entry_gname_w(self._entry_p)
+        if not gname:
+            gname = ffi.entry_gname(self._entry_p)
+            if gname is not None:
+                try:
+                    gname = gname.decode(self.header_codec)
+                except UnicodeError:
+                    pass
+        return gname
 
     @gname.setter
     def gname(self, value):
         if not isinstance(value, bytes):
-            value = value.encode('utf8')
-        ffi.entry_update_gname_utf8(self._entry_p, value)
+            value = value.encode(self.header_codec)
+        if self.header_codec == 'utf-8':
+            ffi.entry_update_gname_utf8(self._entry_p, value)
+        else:
+            ffi.entry_copy_gname(self._entry_p, value)
 
     def get_blocks(self, block_size=ffi.page_size):
         """Read the file's content, keeping only one chunk in memory at a time.
 
         Don't do anything like `list(entry.get_blocks())`, it would silently fail.
 
         Args:
@@ -207,15 +235,15 @@
             self.set_atime(value)
         elif isinstance(value, tuple):
             self.set_atime(*value)
         else:
             seconds, fraction = math.modf(value)
             self.set_atime(int(seconds), int(fraction * 1_000_000_000))
 
-    def set_atime(self, timestamp_sec, timestamp_nsec):
+    def set_atime(self, timestamp_sec, timestamp_nsec=0):
         "Kept for backward compatibility. `entry.atime = ...` is supported now."
         return ffi.entry_set_atime(self._entry_p, timestamp_sec, timestamp_nsec)
 
     @property
     def mtime(self):
         if not ffi.entry_mtime_is_set(self._entry_p):
             return None
@@ -231,15 +259,15 @@
             self.set_mtime(value)
         elif isinstance(value, tuple):
             self.set_mtime(*value)
         else:
             seconds, fraction = math.modf(value)
             self.set_mtime(int(seconds), int(fraction * 1_000_000_000))
 
-    def set_mtime(self, timestamp_sec, timestamp_nsec):
+    def set_mtime(self, timestamp_sec, timestamp_nsec=0):
         "Kept for backward compatibility. `entry.mtime = ...` is supported now."
         return ffi.entry_set_mtime(self._entry_p, timestamp_sec, timestamp_nsec)
 
     @property
     def ctime(self):
         if not ffi.entry_ctime_is_set(self._entry_p):
             return None
@@ -255,15 +283,15 @@
             self.set_ctime(value)
         elif isinstance(value, tuple):
             self.set_ctime(*value)
         else:
             seconds, fraction = math.modf(value)
             self.set_ctime(int(seconds), int(fraction * 1_000_000_000))
 
-    def set_ctime(self, timestamp_sec, timestamp_nsec):
+    def set_ctime(self, timestamp_sec, timestamp_nsec=0):
         "Kept for backward compatibility. `entry.ctime = ...` is supported now."
         return ffi.entry_set_ctime(self._entry_p, timestamp_sec, timestamp_nsec)
 
     @property
     def birthtime(self):
         if not ffi.entry_birthtime_is_set(self._entry_p):
             return None
@@ -290,36 +318,56 @@
         )
 
     @property
     def pathname(self):
         path = ffi.entry_pathname_w(self._entry_p)
         if not path:
             path = ffi.entry_pathname(self._entry_p)
-            try:
-                path = path.decode()
-            except UnicodeError:
-                pass
+            if path is not None:
+                try:
+                    path = path.decode(self.header_codec)
+                except UnicodeError:
+                    pass
         return path
 
     @pathname.setter
     def pathname(self, value):
         if not isinstance(value, bytes):
-            value = value.encode('utf8')
-        ffi.entry_update_pathname_utf8(self._entry_p, c_char_p(value))
+            value = value.encode(self.header_codec)
+        if self.header_codec == 'utf-8':
+            ffi.entry_update_pathname_utf8(self._entry_p, value)
+        else:
+            ffi.entry_copy_pathname(self._entry_p, value)
 
     @property
     def linkpath(self):
-        return (ffi.entry_symlink_w(self._entry_p) or
+        path = (
+            (
+                ffi.entry_symlink_w(self._entry_p) or
+                ffi.entry_symlink(self._entry_p)
+            ) if self.issym else (
                 ffi.entry_hardlink_w(self._entry_p) or
-                ffi.entry_symlink(self._entry_p) or
-                ffi.entry_hardlink(self._entry_p))
+                ffi.entry_hardlink(self._entry_p)
+            )
+        )
+        if isinstance(path, bytes):
+            try:
+                path = path.decode(self.header_codec)
+            except UnicodeError:
+                pass
+        return path
 
     @linkpath.setter
     def linkpath(self, value):
-        ffi.entry_update_link_utf8(self._entry_p, value)
+        if not isinstance(value, bytes):
+            value = value.encode(self.header_codec)
+        if self.header_codec == 'utf-8':
+            ffi.entry_update_link_utf8(self._entry_p, value)
+        else:
+            ffi.entry_copy_link(self._entry_p, value)
 
     # aliases for compatibility with the standard `tarfile` module
     path = property(pathname.fget, pathname.fset, doc="alias of pathname")
     name = path
     linkname = property(linkpath.fget, linkpath.fset, doc="alias of linkpath")
 
     @property
```

### Comparing `libarchive-c-4.0/libarchive/extract.py` & `libarchive-c-5.0/libarchive/extract.py`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/libarchive/ffi.py` & `libarchive-c-5.0/libarchive/ffi.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,16 @@
 ffi('entry_symlink', [c_archive_entry_p], c_char_p)
 ffi('entry_symlink_w', [c_archive_entry_p], c_wchar_p)
 ffi('entry_rdev', [c_archive_entry_p], c_uint)
 ffi('entry_rdevmajor', [c_archive_entry_p], c_uint)
 ffi('entry_rdevminor', [c_archive_entry_p], c_uint)
 ffi('entry_uid', [c_archive_entry_p], c_longlong)
 ffi('entry_gid', [c_archive_entry_p], c_longlong)
+ffi('entry_uname', [c_archive_entry_p], c_char_p)
+ffi('entry_gname', [c_archive_entry_p], c_char_p)
 ffi('entry_uname_w', [c_archive_entry_p], c_wchar_p)
 ffi('entry_gname_w', [c_archive_entry_p], c_wchar_p)
 
 ffi('entry_set_size', [c_archive_entry_p, c_longlong], None)
 ffi('entry_set_filetype', [c_archive_entry_p, c_uint], None)
 ffi('entry_set_uid', [c_archive_entry_p, c_longlong], None)
 ffi('entry_set_gid', [c_archive_entry_p, c_longlong], None)
@@ -218,17 +220,21 @@
 ffi('entry_set_rdevminor', [c_archive_entry_p, c_uint], None)
 ffi('entry_unset_size', [c_archive_entry_p], None)
 ffi('entry_unset_atime', [c_archive_entry_p], None)
 ffi('entry_unset_mtime', [c_archive_entry_p], None)
 ffi('entry_unset_ctime', [c_archive_entry_p], None)
 ffi('entry_unset_birthtime', [c_archive_entry_p], None)
 
+ffi('entry_copy_pathname', [c_archive_entry_p, c_char_p], None)
 ffi('entry_update_pathname_utf8', [c_archive_entry_p, c_char_p], c_int, check_int)
+ffi('entry_copy_link', [c_archive_entry_p, c_char_p], None)
 ffi('entry_update_link_utf8', [c_archive_entry_p, c_char_p], c_int, check_int)
+ffi('entry_copy_uname', [c_archive_entry_p, c_char_p], None)
 ffi('entry_update_uname_utf8', [c_archive_entry_p, c_char_p], c_int, check_int)
+ffi('entry_copy_gname', [c_archive_entry_p, c_char_p], None)
 ffi('entry_update_gname_utf8', [c_archive_entry_p, c_char_p], c_int, check_int)
 
 ffi('entry_clear', [c_archive_entry_p], c_archive_entry_p)
 ffi('entry_free', [c_archive_entry_p], None)
 
 # archive_read
```

### Comparing `libarchive-c-4.0/libarchive/read.py` & `libarchive-c-5.0/libarchive/read.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,24 +8,26 @@
     NO_OPEN_CB, NO_CLOSE_CB, page_size,
 )
 from .entry import ArchiveEntry, PassedArchiveEntry
 
 
 class ArchiveRead:
 
-    def __init__(self, archive_p):
+    def __init__(self, archive_p, header_codec='utf-8'):
         self._pointer = archive_p
+        self.header_codec = header_codec
 
     def __iter__(self):
         """Iterates through an archive's entries.
         """
         archive_p = self._pointer
+        header_codec = self.header_codec
         read_next_header2 = ffi.read_next_header2
         while 1:
-            entry = ArchiveEntry(archive_p)
+            entry = ArchiveEntry(archive_p, header_codec)
             r = read_next_header2(archive_p, entry._entry_p)
             if r == ARCHIVE_EOF:
                 return
             yield entry
             entry.__class__ = PassedArchiveEntry
 
     @property
@@ -64,71 +66,77 @@
 
 
 @contextmanager
 def custom_reader(
     read_func, format_name='all', filter_name='all',
     open_func=None, seek_func=None, close_func=None,
     block_size=page_size, archive_read_class=ArchiveRead, passphrase=None,
+    header_codec='utf-8',
 ):
     """Read an archive using a custom function.
     """
     open_cb = OPEN_CALLBACK(open_func) if open_func else NO_OPEN_CB
     read_cb = READ_CALLBACK(read_func)
     close_cb = CLOSE_CALLBACK(close_func) if close_func else NO_CLOSE_CB
     seek_cb = SEEK_CALLBACK(seek_func)
     with new_archive_read(format_name, filter_name, passphrase) as archive_p:
         if seek_func:
             ffi.read_set_seek_callback(archive_p, seek_cb)
         ffi.read_open(archive_p, None, open_cb, read_cb, close_cb)
-        yield archive_read_class(archive_p)
+        yield archive_read_class(archive_p, header_codec)
 
 
 @contextmanager
 def fd_reader(
     fd, format_name='all', filter_name='all', block_size=4096, passphrase=None,
+    header_codec='utf-8',
 ):
     """Read an archive from a file descriptor.
     """
     with new_archive_read(format_name, filter_name, passphrase) as archive_p:
         try:
             block_size = fstat(fd).st_blksize
         except (OSError, AttributeError):  # pragma: no cover
             pass
         ffi.read_open_fd(archive_p, fd, block_size)
-        yield ArchiveRead(archive_p)
+        yield ArchiveRead(archive_p, header_codec)
 
 
 @contextmanager
 def file_reader(
     path, format_name='all', filter_name='all', block_size=4096, passphrase=None,
+    header_codec='utf-8',
 ):
     """Read an archive from a file.
     """
     with new_archive_read(format_name, filter_name, passphrase) as archive_p:
         try:
             block_size = stat(path).st_blksize
         except (OSError, AttributeError):  # pragma: no cover
             pass
         ffi.read_open_filename_w(archive_p, path, block_size)
-        yield ArchiveRead(archive_p)
+        yield ArchiveRead(archive_p, header_codec)
 
 
 @contextmanager
-def memory_reader(buf, format_name='all', filter_name='all', passphrase=None):
+def memory_reader(
+    buf, format_name='all', filter_name='all', passphrase=None,
+    header_codec='utf-8',
+):
     """Read an archive from memory.
     """
     with new_archive_read(format_name, filter_name, passphrase) as archive_p:
         ffi.read_open_memory(archive_p, cast(buf, c_void_p), len(buf))
-        yield ArchiveRead(archive_p)
+        yield ArchiveRead(archive_p, header_codec)
 
 
 @contextmanager
 def stream_reader(
     stream, format_name='all', filter_name='all', block_size=page_size,
-    passphrase=None,
+    passphrase=None, header_codec='utf-8',
 ):
     """Read an archive from a stream.
 
     The `stream` object must support the standard `readinto` method.
 
     If `stream.seekable()` returns `True`, then an appropriate seek callback is
     passed to libarchive.
@@ -154,11 +162,11 @@
     read_cb = READ_CALLBACK(read_func)
     close_cb = NO_CLOSE_CB
     seek_cb = SEEK_CALLBACK(seek_func)
     with new_archive_read(format_name, filter_name, passphrase) as archive_p:
         if stream.seekable():
             ffi.read_set_seek_callback(archive_p, seek_cb)
         ffi.read_open(archive_p, None, open_cb, read_cb, close_cb)
-        yield ArchiveRead(archive_p)
+        yield ArchiveRead(archive_p, header_codec)
 
 
 seekable_stream_reader = stream_reader
```

### Comparing `libarchive-c-4.0/libarchive/write.py` & `libarchive-c-5.0/libarchive/write.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,55 +26,60 @@
         yield archive_p
     finally:
         read_free(archive_p)
 
 
 class ArchiveWrite:
 
-    def __init__(self, archive_p):
+    def __init__(self, archive_p, header_codec='utf-8'):
         self._pointer = archive_p
+        self.header_codec = header_codec
 
     def add_entries(self, entries):
         """Add the given entries to the archive.
         """
         write_p = self._pointer
         for entry in entries:
             write_header(write_p, entry._entry_p)
             for block in entry.get_blocks():
                 write_data(write_p, block, len(block))
             write_finish_entry(write_p)
 
     def add_files(
-        self, *paths, flags=0, lookup=False, pathname=None, **attributes
+        self, *paths, flags=0, lookup=False, pathname=None, recursive=True,
+        **attributes
     ):
         """Read files through the OS and add them to the archive.
 
         Args:
             paths (str): the paths of the files to add to the archive
             flags (int):
                 passed to the C function `archive_read_disk_set_behavior`;
                 use the `libarchive.flags.READDISK_*` constants
             lookup (bool):
                 when True, the C function `archive_read_disk_set_standard_lookup`
                 is called to enable the lookup of user and group names
             pathname (str | None):
                 the path of the file in the archive, defaults to the source path
+            recursive (bool):
+                when False, if a path in `paths` is a directory,
+                only the directory itself is added.
             attributes (dict): passed to `ArchiveEntry.modify()`
 
         Raises:
             ArchiveError: if a file doesn't exist or can't be accessed, or if
                           adding it to the archive fails
         """
         write_p = self._pointer
 
         block_size = ffi.write_get_bytes_per_block(write_p)
         if block_size <= 0:
             block_size = 10240  # pragma: no cover
 
-        entry = ArchiveEntry()
+        entry = ArchiveEntry(header_codec=self.header_codec)
         entry_p = entry._entry_p
         destination_path = attributes.pop('pathname', None)
         for path in paths:
             with new_archive_read_disk(path, flags, lookup) as read_p:
                 while 1:
                     r = read_next_header2(read_p, entry_p)
                     if r == ARCHIVE_EOF:
@@ -99,28 +104,30 @@
                             while 1:
                                 data = f.read(block_size)
                                 if not data:
                                     break
                                 write_data(write_p, data, len(data))
                     write_finish_entry(write_p)
                     entry_clear(entry_p)
+                    if not recursive:
+                        break
 
     def add_file(self, path, **kw):
         "Single-path alias of `add_files()`"
         return self.add_files(path, **kw)
 
     def add_file_from_memory(
         self, entry_path, entry_size, entry_data,
         filetype=FileType.REGULAR_FILE, permission=0o664,
         **other_attributes
     ):
         """"Add file from memory to archive.
 
         Args:
-            entry_path (str): the file's path
+            entry_path (str | bytes): the file's path
             entry_size (int): the file's size, in bytes
             entry_data (bytes | Iterable[bytes]): the file's content
             filetype (int): see `libarchive.entry.ArchiveEntry.modify()`
             permission (int): see `libarchive.entry.ArchiveEntry.modify()`
             other_attributes: see `libarchive.entry.ArchiveEntry.modify()`
         """
         archive_pointer = self._pointer
@@ -130,15 +137,16 @@
         elif isinstance(entry_data, str):
             raise TypeError(
                 "entry_data: expected bytes, got %r" % type(entry_data)
             )
 
         entry = ArchiveEntry(
             pathname=entry_path, size=entry_size, filetype=filetype,
-            perm=permission, **other_attributes
+            perm=permission, header_codec=self.header_codec,
+            **other_attributes
         )
         write_header(archive_pointer, entry._entry_p)
 
         for chunk in entry_data:
             if not chunk:
                 break
             write_data(archive_pointer, chunk, len(chunk))
@@ -190,14 +198,15 @@
 
 
 @contextmanager
 def custom_writer(
     write_func, format_name, filter_name=None,
     open_func=None, close_func=None, block_size=page_size,
     archive_write_class=ArchiveWrite, options='', passphrase=None,
+    header_codec='utf-8',
 ):
     """Create an archive and send it in chunks to the `write_func` function.
 
     For formats and filters, see `WRITE_FORMATS` and `WRITE_FILTERS` in the
     `libarchive.ffi` module.
     """
 
@@ -210,58 +219,61 @@
     close_cb = CLOSE_CALLBACK(close_func) if close_func else NO_CLOSE_CB
 
     with new_archive_write(format_name, filter_name, options,
                            passphrase) as archive_p:
         ffi.write_set_bytes_in_last_block(archive_p, 1)
         ffi.write_set_bytes_per_block(archive_p, block_size)
         ffi.write_open(archive_p, None, open_cb, write_cb, close_cb)
-        yield archive_write_class(archive_p)
+        yield archive_write_class(archive_p, header_codec)
 
 
 @contextmanager
 def fd_writer(
     fd, format_name, filter_name=None,
     archive_write_class=ArchiveWrite, options='', passphrase=None,
+    header_codec='utf-8',
 ):
     """Create an archive and write it into a file descriptor.
 
     For formats and filters, see `WRITE_FORMATS` and `WRITE_FILTERS` in the
     `libarchive.ffi` module.
     """
     with new_archive_write(format_name, filter_name, options,
                            passphrase) as archive_p:
         ffi.write_open_fd(archive_p, fd)
-        yield archive_write_class(archive_p)
+        yield archive_write_class(archive_p, header_codec)
 
 
 @contextmanager
 def file_writer(
     filepath, format_name, filter_name=None,
     archive_write_class=ArchiveWrite, options='', passphrase=None,
+    header_codec='utf-8',
 ):
     """Create an archive and write it into a file.
 
     For formats and filters, see `WRITE_FORMATS` and `WRITE_FILTERS` in the
     `libarchive.ffi` module.
     """
     with new_archive_write(format_name, filter_name, options,
                            passphrase) as archive_p:
         ffi.write_open_filename_w(archive_p, filepath)
-        yield archive_write_class(archive_p)
+        yield archive_write_class(archive_p, header_codec)
 
 
 @contextmanager
 def memory_writer(
     buf, format_name, filter_name=None,
     archive_write_class=ArchiveWrite, options='', passphrase=None,
+    header_codec='utf-8',
 ):
     """Create an archive and write it into a buffer.
 
     For formats and filters, see `WRITE_FORMATS` and `WRITE_FILTERS` in the
     `libarchive.ffi` module.
     """
     with new_archive_write(format_name, filter_name, options,
                            passphrase) as archive_p:
         used = byref(c_size_t())
         buf_p = cast(buf, c_void_p)
         ffi.write_open_memory(archive_p, buf_p, len(buf), used)
-        yield archive_write_class(archive_p)
+        yield archive_write_class(archive_p, header_codec)
```

### Comparing `libarchive-c-4.0/libarchive_c.egg-info/PKG-INFO` & `libarchive-c-5.0/libarchive_c.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: libarchive-c
-Version: 4.0
+Version: 5.0
 Summary: Python interface to libarchive
 Home-page: https://github.com/Changaco/python-libarchive-c
 Author: Changaco
 Author-email: changaco@changaco.oy.lc
 License: CC0
 Keywords: archive libarchive 7z tar bz2 zip gz
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 
 A Python interface to libarchive. It uses the standard ctypes_ module to
 dynamically load and access the C library.
 
 .. _ctypes: https://docs.python.org/3/library/ctypes.html
@@ -23,15 +22,15 @@
 
 Compatibility
 =============
 
 python
 ------
 
-python-libarchive-c is currently tested with python 3.7, 3.8, and 3.9.
+python-libarchive-c is currently tested with python 3.8, 3.9, 3.10 and 3.11.
 
 If you find an incompatibility with older versions you can send us a small patch,
 but we won't accept big changes.
 
 libarchive
 ----------
 
@@ -123,13 +122,26 @@
 ``fd_writer`` to a file descriptor, and ``custom_writer`` to a callback function.
 
 For each of those functions, the mandatory second argument is the archive format,
 and the optional third argument is the compression format (called “filter” in
 libarchive). The acceptable values are listed in ``libarchive.ffi.WRITE_FORMATS``
 and ``libarchive.ffi.WRITE_FILTERS``.
 
+File metadata codecs
+--------------------
+
+By default, UTF-8 is used to read and write file attributes from and to archives.
+A different codec can be specified through the ``header_codec`` arguments of the
+``*_reader`` and ``*_writer`` functions. Example::
+
+    with libarchive.file_writer('test.tar', 'ustar', header_codec='cp037') as archive:
+        ...
+    with file_reader('test.tar', header_codec='cp037') as archive:
+        ...
+
+In addition to file paths (``pathname`` and ``linkpath``), the specified codec is
+used to encode and decode user and group names (``uname`` and ``gname``).
+
 License
 =======
 
 `CC0 Public Domain Dedication <http://creativecommons.org/publicdomain/zero/1.0/>`_
-
-
```

### Comparing `libarchive-c-4.0/libarchive_c.egg-info/SOURCES.txt` & `libarchive-c-5.0/libarchive_c.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/setup.py` & `libarchive-c-5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 
 from setuptools import setup, find_packages
 
 from version import get_version
 
 os.umask(0o022)
 
+with open(join(dirname(__file__), 'README.rst'), encoding="utf-8") as f:
+    README = f.read()
+
 setup(
     name='libarchive-c',
     version=get_version(),
     description='Python interface to libarchive',
     author='Changaco',
     author_email='changaco@changaco.oy.lc',
     url='https://github.com/Changaco/python-libarchive-c',
     license='CC0',
     packages=find_packages(exclude=['tests']),
-    long_description=open(join(dirname(__file__), 'README.rst')).read(),
+    long_description=README,
     long_description_content_type='text/x-rst',
     keywords='archive libarchive 7z tar bz2 zip gz',
 )
```

### Comparing `libarchive-c-4.0/tests/__init__.py` & `libarchive-c-5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/tests/data/flags.tar` & `libarchive-c-5.0/tests/data/flags.tar`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/tests/data/special.tar` & `libarchive-c-5.0/tests/data/special.tar`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/tests/data/tar_relative.tar` & `libarchive-c-5.0/tests/data/tar_relative.tar`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/tests/data/testtar.tar` & `libarchive-c-5.0/tests/data/testtar.tar`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/tests/data/testtar.tar.json` & `libarchive-c-5.0/tests/data/testtar.tar.json`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/tests/data/unicode.tar` & `libarchive-c-5.0/tests/data/unicode.tar`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/tests/data/unicode.tar.json` & `libarchive-c-5.0/tests/data/unicode.tar.json`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/tests/data/unicode.zip` & `libarchive-c-5.0/tests/data/unicode.zip`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/tests/data/unicode.zip.json` & `libarchive-c-5.0/tests/data/unicode.zip.json`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/tests/data/unicode2.zip` & `libarchive-c-5.0/tests/data/unicode2.zip`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/tests/data/unicode2.zip.json` & `libarchive-c-5.0/tests/data/unicode2.zip.json`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/tests/data/프로그램.zip.json` & `libarchive-c-5.0/tests/data/프로그램.zip.json`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/tests/test_atime_mtime_ctime.py` & `libarchive-c-5.0/tests/test_atime_mtime_ctime.py`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/tests/test_convert.py` & `libarchive-c-5.0/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/tests/test_entry.py` & `libarchive-c-5.0/tests/test_entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             for key in d:
                 if isinstance(d[key], text_type):
                     d[key] = unicodedata.normalize('NFC', d[key])
         assert e1 == e2
 
 
 def test_the_life_cycle_of_archive_entries():
-    """Check that the `get_blocks` method only works on the current entry, and only once.
+    """Check that `get_blocks` only works on the current entry, and only once.
     """
     # Create a test archive in memory
     buf = bytes(bytearray(10_000_000))
     with memory_writer(buf, 'gnutar') as archive:
         archive.add_files(
             'README.rst',
             'libarchive/__init__.py',
@@ -131,7 +131,21 @@
         assert type(entry1) is PassedArchiveEntry
         with pytest.raises(TypeError):
             entry1.get_blocks()
         entry3 = next(archive_iter)
         assert type(entry3) is ArchiveEntry
         assert type(entry2) is PassedArchiveEntry
         assert type(entry1) is PassedArchiveEntry
+
+
+def test_non_ASCII_encoding_of_file_metadata():
+    buf = bytes(bytearray(100_000))
+    file_name = 'README.rst'
+    encoded_file_name = 'README.rst'.encode('cp037')
+    with memory_writer(buf, 'ustar', header_codec='cp037') as archive:
+        archive.add_file(file_name)
+    with memory_reader(buf) as archive:
+        entry = next(iter(archive))
+        assert entry.pathname == encoded_file_name
+    with memory_reader(buf, header_codec='cp037') as archive:
+        entry = next(iter(archive))
+        assert entry.pathname == file_name
```

### Comparing `libarchive-c-4.0/tests/test_errors.py` & `libarchive-c-5.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/tests/test_rwx.py` & `libarchive-c-5.0/tests/test_rwx.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import io
 import json
 
 import libarchive
 from libarchive.entry import format_time
 from libarchive.extract import EXTRACT_OWNER, EXTRACT_PERM, EXTRACT_TIME
 from libarchive.write import memory_writer
-from mock import patch
+from unittest.mock import patch
 import pytest
 
 from . import check_archive, in_dir, treestat
 
 
 def test_buffers(tmpdir):
```

### Comparing `libarchive-c-4.0/tests/test_security_flags.py` & `libarchive-c-5.0/tests/test_security_flags.py`

 * *Files identical despite different names*

### Comparing `libarchive-c-4.0/version.py` & `libarchive-c-5.0/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         if '-' in version:
             if version.endswith('-dirty'):
                 raise RuntimeError('The working tree is dirty')
             version = '.post'.join(version.split('-')[:2])
 
     else:
         # Extract the version from the PKG-INFO file.
-        with open(join(d, 'PKG-INFO')) as f:
+        with open(join(d, 'PKG-INFO'), encoding='utf-8', errors='replace') as f:
             version = version_re.search(f.read()).group(1)
 
     return version
 
 
 if __name__ == '__main__':
     print(get_version())
```

