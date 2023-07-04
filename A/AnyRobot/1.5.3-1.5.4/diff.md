# Comparing `tmp/AnyRobot-1.5.3.tar.gz` & `tmp/AnyRobot-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\AnyRobot-1.5.3.tar", last modified: Tue Jun 27 07:53:19 2023, max compression
+gzip compressed data, was "dist\AnyRobot-1.5.4.tar", last modified: Tue Jul  4 06:36:34 2023, max compression
```

## Comparing `AnyRobot-1.5.3.tar` & `AnyRobot-1.5.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 07:53:19.328481 AnyRobot-1.5.3/
-drwxrwxrwx   0        0        0        0 2023-06-27 07:53:19.272481 AnyRobot-1.5.3/AnyRobot.egg-info/
--rw-rw-rw-   0        0        0      880 2023-06-27 07:53:19.000000 AnyRobot-1.5.3/AnyRobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1564 2023-06-27 07:53:19.000000 AnyRobot-1.5.3/AnyRobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 07:53:19.000000 AnyRobot-1.5.3/AnyRobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-27 07:53:19.000000 AnyRobot-1.5.3/AnyRobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      880 2023-06-27 07:53:19.327481 AnyRobot-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0      150 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-27 07:53:19.276483 AnyRobot-1.5.3/aishu/
--rw-rw-rw-   0        0        0        0 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/__init__.py
--rw-rw-rw-   0        0        0     1554 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/anyrobot.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:53:19.278482 AnyRobot-1.5.3/aishu/datafaker/
--rw-rw-rw-   0        0        0        0 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:53:19.281482 AnyRobot-1.5.3/aishu/datafaker/anyrobot/
--rw-rw-rw-   0        0        0        0 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/anyrobot/__init__.py
--rw-rw-rw-   0        0        0      615 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/anyrobot/getSqlVaule.py
--rw-rw-rw-   0        0        0    10120 2023-06-27 07:09:25.000000 AnyRobot-1.5.3/aishu/datafaker/anyrobot/sqlMapping.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:53:19.283483 AnyRobot-1.5.3/aishu/datafaker/profession/
--rw-rw-rw-   0        0        0        0 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:53:19.318484 AnyRobot-1.5.3/aishu/datafaker/profession/entity/
--rw-rw-rw-   0        0        0     2095 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/AssociationMapping.py
--rw-rw-rw-   0        0        0     1346 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/CreateTestPort.py
--rw-rw-rw-   0        0        0     2806 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/DataManage.py
--rw-rw-rw-   0        0        0     9755 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/ParaDateFiled.py
--rw-rw-rw-   0        0        0     3367 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/RetrievesAssociated.py
--rw-rw-rw-   0        0        0        0 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/__init__.py
--rw-rw-rw-   0        0        0     1516 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/agent.py
--rw-rw-rw-   0        0        0     1361 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/arPort.py
--rw-rw-rw-   0        0        0      543 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/databaseInfo.py
--rw-rw-rw-   0        0        0      225 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/date.py
--rw-rw-rw-   0        0        0      910 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/id.py
--rw-rw-rw-   0        0        0     1611 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/index.py
--rw-rw-rw-   0        0        0     1980 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/ip.py
--rw-rw-rw-   0        0        0    56391 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/kai.py
--rw-rw-rw-   0        0        0      232 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/ml.py
--rw-rw-rw-   0        0        0      314 2023-04-04 08:27:02.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/name.py
--rw-rw-rw-   0        0        0     1163 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/objectManager.py
--rw-rw-rw-   0        0        0     2869 2023-06-27 07:50:23.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/port.py
--rw-rw-rw-   0        0        0      128 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/switch.py
--rw-rw-rw-   0        0        0      264 2023-04-04 08:08:53.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/testMail.py
--rw-rw-rw-   0        0        0      995 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/timestamp.py
--rw-rw-rw-   0        0        0     5969 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/datafaker/profession/entity/zx.py
--rw-rw-rw-   0        0        0     5946 2023-06-27 07:09:42.000000 AnyRobot-1.5.3/aishu/datafaker/profession/getFiledValue.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:53:19.326484 AnyRobot-1.5.3/aishu/public/
--rw-rw-rw-   0        0        0        0 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/public/__init__.py
--rw-rw-rw-   0        0        0      366 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/public/db_select.py
--rw-rw-rw-   0        0        0     1653 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/public/mysql_pool.py
--rw-rw-rw-   0        0        0      476 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/public/operationJson.py
--rw-rw-rw-   0        0        0      250 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/public/urlJoin.py
--rw-rw-rw-   0        0        0      427 2022-12-02 08:25:16.000000 AnyRobot-1.5.3/aishu/setting.py
--rw-rw-rw-   0        0        0       42 2023-06-27 07:53:19.328481 AnyRobot-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1147 2023-06-27 07:52:18.000000 AnyRobot-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 06:36:34.746352 AnyRobot-1.5.4/
+drwxrwxrwx   0        0        0        0 2023-07-04 06:36:34.676352 AnyRobot-1.5.4/AnyRobot.egg-info/
+-rw-rw-rw-   0        0        0      880 2023-07-04 06:36:34.000000 AnyRobot-1.5.4/AnyRobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1564 2023-07-04 06:36:34.000000 AnyRobot-1.5.4/AnyRobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 06:36:34.000000 AnyRobot-1.5.4/AnyRobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-04 06:36:34.000000 AnyRobot-1.5.4/AnyRobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      880 2023-07-04 06:36:34.744352 AnyRobot-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-04 06:36:34.679353 AnyRobot-1.5.4/aishu/
+-rw-rw-rw-   0        0        0        0 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/__init__.py
+-rw-rw-rw-   0        0        0     1554 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/anyrobot.py
+drwxrwxrwx   0        0        0        0 2023-07-04 06:36:34.682352 AnyRobot-1.5.4/aishu/datafaker/
+-rw-rw-rw-   0        0        0        0 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 06:36:34.684352 AnyRobot-1.5.4/aishu/datafaker/anyrobot/
+-rw-rw-rw-   0        0        0        0 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/anyrobot/__init__.py
+-rw-rw-rw-   0        0        0      615 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/anyrobot/getSqlVaule.py
+-rw-rw-rw-   0        0        0    10120 2023-06-27 07:09:25.000000 AnyRobot-1.5.4/aishu/datafaker/anyrobot/sqlMapping.py
+drwxrwxrwx   0        0        0        0 2023-07-04 06:36:34.690356 AnyRobot-1.5.4/aishu/datafaker/profession/
+-rw-rw-rw-   0        0        0        0 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 06:36:34.737352 AnyRobot-1.5.4/aishu/datafaker/profession/entity/
+-rw-rw-rw-   0        0        0     2095 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/AssociationMapping.py
+-rw-rw-rw-   0        0        0     1346 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/CreateTestPort.py
+-rw-rw-rw-   0        0        0     2806 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/DataManage.py
+-rw-rw-rw-   0        0        0     9755 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/ParaDateFiled.py
+-rw-rw-rw-   0        0        0     3367 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/RetrievesAssociated.py
+-rw-rw-rw-   0        0        0        0 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/__init__.py
+-rw-rw-rw-   0        0        0     1516 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/agent.py
+-rw-rw-rw-   0        0        0     1361 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/arPort.py
+-rw-rw-rw-   0        0        0      543 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/databaseInfo.py
+-rw-rw-rw-   0        0        0      225 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/date.py
+-rw-rw-rw-   0        0        0      910 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/id.py
+-rw-rw-rw-   0        0        0     1611 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/index.py
+-rw-rw-rw-   0        0        0     1980 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/ip.py
+-rw-rw-rw-   0        0        0    56391 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/kai.py
+-rw-rw-rw-   0        0        0      232 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/ml.py
+-rw-rw-rw-   0        0        0      314 2023-04-04 08:27:02.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/name.py
+-rw-rw-rw-   0        0        0     1163 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/objectManager.py
+-rw-rw-rw-   0        0        0     2869 2023-06-27 07:50:23.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/port.py
+-rw-rw-rw-   0        0        0      128 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/switch.py
+-rw-rw-rw-   0        0        0      263 2023-07-04 06:35:01.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/testMail.py
+-rw-rw-rw-   0        0        0      995 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/timestamp.py
+-rw-rw-rw-   0        0        0     5969 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/datafaker/profession/entity/zx.py
+-rw-rw-rw-   0        0        0     5946 2023-06-27 07:09:42.000000 AnyRobot-1.5.4/aishu/datafaker/profession/getFiledValue.py
+drwxrwxrwx   0        0        0        0 2023-07-04 06:36:34.743357 AnyRobot-1.5.4/aishu/public/
+-rw-rw-rw-   0        0        0        0 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/public/__init__.py
+-rw-rw-rw-   0        0        0      366 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/public/db_select.py
+-rw-rw-rw-   0        0        0     1653 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/public/mysql_pool.py
+-rw-rw-rw-   0        0        0      476 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/public/operationJson.py
+-rw-rw-rw-   0        0        0      250 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/public/urlJoin.py
+-rw-rw-rw-   0        0        0      427 2022-12-02 08:25:16.000000 AnyRobot-1.5.4/aishu/setting.py
+-rw-rw-rw-   0        0        0       42 2023-07-04 06:36:34.746352 AnyRobot-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1147 2023-07-04 06:36:09.000000 AnyRobot-1.5.4/setup.py
```

### Comparing `AnyRobot-1.5.3/AnyRobot.egg-info/PKG-INFO` & `AnyRobot-1.5.4/AnyRobot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: AnyRobot
-Version: 1.5.3
+Version: 1.5.4
 Summary: This is a data service module that solves test data problems.
 Home-page: https://mp.weixin.qq.com/s/v6FS96ifCoMvp_rwrhzhKw
 Author: Evan.hu
 Author-email: 1056212287@qq.com
 License: BSD License
 Description: # Example Package
         This is a data service module that solves test data problems. You can use it.
```

### Comparing `AnyRobot-1.5.3/AnyRobot.egg-info/SOURCES.txt` & `AnyRobot-1.5.4/AnyRobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/PKG-INFO` & `AnyRobot-1.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: AnyRobot
-Version: 1.5.3
+Version: 1.5.4
 Summary: This is a data service module that solves test data problems.
 Home-page: https://mp.weixin.qq.com/s/v6FS96ifCoMvp_rwrhzhKw
 Author: Evan.hu
 Author-email: 1056212287@qq.com
 License: BSD License
 Description: # Example Package
         This is a data service module that solves test data problems. You can use it.
```

### Comparing `AnyRobot-1.5.3/aishu/anyrobot.py` & `AnyRobot-1.5.4/aishu/anyrobot.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/anyrobot/getSqlVaule.py` & `AnyRobot-1.5.4/aishu/datafaker/anyrobot/getSqlVaule.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/anyrobot/sqlMapping.py` & `AnyRobot-1.5.4/aishu/datafaker/anyrobot/sqlMapping.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/profession/entity/AssociationMapping.py` & `AnyRobot-1.5.4/aishu/datafaker/profession/entity/AssociationMapping.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/profession/entity/CreateTestPort.py` & `AnyRobot-1.5.4/aishu/datafaker/profession/entity/CreateTestPort.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/profession/entity/DataManage.py` & `AnyRobot-1.5.4/aishu/datafaker/profession/entity/DataManage.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/profession/entity/ParaDateFiled.py` & `AnyRobot-1.5.4/aishu/datafaker/profession/entity/ParaDateFiled.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/profession/entity/RetrievesAssociated.py` & `AnyRobot-1.5.4/aishu/datafaker/profession/entity/RetrievesAssociated.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/profession/entity/agent.py` & `AnyRobot-1.5.4/aishu/datafaker/profession/entity/agent.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/profession/entity/arPort.py` & `AnyRobot-1.5.4/aishu/datafaker/profession/entity/arPort.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/profession/entity/databaseInfo.py` & `AnyRobot-1.5.4/aishu/datafaker/profession/entity/databaseInfo.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/profession/entity/id.py` & `AnyRobot-1.5.4/aishu/datafaker/profession/entity/id.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/profession/entity/index.py` & `AnyRobot-1.5.4/aishu/datafaker/profession/entity/index.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/profession/entity/ip.py` & `AnyRobot-1.5.4/aishu/datafaker/profession/entity/ip.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/profession/entity/kai.py` & `AnyRobot-1.5.4/aishu/datafaker/profession/entity/kai.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/profession/entity/objectManager.py` & `AnyRobot-1.5.4/aishu/datafaker/profession/entity/objectManager.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/profession/entity/port.py` & `AnyRobot-1.5.4/aishu/datafaker/profession/entity/port.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/profession/entity/timestamp.py` & `AnyRobot-1.5.4/aishu/datafaker/profession/entity/timestamp.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/profession/entity/zx.py` & `AnyRobot-1.5.4/aishu/datafaker/profession/entity/zx.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/datafaker/profession/getFiledValue.py` & `AnyRobot-1.5.4/aishu/datafaker/profession/getFiledValue.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/aishu/public/mysql_pool.py` & `AnyRobot-1.5.4/aishu/public/mysql_pool.py`

 * *Files identical despite different names*

### Comparing `AnyRobot-1.5.3/setup.py` & `AnyRobot-1.5.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages
 
 here = os.path.abspath(os.path.dirname(__file__)) + os.path.sep + 'README.rst'
 
 with open(here, "r") as f:
   long_description = f.read()
 setup(name='AnyRobot',
-      version='1.5.3',
+      version='1.5.4',
       description='This is a data service module that solves test data problems.',
       long_description=long_description,
       author='Evan.hu',
       author_email='1056212287@qq.com',
       url='https://mp.weixin.qq.com/s/v6FS96ifCoMvp_rwrhzhKw',
       install_requires=[],
       license='BSD License',
```

