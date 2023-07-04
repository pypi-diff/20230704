# Comparing `tmp/alibabacloud_rds20140815_py2-1.1.4.tar.gz` & `tmp/alibabacloud_rds20140815_py2-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_rds20140815_py2-1.1.4.tar", last modified: Tue Jul  4 03:29:42 2023, max compression
+gzip compressed data, was "dist/alibabacloud_rds20140815_py2-1.1.5.tar", last modified: Tue Jul  4 15:10:09 2023, max compression
```

## Comparing `alibabacloud_rds20140815_py2-1.1.4.tar` & `alibabacloud_rds20140815_py2-1.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 03:29:42.000000 alibabacloud_rds20140815_py2-1.1.4/
--rw-r--r--   0 root         (0) root         (0)     1032 2023-07-04 03:29:41.000000 alibabacloud_rds20140815_py2-1.1.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-04 03:29:41.000000 alibabacloud_rds20140815_py2-1.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-04 03:29:41.000000 alibabacloud_rds20140815_py2-1.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2472 2023-07-04 03:29:42.000000 alibabacloud_rds20140815_py2-1.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-07-04 03:29:41.000000 alibabacloud_rds20140815_py2-1.1.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-07-04 03:29:41.000000 alibabacloud_rds20140815_py2-1.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 03:29:42.000000 alibabacloud_rds20140815_py2-1.1.4/alibabacloud_rds20140815/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 03:29:41.000000 alibabacloud_rds20140815_py2-1.1.4/alibabacloud_rds20140815/__init__.py
--rw-r--r--   0 root         (0) root         (0)   752829 2023-07-04 03:29:41.000000 alibabacloud_rds20140815_py2-1.1.4/alibabacloud_rds20140815/client.py
--rw-r--r--   0 root         (0) root         (0)  2561990 2023-07-04 03:29:41.000000 alibabacloud_rds20140815_py2-1.1.4/alibabacloud_rds20140815/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 03:29:42.000000 alibabacloud_rds20140815_py2-1.1.4/alibabacloud_rds20140815_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2472 2023-07-04 03:29:41.000000 alibabacloud_rds20140815_py2-1.1.4/alibabacloud_rds20140815_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-07-04 03:29:41.000000 alibabacloud_rds20140815_py2-1.1.4/alibabacloud_rds20140815_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 03:29:41.000000 alibabacloud_rds20140815_py2-1.1.4/alibabacloud_rds20140815_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-04 03:29:41.000000 alibabacloud_rds20140815_py2-1.1.4/alibabacloud_rds20140815_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-04 03:29:41.000000 alibabacloud_rds20140815_py2-1.1.4/alibabacloud_rds20140815_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 03:29:42.000000 alibabacloud_rds20140815_py2-1.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2903 2023-07-04 03:29:41.000000 alibabacloud_rds20140815_py2-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/
+-rw-r--r--   0 root         (0) root         (0)     1216 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/alibabacloud_rds20140815/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/alibabacloud_rds20140815/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   752829 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/alibabacloud_rds20140815/client.py
+-rw-r--r--   0 root         (0) root         (0)  2561990 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/alibabacloud_rds20140815/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/alibabacloud_rds20140815_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/alibabacloud_rds20140815_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/alibabacloud_rds20140815_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/alibabacloud_rds20140815_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/alibabacloud_rds20140815_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/alibabacloud_rds20140815_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-07-04 15:10:09.000000 alibabacloud_rds20140815_py2-1.1.5/setup.py
```

### Comparing `alibabacloud_rds20140815_py2-1.1.4/ChangeLog.md` & `alibabacloud_rds20140815_py2-1.1.5/ChangeLog.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2023-07-04 Version: 1.1.4
+- ModifyBackupPolicy API support parameter BackupPriority.
+- DescribeBackupPolicy API add return parameters: BackupPriority and SupportModifyBackupPriority.
+
 2023-07-03 Version: 1.1.3
 - Fix bugs for  DescribeDedicatedHosts.
 - Fixed bugs add ERRORCODE.
 - Added serverless config to support serverless price query.
 
 2023-07-02 Version: 1.1.2
 - Fixed bugs for lack of regionId.
```

### Comparing `alibabacloud_rds20140815_py2-1.1.4/LICENSE` & `alibabacloud_rds20140815_py2-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.1.4/PKG-INFO` & `alibabacloud_rds20140815_py2-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_rds20140815_py2
-Version: 1.1.4
+Version: 1.1.5
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815_py2-1.1.4/README-CN.md` & `alibabacloud_rds20140815_py2-1.1.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.1.4/README.md` & `alibabacloud_rds20140815_py2-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.1.4/alibabacloud_rds20140815/client.py` & `alibabacloud_rds20140815_py2-1.1.5/alibabacloud_rds20140815/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.1.4/alibabacloud_rds20140815/models.py` & `alibabacloud_rds20140815_py2-1.1.5/alibabacloud_rds20140815/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.1.4/alibabacloud_rds20140815_py2.egg-info/PKG-INFO` & `alibabacloud_rds20140815_py2-1.1.5/alibabacloud_rds20140815_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-rds20140815-py2
-Version: 1.1.4
+Version: 1.1.5
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815_py2-1.1.4/setup.py` & `alibabacloud_rds20140815_py2-1.1.5/setup.py`

 * *Files identical despite different names*

