# Comparing `tmp/ctpwrapper-6.6.9.1.tar.gz` & `tmp/ctpwrapper-6.6.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctpwrapper-6.6.9.1.tar", last modified: Wed Feb 22 16:16:34 2023, max compression
+gzip compressed data, was "ctpwrapper-6.6.9.2.tar", last modified: Tue Jul  4 14:35:46 2023, max compression
```

## Comparing `ctpwrapper-6.6.9.1.tar` & `ctpwrapper-6.6.9.2.tar`

### file list

```diff
@@ -1,56 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 16:16:34.378363 ctpwrapper-6.6.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-02-22 16:16:34.378363 ctpwrapper-6.6.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 16:16:34.354362 ctpwrapper-6.6.9.1/ctp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 16:16:34.354362 ctpwrapper-6.6.9.1/ctp/header/
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctp/header/DataCollect.h
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctp/header/ThostFtdcMdApi.h
--rw-r--r--   0 runner    (1001) docker     (123)    44962 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctp/header/ThostFtdcTraderApi.h
--rw-r--r--   0 runner    (1001) docker     (123)   273924 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctp/header/ThostFtdcUserApiDataType.h
--rw-r--r--   0 runner    (1001) docker     (123)   327032 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctp/header/ThostFtdcUserApiStruct.h
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctp/header/error.dtd
--rw-r--r--   0 runner    (1001) docker     (123)    25107 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctp/header/error.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 16:16:34.362362 ctpwrapper-6.6.9.1/ctp/linux/
--rw-r--r--   0 runner    (1001) docker     (123)  2667444 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctp/linux/libLinuxDataCollect.so
--rw-r--r--   0 runner    (1001) docker     (123)  4818248 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctp/linux/libthostmduserapi_se.so
--rw-r--r--   0 runner    (1001) docker     (123)  5467003 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctp/linux/libthosttraderapi_se.so
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctp/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 16:16:34.374363 ctpwrapper-6.6.9.1/ctp/win/
--rw-r--r--   0 runner    (1001) docker     (123)  1865728 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctp/win/WinDataCollect.dll
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctp/win/WinDataCollect.lib
--rw-r--r--   0 runner    (1001) docker     (123)  2941440 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctp/win/thostmduserapi_se.dll
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctp/win/thostmduserapi_se.lib
--rw-r--r--   0 runner    (1001) docker     (123)  3325952 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctp/win/thosttraderapi_se.dll
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctp/win/thosttraderapi_se.lib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 16:16:34.378363 ctpwrapper-6.6.9.1/ctpwrapper/
--rw-r--r--   0 runner    (1001) docker     (123)   709696 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctpwrapper/ApiStructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctpwrapper/Md.py
--rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctpwrapper/MdApi.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    52430 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctpwrapper/Trader.py
--rw-r--r--   0 runner    (1001) docker     (123)   126322 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctpwrapper/TraderApi.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctpwrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctpwrapper/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 16:16:34.378363 ctpwrapper-6.6.9.1/ctpwrapper/cppheader/
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctpwrapper/cppheader/CMdAPI.h
--rw-r--r--   0 runner    (1001) docker     (123)    60056 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctpwrapper/cppheader/CTraderAPI.h
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctpwrapper/datacollect.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 16:16:34.378363 ctpwrapper-6.6.9.1/ctpwrapper/headers/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctpwrapper/headers/DataCollect.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    38616 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctpwrapper/headers/ThostFtdcUserApiDataType.pxd
--rw-r--r--   0 runner    (1001) docker     (123)   222333 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctpwrapper/headers/ThostFtdcUserApiStruct.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctpwrapper/headers/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctpwrapper/headers/cMdAPI.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    19840 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/ctpwrapper/headers/cTraderApi.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 16:16:34.378363 ctpwrapper-6.6.9.1/ctpwrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-02-22 16:16:34.000000 ctpwrapper-6.6.9.1/ctpwrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-02-22 16:16:34.000000 ctpwrapper-6.6.9.1/ctpwrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 16:16:34.000000 ctpwrapper-6.6.9.1/ctpwrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-22 16:16:34.000000 ctpwrapper-6.6.9.1/ctpwrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-22 16:16:34.378363 ctpwrapper-6.6.9.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     5210 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 16:16:34.378363 ctpwrapper-6.6.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/tests/test_datacollect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-02-22 16:16:25.000000 ctpwrapper-6.6.9.1/tests/test_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:35:46.569919 ctpwrapper-6.6.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-04 14:35:46.573919 ctpwrapper-6.6.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:35:46.545919 ctpwrapper-6.6.9.2/ctp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:35:46.545919 ctpwrapper-6.6.9.2/ctp/header/
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctp/header/DataCollect.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctp/header/ThostFtdcMdApi.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44962 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctp/header/ThostFtdcTraderApi.h
+-rw-r--r--   0 runner    (1001) docker     (123)   273924 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctp/header/ThostFtdcUserApiDataType.h
+-rw-r--r--   0 runner    (1001) docker     (123)   327032 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctp/header/ThostFtdcUserApiStruct.h
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctp/header/error.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)    25107 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctp/header/error.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:35:46.553919 ctpwrapper-6.6.9.2/ctp/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)  2667444 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctp/linux/libLinuxDataCollect.so
+-rw-r--r--   0 runner    (1001) docker     (123)  4818248 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctp/linux/libthostmduserapi_se.so
+-rw-r--r--   0 runner    (1001) docker     (123)  5467003 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctp/linux/libthosttraderapi_se.so
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctp/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:35:46.569919 ctpwrapper-6.6.9.2/ctp/win/
+-rw-r--r--   0 runner    (1001) docker     (123)  1865728 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctp/win/WinDataCollect.dll
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctp/win/WinDataCollect.lib
+-rw-r--r--   0 runner    (1001) docker     (123)  2941440 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctp/win/thostmduserapi_se.dll
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctp/win/thostmduserapi_se.lib
+-rw-r--r--   0 runner    (1001) docker     (123)  3325952 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctp/win/thosttraderapi_se.dll
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctp/win/thosttraderapi_se.lib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:35:46.569919 ctpwrapper-6.6.9.2/ctpwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)   709696 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctpwrapper/ApiStructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9338 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctpwrapper/Md.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctpwrapper/MdApi.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    52430 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctpwrapper/Trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126322 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctpwrapper/TraderApi.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctpwrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctpwrapper/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:35:46.569919 ctpwrapper-6.6.9.2/ctpwrapper/cppheader/
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctpwrapper/cppheader/CMdAPI.h
+-rw-r--r--   0 runner    (1001) docker     (123)    60056 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctpwrapper/cppheader/CTraderAPI.h
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctpwrapper/datacollect.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:35:46.569919 ctpwrapper-6.6.9.2/ctpwrapper/headers/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctpwrapper/headers/DataCollect.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    38616 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctpwrapper/headers/ThostFtdcUserApiDataType.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)   222333 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctpwrapper/headers/ThostFtdcUserApiStruct.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctpwrapper/headers/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctpwrapper/headers/cMdAPI.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    19840 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/ctpwrapper/headers/cTraderApi.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:35:46.569919 ctpwrapper-6.6.9.2/ctpwrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-04 14:35:46.000000 ctpwrapper-6.6.9.2/ctpwrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-04 14:35:46.000000 ctpwrapper-6.6.9.2/ctpwrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:35:46.000000 ctpwrapper-6.6.9.2/ctpwrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 14:35:46.000000 ctpwrapper-6.6.9.2/ctpwrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-04 14:35:46.573919 ctpwrapper-6.6.9.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5210 2023-07-04 14:35:38.000000 ctpwrapper-6.6.9.2/setup.py
```

### Comparing `ctpwrapper-6.6.9.1/LICENSE` & `ctpwrapper-6.6.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/PKG-INFO` & `ctpwrapper-6.6.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctpwrapper
-Version: 6.6.9.1
+Version: 6.6.9.2
 Summary: CTP client v6.6.5
 Home-page: https://github.com/nooperpudd/ctpwrapper
 Author: Winton Wang
 Author-email: 365504029@qq.com
 License: LGPLv3
 Keywords: CTP,Future,SHFE,Shanghai Future Exchange
 Platform: win32
@@ -31,26 +31,26 @@
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CTP期货 API Python Wrapper 
 
-[![Build Status](https://app.travis-ci.com/nooperpudd/ctpwrapper.svg?branch=master)](https://app.travis-ci.com/nooperpudd/ctpwrapper)
+[![build action](https://github.com/nooperpudd/ctpwrapper/actions/workflows/build.yaml/badge.svg?branch=master)](https://github.com/nooperpudd/ctpwrapper/actions/workflows/build.yaml)
 [![Build status](https://ci.appveyor.com/api/projects/status/gvvtcqsjo9nsw0ct/branch/master?svg=true)](https://ci.appveyor.com/project/nooperpudd/ctpwrapper)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/9ed5d0e55ed84dfeba30a7630ab5c160)](https://www.codacy.com/app/nooperpudd/ctpwrapper?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=nooperpudd/ctpwrapper&amp;utm_campaign=Badge_Grade)
 [![pypi](https://img.shields.io/pypi/v/ctpwrapper.svg)](https://pypi.python.org/pypi/ctpwrapper)
 [![status](https://img.shields.io/pypi/status/ctpwrapper.svg)](https://pypi.python.org/pypi/ctpwrapper)
 [![pyversion](https://img.shields.io/pypi/pyversions/ctpwrapper.svg)](https://pypi.python.org/pypi/ctpwrapper)
 [![implementation](https://img.shields.io/pypi/implementation/ctpwrapper.svg)](https://pypi.python.org/pypi/ctpwrapper)
 [![Downloads](https://pepy.tech/badge/ctpwrapper)](https://pepy.tech/project/ctpwrapper)
 
 [CTP Website](http://www.sfit.com.cn/5_2_DocumentDown_1.htm)
 
-Version: v6.6.9.1
+Version: v6.6.9.2
 
 Platform: Linux 64bit, Windows 64bit
 
 Python Requirement: x86-64
 
 **Especially Support PyPy3-3.6 Linux 64bit**
```

### Comparing `ctpwrapper-6.6.9.1/README.md` & `ctpwrapper-6.6.9.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # CTP期货 API Python Wrapper 
 
-[![Build Status](https://app.travis-ci.com/nooperpudd/ctpwrapper.svg?branch=master)](https://app.travis-ci.com/nooperpudd/ctpwrapper)
+[![build action](https://github.com/nooperpudd/ctpwrapper/actions/workflows/build.yaml/badge.svg?branch=master)](https://github.com/nooperpudd/ctpwrapper/actions/workflows/build.yaml)
 [![Build status](https://ci.appveyor.com/api/projects/status/gvvtcqsjo9nsw0ct/branch/master?svg=true)](https://ci.appveyor.com/project/nooperpudd/ctpwrapper)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/9ed5d0e55ed84dfeba30a7630ab5c160)](https://www.codacy.com/app/nooperpudd/ctpwrapper?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=nooperpudd/ctpwrapper&amp;utm_campaign=Badge_Grade)
 [![pypi](https://img.shields.io/pypi/v/ctpwrapper.svg)](https://pypi.python.org/pypi/ctpwrapper)
 [![status](https://img.shields.io/pypi/status/ctpwrapper.svg)](https://pypi.python.org/pypi/ctpwrapper)
 [![pyversion](https://img.shields.io/pypi/pyversions/ctpwrapper.svg)](https://pypi.python.org/pypi/ctpwrapper)
 [![implementation](https://img.shields.io/pypi/implementation/ctpwrapper.svg)](https://pypi.python.org/pypi/ctpwrapper)
 [![Downloads](https://pepy.tech/badge/ctpwrapper)](https://pepy.tech/project/ctpwrapper)
 
 [CTP Website](http://www.sfit.com.cn/5_2_DocumentDown_1.htm)
 
-Version: v6.6.9.1
+Version: v6.6.9.2
 
 Platform: Linux 64bit, Windows 64bit
 
 Python Requirement: x86-64
 
 **Especially Support PyPy3-3.6 Linux 64bit**
```

### Comparing `ctpwrapper-6.6.9.1/ctp/header/DataCollect.h` & `ctpwrapper-6.6.9.2/ctp/header/DataCollect.h`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctp/header/ThostFtdcMdApi.h` & `ctpwrapper-6.6.9.2/ctp/header/ThostFtdcMdApi.h`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctp/header/ThostFtdcTraderApi.h` & `ctpwrapper-6.6.9.2/ctp/header/ThostFtdcTraderApi.h`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctp/header/ThostFtdcUserApiDataType.h` & `ctpwrapper-6.6.9.2/ctp/header/ThostFtdcUserApiDataType.h`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctp/header/ThostFtdcUserApiStruct.h` & `ctpwrapper-6.6.9.2/ctp/header/ThostFtdcUserApiStruct.h`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctp/header/error.xml` & `ctpwrapper-6.6.9.2/ctp/header/error.xml`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctp/linux/libLinuxDataCollect.so` & `ctpwrapper-6.6.9.2/ctp/linux/libLinuxDataCollect.so`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctp/linux/libthostmduserapi_se.so` & `ctpwrapper-6.6.9.2/ctp/linux/libthostmduserapi_se.so`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctp/linux/libthosttraderapi_se.so` & `ctpwrapper-6.6.9.2/ctp/linux/libthosttraderapi_se.so`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctp/win/WinDataCollect.dll` & `ctpwrapper-6.6.9.2/ctp/win/WinDataCollect.dll`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctp/win/WinDataCollect.lib` & `ctpwrapper-6.6.9.2/ctp/win/WinDataCollect.lib`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctp/win/thostmduserapi_se.dll` & `ctpwrapper-6.6.9.2/ctp/win/thostmduserapi_se.dll`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctp/win/thostmduserapi_se.lib` & `ctpwrapper-6.6.9.2/ctp/win/thostmduserapi_se.lib`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctp/win/thosttraderapi_se.dll` & `ctpwrapper-6.6.9.2/ctp/win/thosttraderapi_se.dll`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctp/win/thosttraderapi_se.lib` & `ctpwrapper-6.6.9.2/ctp/win/thosttraderapi_se.lib`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctpwrapper/ApiStructure.py` & `ctpwrapper-6.6.9.2/ctpwrapper/ApiStructure.py`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctpwrapper/Md.py` & `ctpwrapper-6.6.9.2/ctpwrapper/Md.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,17 @@
     def Join(self) -> int:
         """
         等待接口线程结束运行
         @return 线程退出代码
         """
         return super(MdApiPy, self).Join()
 
+    def Release(self) -> None:
+        super(MdApiPy, self).Release()
+
     def ReqUserLogin(self, pReqUserLogin: "ReqUserLoginField", nRequestID: int) -> int:
         """
         用户登录请求
         """
         return super(MdApiPy, self).ReqUserLogin(pReqUserLogin, nRequestID)
 
     def ReqUserLogout(self, pUserLogout: "UserLogoutField", nRequestID: int) -> int:
```

### Comparing `ctpwrapper-6.6.9.1/ctpwrapper/MdApi.pyx` & `ctpwrapper-6.6.9.2/ctpwrapper/MdApi.pyx`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctpwrapper/Trader.py` & `ctpwrapper-6.6.9.2/ctpwrapper/Trader.py`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctpwrapper/TraderApi.pyx` & `ctpwrapper-6.6.9.2/ctpwrapper/TraderApi.pyx`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctpwrapper/__init__.py` & `ctpwrapper-6.6.9.2/ctpwrapper/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with ctpwrapper.  If not, see <http://www.gnu.org/licenses/>.
 
 """
-__version__ = "6.6.9.1"
+__version__ = "6.6.9.2"
 __date__ = "2021-09-24"
 
 from ctpwrapper.Md import MdApiPy
 from ctpwrapper.Trader import TraderApiPy
 
 from ctpwrapper.datacollect import GetSystemInfo, GetDataCollectApiVersion
```

### Comparing `ctpwrapper-6.6.9.1/ctpwrapper/base.py` & `ctpwrapper-6.6.9.2/ctpwrapper/base.py`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctpwrapper/cppheader/CMdAPI.h` & `ctpwrapper-6.6.9.2/ctpwrapper/cppheader/CMdAPI.h`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctpwrapper/cppheader/CTraderAPI.h` & `ctpwrapper-6.6.9.2/ctpwrapper/cppheader/CTraderAPI.h`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctpwrapper/headers/ThostFtdcUserApiDataType.pxd` & `ctpwrapper-6.6.9.2/ctpwrapper/headers/ThostFtdcUserApiDataType.pxd`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctpwrapper/headers/ThostFtdcUserApiStruct.pxd` & `ctpwrapper-6.6.9.2/ctpwrapper/headers/ThostFtdcUserApiStruct.pxd`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctpwrapper/headers/__init__.pxd` & `ctpwrapper-6.6.9.2/ctpwrapper/headers/__init__.pxd`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctpwrapper/headers/cMdAPI.pxd` & `ctpwrapper-6.6.9.2/ctpwrapper/headers/cMdAPI.pxd`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctpwrapper/headers/cTraderApi.pxd` & `ctpwrapper-6.6.9.2/ctpwrapper/headers/cTraderApi.pxd`

 * *Files identical despite different names*

### Comparing `ctpwrapper-6.6.9.1/ctpwrapper.egg-info/PKG-INFO` & `ctpwrapper-6.6.9.2/ctpwrapper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctpwrapper
-Version: 6.6.9.1
+Version: 6.6.9.2
 Summary: CTP client v6.6.5
 Home-page: https://github.com/nooperpudd/ctpwrapper
 Author: Winton Wang
 Author-email: 365504029@qq.com
 License: LGPLv3
 Keywords: CTP,Future,SHFE,Shanghai Future Exchange
 Platform: win32
@@ -31,26 +31,26 @@
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CTP期货 API Python Wrapper 
 
-[![Build Status](https://app.travis-ci.com/nooperpudd/ctpwrapper.svg?branch=master)](https://app.travis-ci.com/nooperpudd/ctpwrapper)
+[![build action](https://github.com/nooperpudd/ctpwrapper/actions/workflows/build.yaml/badge.svg?branch=master)](https://github.com/nooperpudd/ctpwrapper/actions/workflows/build.yaml)
 [![Build status](https://ci.appveyor.com/api/projects/status/gvvtcqsjo9nsw0ct/branch/master?svg=true)](https://ci.appveyor.com/project/nooperpudd/ctpwrapper)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/9ed5d0e55ed84dfeba30a7630ab5c160)](https://www.codacy.com/app/nooperpudd/ctpwrapper?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=nooperpudd/ctpwrapper&amp;utm_campaign=Badge_Grade)
 [![pypi](https://img.shields.io/pypi/v/ctpwrapper.svg)](https://pypi.python.org/pypi/ctpwrapper)
 [![status](https://img.shields.io/pypi/status/ctpwrapper.svg)](https://pypi.python.org/pypi/ctpwrapper)
 [![pyversion](https://img.shields.io/pypi/pyversions/ctpwrapper.svg)](https://pypi.python.org/pypi/ctpwrapper)
 [![implementation](https://img.shields.io/pypi/implementation/ctpwrapper.svg)](https://pypi.python.org/pypi/ctpwrapper)
 [![Downloads](https://pepy.tech/badge/ctpwrapper)](https://pepy.tech/project/ctpwrapper)
 
 [CTP Website](http://www.sfit.com.cn/5_2_DocumentDown_1.htm)
 
-Version: v6.6.9.1
+Version: v6.6.9.2
 
 Platform: Linux 64bit, Windows 64bit
 
 Python Requirement: x86-64
 
 **Especially Support PyPy3-3.6 Linux 64bit**
```

### Comparing `ctpwrapper-6.6.9.1/ctpwrapper.egg-info/SOURCES.txt` & `ctpwrapper-6.6.9.2/ctpwrapper.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -35,11 +35,8 @@
 ctpwrapper/cppheader/CMdAPI.h
 ctpwrapper/cppheader/CTraderAPI.h
 ctpwrapper/headers/DataCollect.pxd
 ctpwrapper/headers/ThostFtdcUserApiDataType.pxd
 ctpwrapper/headers/ThostFtdcUserApiStruct.pxd
 ctpwrapper/headers/__init__.pxd
 ctpwrapper/headers/cMdAPI.pxd
-ctpwrapper/headers/cTraderApi.pxd
-tests/test_api.py
-tests/test_datacollect.py
-tests/test_structure.py
+ctpwrapper/headers/cTraderApi.pxd
```

### Comparing `ctpwrapper-6.6.9.1/setup.py` & `ctpwrapper-6.6.9.2/setup.py`

 * *Files identical despite different names*

