# Comparing `tmp/alibabacloud_rds20140815-2.2.3.tar.gz` & `tmp/alibabacloud_rds20140815-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_rds20140815-2.2.3.tar", last modified: Tue Jul  4 03:30:06 2023, max compression
+gzip compressed data, was "dist/alibabacloud_rds20140815-2.2.4.tar", last modified: Tue Jul  4 15:10:17 2023, max compression
```

## Comparing `alibabacloud_rds20140815-2.2.3.tar` & `alibabacloud_rds20140815-2.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/
--rw-r--r--   0 root         (0) root         (0)     1443 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2328 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/alibabacloud_rds20140815/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/alibabacloud_rds20140815/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1662291 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/alibabacloud_rds20140815/client.py
--rw-r--r--   0 root         (0) root         (0)  2539902 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/alibabacloud_rds20140815/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/alibabacloud_rds20140815.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2328 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/alibabacloud_rds20140815.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/alibabacloud_rds20140815.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/alibabacloud_rds20140815.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/alibabacloud_rds20140815.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/alibabacloud_rds20140815.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2610 2023-07-04 03:30:06.000000 alibabacloud_rds20140815-2.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:10:17.000000 alibabacloud_rds20140815-2.2.4/
+-rw-r--r--   0 root         (0) root         (0)     1627 2023-07-04 15:10:16.000000 alibabacloud_rds20140815-2.2.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-04 15:10:16.000000 alibabacloud_rds20140815-2.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-04 15:10:16.000000 alibabacloud_rds20140815-2.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-07-04 15:10:17.000000 alibabacloud_rds20140815-2.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-04 15:10:16.000000 alibabacloud_rds20140815-2.2.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-04 15:10:16.000000 alibabacloud_rds20140815-2.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:10:17.000000 alibabacloud_rds20140815-2.2.4/alibabacloud_rds20140815/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 15:10:16.000000 alibabacloud_rds20140815-2.2.4/alibabacloud_rds20140815/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1662291 2023-07-04 15:10:16.000000 alibabacloud_rds20140815-2.2.4/alibabacloud_rds20140815/client.py
+-rw-r--r--   0 root         (0) root         (0)  2539902 2023-07-04 15:10:16.000000 alibabacloud_rds20140815-2.2.4/alibabacloud_rds20140815/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:10:17.000000 alibabacloud_rds20140815-2.2.4/alibabacloud_rds20140815.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-07-04 15:10:16.000000 alibabacloud_rds20140815-2.2.4/alibabacloud_rds20140815.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-04 15:10:16.000000 alibabacloud_rds20140815-2.2.4/alibabacloud_rds20140815.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 15:10:16.000000 alibabacloud_rds20140815-2.2.4/alibabacloud_rds20140815.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-04 15:10:16.000000 alibabacloud_rds20140815-2.2.4/alibabacloud_rds20140815.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-04 15:10:16.000000 alibabacloud_rds20140815-2.2.4/alibabacloud_rds20140815.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 15:10:17.000000 alibabacloud_rds20140815-2.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2610 2023-07-04 15:10:16.000000 alibabacloud_rds20140815-2.2.4/setup.py
```

### Comparing `alibabacloud_rds20140815-2.2.3/ChangeLog.md` & `alibabacloud_rds20140815-2.2.4/ChangeLog.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2023-07-04 Version: 2.2.3
+- ModifyBackupPolicy API support parameter BackupPriority.
+- DescribeBackupPolicy API add return parameters: BackupPriority and SupportModifyBackupPriority.
+
 2023-07-03 Version: 2.2.2
 - Fix bugs for  DescribeDedicatedHosts.
 - Fixed bugs add ERRORCODE.
 - Added serverless config to support serverless price query.
 
 2023-07-02 Version: 2.2.1
 - Fixed bugs for lack of regionId.
```

### Comparing `alibabacloud_rds20140815-2.2.3/LICENSE` & `alibabacloud_rds20140815-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.3/PKG-INFO` & `alibabacloud_rds20140815-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_rds20140815
-Version: 2.2.3
+Version: 2.2.4
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815-2.2.3/README-CN.md` & `alibabacloud_rds20140815-2.2.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.3/README.md` & `alibabacloud_rds20140815-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.3/alibabacloud_rds20140815/client.py` & `alibabacloud_rds20140815-2.2.4/alibabacloud_rds20140815/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.3/alibabacloud_rds20140815/models.py` & `alibabacloud_rds20140815-2.2.4/alibabacloud_rds20140815/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.3/alibabacloud_rds20140815.egg-info/PKG-INFO` & `alibabacloud_rds20140815-2.2.4/alibabacloud_rds20140815.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-rds20140815
-Version: 2.2.3
+Version: 2.2.4
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815-2.2.3/setup.py` & `alibabacloud_rds20140815-2.2.4/setup.py`

 * *Files identical despite different names*

