# Comparing `tmp/cmem_cmempy-23.1.1.tar.gz` & `tmp/cmem_cmempy-23.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_cmempy-23.1.1.tar", max compression
+gzip compressed data, was "cmem_cmempy-23.1.2rc1.tar", max compression
```

## Comparing `cmem_cmempy-23.1.1.tar` & `cmem_cmempy-23.1.2rc1.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0    11357 2023-01-04 14:59:14.088341 cmem_cmempy-23.1.1/LICENSE
--rw-r--r--   0        0        0      651 2023-06-13 18:26:21.198608 cmem_cmempy-23.1.1/README-public.md
--rw-r--r--   0        0        0      110 2023-01-04 14:59:14.088607 cmem_cmempy-23.1.1/cmem/__init__.py
--rw-r--r--   0        0        0       40 2023-01-04 14:59:14.088681 cmem_cmempy-23.1.1/cmem/cmempy/__init__.py
--rw-r--r--   0        0        0     4456 2023-04-27 06:10:06.372985 cmem_cmempy-23.1.1/cmem/cmempy/api.py
--rw-r--r--   0        0        0     4970 2023-04-27 06:10:06.373356 cmem_cmempy-23.1.1/cmem/cmempy/config.py
--rw-r--r--   0        0        0     1062 2023-01-04 14:59:14.088909 cmem_cmempy-23.1.1/cmem/cmempy/custom_tasks/__init__.py
--rw-r--r--   0        0        0       36 2023-01-04 14:59:14.088982 cmem_cmempy-23.1.1/cmem/cmempy/dp/__init__.py
--rw-r--r--   0        0        0     1029 2023-01-04 14:59:14.089065 cmem_cmempy-23.1.1/cmem/cmempy/dp/admin/__init__.py
--rw-r--r--   0        0        0     1014 2023-01-04 14:59:14.089117 cmem_cmempy-23.1.1/cmem/cmempy/dp/admin/backup.py
--rw-r--r--   0        0        0       42 2023-01-04 14:59:14.089196 cmem_cmempy-23.1.1/cmem/cmempy/dp/authorization/__init__.py
--rw-r--r--   0        0        0     1232 2023-01-04 14:59:14.089259 cmem_cmempy-23.1.1/cmem/cmempy/dp/authorization/conditions.py
--rw-r--r--   0        0        0      477 2023-01-04 14:59:14.089322 cmem_cmempy-23.1.1/cmem/cmempy/dp/authorization/refresh.py
--rw-r--r--   0        0        0      380 2023-01-04 14:59:14.089401 cmem_cmempy-23.1.1/cmem/cmempy/dp/proxy/__init__.py
--rw-r--r--   0        0        0     6036 2023-01-04 14:59:14.089475 cmem_cmempy-23.1.1/cmem/cmempy/dp/proxy/graph.py
--rw-r--r--   0        0        0     4159 2023-01-04 14:59:14.089530 cmem_cmempy-23.1.1/cmem/cmempy/dp/proxy/sparql.py
--rw-r--r--   0        0        0     1244 2023-01-04 14:59:14.089583 cmem_cmempy-23.1.1/cmem/cmempy/dp/proxy/update.py
--rw-r--r--   0        0        0     1011 2023-01-04 14:59:14.089671 cmem_cmempy-23.1.1/cmem/cmempy/dp/titles/__init__.py
--rw-r--r--   0        0        0     5905 2023-01-04 14:59:14.089779 cmem_cmempy-23.1.1/cmem/cmempy/health/__init__.py
--rw-r--r--   0        0        0      519 2023-04-27 06:10:06.373437 cmem_cmempy-23.1.1/cmem/cmempy/keycloak/group.py
--rw-r--r--   0        0        0     3630 2023-06-13 18:49:23.475724 cmem_cmempy-23.1.1/cmem/cmempy/keycloak/user.py
--rw-r--r--   0        0        0       31 2023-01-04 14:59:14.089861 cmem_cmempy-23.1.1/cmem/cmempy/linking/__init__.py
--rw-r--r--   0        0        0     2588 2023-01-04 14:59:14.089928 cmem_cmempy-23.1.1/cmem/cmempy/linking/linkingtask.py
--rw-r--r--   0        0        0       26 2023-01-04 14:59:14.090002 cmem_cmempy-23.1.1/cmem/cmempy/plugins/__init__.py
--rw-r--r--   0        0        0     1939 2023-01-04 14:59:14.090063 cmem_cmempy-23.1.1/cmem/cmempy/plugins/marshalling.py
--rw-r--r--   0        0        0    11190 2023-04-27 06:10:06.373634 cmem_cmempy-23.1.1/cmem/cmempy/queries/__init__.py
--rw-r--r--   0        0        0       33 2023-01-04 14:59:14.090285 cmem_cmempy-23.1.1/cmem/cmempy/transform/__init__.py
--rw-r--r--   0        0        0     1090 2023-01-04 14:59:14.090388 cmem_cmempy-23.1.1/cmem/cmempy/transform/rules/__init__.py
--rw-r--r--   0        0        0     1075 2023-01-04 14:59:14.090439 cmem_cmempy-23.1.1/cmem/cmempy/transform/rules/transformationrule.py
--rw-r--r--   0        0        0     1240 2023-01-04 14:59:14.090495 cmem_cmempy-23.1.1/cmem/cmempy/transform/transformationtask.py
--rw-r--r--   0        0        0     3597 2023-01-05 19:05:10.883204 cmem_cmempy-23.1.1/cmem/cmempy/vocabularies/__init__.py
--rw-r--r--   0        0        0      500 2023-01-04 14:59:14.090681 cmem_cmempy-23.1.1/cmem/cmempy/workflow/__init__.py
--rw-r--r--   0        0        0     4502 2023-01-04 14:59:14.090748 cmem_cmempy-23.1.1/cmem/cmempy/workflow/workflow.py
--rw-r--r--   0        0        0      131 2023-01-04 14:59:14.090794 cmem_cmempy-23.1.1/cmem/cmempy/workflow/workflows.py
--rw-r--r--   0        0        0     1873 2023-01-04 14:59:14.090883 cmem_cmempy-23.1.1/cmem/cmempy/workspace/__init__.py
--rw-r--r--   0        0        0      340 2023-01-04 14:59:14.090960 cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/__init__.py
--rw-r--r--   0        0        0      914 2023-01-04 14:59:14.091021 cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/projectactivities.py
--rw-r--r--   0        0        0     2281 2023-01-04 14:59:14.091080 cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/projectactivity.py
--rw-r--r--   0        0        0     3164 2023-01-04 14:59:14.091146 cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/taskactivities.py
--rw-r--r--   0        0        0     2323 2023-01-04 14:59:14.091194 cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/taskactivity.py
--rw-r--r--   0        0        0      744 2023-01-04 14:59:14.091271 cmem_cmempy-23.1.1/cmem/cmempy/workspace/export_/__init__.py
--rw-r--r--   0        0        0     1540 2023-01-04 14:59:14.091352 cmem_cmempy-23.1.1/cmem/cmempy/workspace/import_/__init__.py
--rw-r--r--   0        0        0      454 2023-01-04 14:59:14.091425 cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/__init__.py
--rw-r--r--   0        0        0       45 2023-01-04 14:59:14.091506 cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/datasets/__init__.py
--rw-r--r--   0        0        0     2369 2023-01-04 14:59:14.091570 cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/datasets/dataset.py
--rw-r--r--   0        0        0      748 2023-01-04 14:59:14.091621 cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/export_.py
--rw-r--r--   0        0        0     4945 2023-01-04 14:59:14.091685 cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/import_.py
--rw-r--r--   0        0        0     2007 2023-01-04 14:59:14.091735 cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/project.py
--rw-r--r--   0        0        0      960 2023-04-27 06:10:06.373750 cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/resources/__init__.py
--rw-r--r--   0        0        0     6089 2023-04-27 06:10:06.373861 cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/resources/resource.py
--rw-r--r--   0        0        0     2292 2023-01-04 14:59:14.091934 cmem_cmempy-23.1.1/cmem/cmempy/workspace/python.py
--rw-r--r--   0        0        0     1075 2023-01-04 14:59:14.092020 cmem_cmempy-23.1.1/cmem/cmempy/workspace/search/__init__.py
--rw-r--r--   0        0        0     1078 2023-01-04 14:59:14.092095 cmem_cmempy-23.1.1/cmem/cmempy/workspace/tasks/__init__.py
--rw-r--r--   0        0        0     2042 2023-06-13 18:49:40.640308 cmem_cmempy-23.1.1/pyproject.toml
--rw-r--r--   0        0        0     1938 1970-01-01 00:00:00.000000 cmem_cmempy-23.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/LICENSE
+-rw-r--r--   0        0        0      651 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/README-public.md
+-rw-r--r--   0        0        0      110 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/__init__.py
+-rw-r--r--   0        0        0       40 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/__init__.py
+-rw-r--r--   0        0        0     4456 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/api.py
+-rw-r--r--   0        0        0     4970 2023-04-20 02:23:54.204292 cmem_cmempy-23.1.2rc1/cmem/cmempy/config.py
+-rw-r--r--   0        0        0     1062 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/custom_tasks/__init__.py
+-rw-r--r--   0        0        0       36 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/__init__.py
+-rw-r--r--   0        0        0     1029 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/admin/__init__.py
+-rw-r--r--   0        0        0     1014 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/admin/backup.py
+-rw-r--r--   0        0        0       42 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/authorization/__init__.py
+-rw-r--r--   0        0        0     1232 2023-05-26 11:56:38.147641 cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/authorization/conditions.py
+-rw-r--r--   0        0        0      477 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/authorization/refresh.py
+-rw-r--r--   0        0        0      380 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/proxy/__init__.py
+-rw-r--r--   0        0        0     6036 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/proxy/graph.py
+-rw-r--r--   0        0        0     4159 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/proxy/sparql.py
+-rw-r--r--   0        0        0     1244 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/proxy/update.py
+-rw-r--r--   0        0        0     1011 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/titles/__init__.py
+-rw-r--r--   0        0        0     5905 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/health/__init__.py
+-rw-r--r--   0        0        0      519 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/keycloak/group.py
+-rw-r--r--   0        0        0     4500 2023-07-03 02:45:49.031379 cmem_cmempy-23.1.2rc1/cmem/cmempy/keycloak/user.py
+-rw-r--r--   0        0        0       31 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/linking/__init__.py
+-rw-r--r--   0        0        0     2588 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/linking/linkingtask.py
+-rw-r--r--   0        0        0       26 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/plugins/__init__.py
+-rw-r--r--   0        0        0     1939 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/plugins/marshalling.py
+-rw-r--r--   0        0        0    11190 2023-04-05 05:40:40.672801 cmem_cmempy-23.1.2rc1/cmem/cmempy/queries/__init__.py
+-rw-r--r--   0        0        0       33 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/transform/__init__.py
+-rw-r--r--   0        0        0     1090 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/transform/rules/__init__.py
+-rw-r--r--   0        0        0     1075 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/transform/rules/transformationrule.py
+-rw-r--r--   0        0        0     1240 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/transform/transformationtask.py
+-rw-r--r--   0        0        0     3597 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/vocabularies/__init__.py
+-rw-r--r--   0        0        0      731 2023-06-30 08:10:14.989981 cmem_cmempy-23.1.2rc1/cmem/cmempy/workflow/__init__.py
+-rw-r--r--   0        0        0     4891 2023-07-03 12:45:18.840911 cmem_cmempy-23.1.2rc1/cmem/cmempy/workflow/workflow.py
+-rw-r--r--   0        0        0      131 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/workflow/workflows.py
+-rw-r--r--   0        0        0     1873 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/__init__.py
+-rw-r--r--   0        0        0      340 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/activities/__init__.py
+-rw-r--r--   0        0        0      914 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/activities/projectactivities.py
+-rw-r--r--   0        0        0     2281 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/activities/projectactivity.py
+-rw-r--r--   0        0        0     3164 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/activities/taskactivities.py
+-rw-r--r--   0        0        0     2323 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/activities/taskactivity.py
+-rw-r--r--   0        0        0      744 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/export_/__init__.py
+-rw-r--r--   0        0        0     1540 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/import_/__init__.py
+-rw-r--r--   0        0        0      454 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/projects/__init__.py
+-rw-r--r--   0        0        0       45 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/projects/datasets/__init__.py
+-rw-r--r--   0        0        0     4150 2023-07-04 11:11:24.990283 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/projects/datasets/dataset.py
+-rw-r--r--   0        0        0      748 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/projects/export_.py
+-rw-r--r--   0        0        0     4945 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/projects/import_.py
+-rw-r--r--   0        0        0     2007 2023-06-05 12:52:07.523183 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/projects/project.py
+-rw-r--r--   0        0        0      960 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/projects/resources/__init__.py
+-rw-r--r--   0        0        0     6089 2023-06-30 08:10:14.989981 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/projects/resources/resource.py
+-rw-r--r--   0        0        0     2292 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/python.py
+-rw-r--r--   0        0        0     1075 2023-04-05 05:40:40.676801 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/search/__init__.py
+-rw-r--r--   0        0        0     2087 2023-07-03 12:45:18.844911 cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/tasks/__init__.py
+-rw-r--r--   0        0        0     2099 2023-07-04 11:12:13.034822 cmem_cmempy-23.1.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 cmem_cmempy-23.1.2rc1/setup.py
+-rw-r--r--   0        0        0     2045 1970-01-01 00:00:00.000000 cmem_cmempy-23.1.2rc1/PKG-INFO
```

### Comparing `cmem_cmempy-23.1.1/LICENSE` & `cmem_cmempy-23.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/README-public.md` & `cmem_cmempy-23.1.2rc1/README-public.md`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/api.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/api.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/config.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/config.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/custom_tasks/__init__.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/custom_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/dp/admin/__init__.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/dp/admin/backup.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/admin/backup.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/dp/authorization/conditions.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/authorization/conditions.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/dp/proxy/graph.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/proxy/graph.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/dp/proxy/sparql.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/proxy/sparql.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/dp/proxy/update.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/proxy/update.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/dp/titles/__init__.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/dp/titles/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/health/__init__.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/health/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/keycloak/group.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/keycloak/group.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/keycloak/user.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/keycloak/user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 API method to manage cmem realm users
 """
 import json
 from json import loads
 from typing import Optional
 
+from email_validator import validate_email, EmailNotValidError
+
 from cmem.cmempy import config
 from cmem.cmempy.api import send_request
 
 
 def get_users_uri():
     """Get endpoint URI for user list."""
     path = f"/admin/realms/{config.get_keycloak_realm_id()}/users"
@@ -29,30 +31,59 @@
 
 def get_user_groups_uri():
     """Get endpoint URI pattern for a user group list."""
     path = f"{get_user_uri()}/groups"
     return path
 
 
+def get_execute_actions_email_uri():
+    """Get endpoint URI pattern for a execute actions email."""
+    path = f"{get_user_uri()}/execute-actions-email"
+    return path
+
+
 def list_users(params=None):
     """List users in cmem realm."""
     uri = get_users_uri()
     list_request = send_request(uri, method="GET", params=params)
     return loads(list_request)
 
 
+def request_password_change(user_id):
+    """Email to update the password"""
+    uri = get_execute_actions_email_uri().format(user_id)
+    headers = {"Content-Type": "application/json"}
+    data = ["UPDATE_PASSWORD"]
+    json_data = json.dumps(data).encode("utf-8")
+    send_request(uri=uri, method="PUT", headers=headers, data=json_data)
+
+
 def create_user(username):
     """create user to cmem relam"""
-    data = {"username": username, "enabled": True}
+    data = {
+        "username": username,
+        "email": _get_normalized_email(username),
+        "enabled": True,
+    }
+
     uri = get_users_uri()
     json_data = json.dumps(data).encode("utf-8")
     headers = {"Content-Type": "application/json"}
     send_request(uri, method="POST", headers=headers, data=json_data)
 
 
+def _get_normalized_email(email):
+    """validate and get normalized email."""
+    try:
+        email_info = validate_email(email)
+        return email_info.normalized
+    except EmailNotValidError:
+        return ""
+
+
 def update_user(
     user_id: str,
     username: str,
     first_name: str,
     last_name: str,
     email: str,
     email_verified: Optional[bool] = None,
```

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/linking/linkingtask.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/linking/linkingtask.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/plugins/marshalling.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/plugins/marshalling.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/queries/__init__.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/transform/rules/__init__.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/transform/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/transform/rules/transformationrule.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/transform/rules/transformationrule.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/transform/transformationtask.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/transform/transformationtask.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/vocabularies/__init__.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/workflow/workflow.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/workflow/workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """API methods for working with a single workflow."""
+from requests_toolbelt.multipart import encoder
 from cmem.cmempy import config
-
 from cmem.cmempy.api import get_json, request, send_request
+from cmem.cmempy.workspace.tasks import post_task
 
 
 def get_workflow_uri():
     """Get endpoint URI pattern for a workflow."""
     return config.get_di_api_endpoint() + "/workflow/workflows/{}/{}"
 
 
@@ -35,23 +36,23 @@
 def get_workflow(project_name, task_name):
     """GET retrieve single workflow."""
     return send_request(
         get_workflow_uri().format(project_name, task_name), method="GET"
     ).decode("utf-8")
 
 
-def make_new_workflow(project_name, task_name, data=None):
+def make_new_workflow(project_name, task_name, data=None, metadata=None):
     """PUT create workflow."""
-    headers = {"Content-Type": "application/xml"}
-    return send_request(
-        get_workflow_uri().format(project_name, task_name),
-        method="PUT",
+    return post_task(
+        project=project_name,
+        task=task_name,
         data=data,
-        headers=headers,
-    ).decode("utf-8")
+        metadata=metadata,
+        task_type="Workflow",
+    )
 
 
 def execute_on_payload(project_name, task_name, data=None, headers=None):
     """POST execute on payload."""
     if not headers:
         headers = {"Content-Type": "application/xml"}
 
@@ -136,19 +137,27 @@
     Returns:
         Response object from requests API
     """
     endpoint = (
         f"{config.get_di_api_endpoint()}/api/workflow/"
         f"result/{project_name}/{task_name}"
     )
+
     if auto_config:
         endpoint = f"{endpoint}?config-general-autoConfig=true"
     headers = {"Accept": output_mime_type}
-    if input_file:
-        # in case an input is given do a streaming upload
+    if input_file and input_mime_type:
+        # in case an input is given, do a streaming upload
         headers["Content-Type"] = input_mime_type
         with open(input_file, "rb") as data:
+            files = [("file", (input_file, data, input_mime_type))]
+            multipart_encoder = encoder.MultipartEncoder(fields=files)
+            headers["Content-Type"] = multipart_encoder.content_type
             return request(
-                endpoint, method="POST", headers=headers, data=data, stream=True
+                endpoint,
+                method="POST",
+                headers=headers,
+                data=multipart_encoder,
+                stream=True,
             )
-    # without an input, just a post without a body
+    # without an input, just a post without a body - needed for only output requests
     return request(endpoint, method="POST", headers=headers, stream=True)
```

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/workspace/__init__.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/projectactivities.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/activities/projectactivities.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/projectactivity.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/activities/projectactivity.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/taskactivities.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/activities/taskactivities.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/taskactivity.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/activities/taskactivity.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/workspace/export_/__init__.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/export_/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/workspace/import_/__init__.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/import_/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/datasets/dataset.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/tasks/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,72 @@
-"""API methods for working with single datasets."""
+"""API for getting tasks in the data integration workspace."""
+
 import json
 
 from cmem.cmempy import config
 
 from cmem.cmempy.api import send_request
 
 
-def get_dataset_uri():
-    """Get endpoint URI pattern for a dataset."""
-    path = "/workspace/projects/{}/datasets/{}"
-    return config.get_di_api_endpoint() + path
+def get_task_uri(project_id=None, task_id=None):
+    """Get endpoint URL for the tasks API."""
+    base_path = "/workspace/projects/{}/tasks"
+
+    if project_id and task_id:
+        path = base_path + "/{}"
+        return config.get_di_api_endpoint() + path.format(project_id, task_id)
+    return config.get_di_api_endpoint() + base_path.format(project_id)
 
 
-def get_dataset(project_name, dataset_name):
-    """GET retrieve single dataset."""
-    headers = {"Accept": "application/json"}
+def get_task(project=None, task=None, with_labels=True):
+    """GET a task description."""
     response = send_request(
-        get_dataset_uri().format(project_name, dataset_name),
+        get_task_uri(project, task) + "?withLabels=" + str(with_labels).lower(),
         method="GET",
-        headers=headers,
+        headers={"Accept": "application/json"},
     )
     return json.loads(response.decode("utf-8"))
 
 
-def make_new_dataset(
-    project_name, dataset_name, dataset_type, parameters, autoconfigure
-):
-    """PUT create new dataset (deprecated)."""
-    data = {
-        "id": f"{dataset_name}",
-        "type": f"{dataset_type}",
-        "parameters": parameters,
-    }
-    data = json.dumps(data).encode("utf-8")
-    headers = {"Content-Type": "application/json"}
-    params = None
-    if autoconfigure:
-        params = {"autoConfigure": "true"}
-    send_request(
-        get_dataset_uri().format(project_name, dataset_name),
-        method="PUT",
-        data=data,
+def post_task(project=None, task=None, data=None, metadata=None, task_type=None):
+    """POST a task"""
+    if project is None:
+        raise ValueError("Project name cannot be None.")
+    if task is None:
+        raise ValueError("Task id cannot be None.")
+    if task_type is None:
+        raise ValueError("Task type cannot be None.")
+
+    url = get_task_uri(project)
+    headers = {"Content-Type": "application/json", "Accept": "application/json"}
+
+    task_data = {"id": task, "data": data or {}}
+
+    if metadata is not None:
+        task_data["metadata"] = metadata
+
+    task_data["data"]["taskType"] = task_type
+
+    encoded_data = json.dumps(task_data).encode("utf-8")
+
+    response = send_request(
+        url,
+        method="POST",
+        data=encoded_data,
         headers=headers,
-        params=params,
     )
 
+    return json.loads(response.decode("utf-8"))
 
-def delete_dataset(project_name, dataset_name):
-    """DELETE remove existing dataset."""
-    send_request(get_dataset_uri().format(project_name, dataset_name), method="DELETE")
-
-
-def create_dataset(
-    project_id, dataset_type, dataset_id=None, parameter=None, metadata=None
-):
-    """Create a dataset.
-
-    In difference to make_new_dataset, this uses the task API and does
-    not enforce an ID in advance. Also it allows for metadata parameters.
-    """
-    if parameter is None:
-        parameter = {}
-    if metadata is None:
-        metadata = {}
-    # add needed base task data
-    data = {
-        "taskType": "Dataset",
-        "type": dataset_type,
-        "parameters": parameter,
-        "metadata": metadata,
-    }
-    # add the optional task / dataset ID
-    if dataset_id:
-        data["id"] = dataset_id
-    params = None
-    path = f"/workspace/projects/{project_id}/tasks"
-    return send_request(
-        config.get_di_api_endpoint() + path,
-        method="POST",
-        data=json.dumps(data).encode("utf-8"),
-        headers={"Content-Type": "application/json"},
-        params=params,
+
+def delete_task(project=None, task=None):
+    """DELETE a task."""
+    send_request(get_task_uri(project, task), method="DELETE")
+
+
+def patch_parameter(project=None, task=None, data=None):
+    """PATCH a task."""
+    headers = {"Content-Type": "application/json"}
+    data = json.dumps(data)
+    send_request(
+        get_task_uri(project, task), data=data, headers=headers, method="PATCH"
     )
```

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/export_.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/projects/export_.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/import_.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/projects/import_.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/project.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/projects/project.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/resources/__init__.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/projects/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/resources/resource.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/projects/resources/resource.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/workspace/python.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/python.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/cmem/cmempy/workspace/search/__init__.py` & `cmem_cmempy-23.1.2rc1/cmem/cmempy/workspace/search/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.1/pyproject.toml` & `cmem_cmempy-23.1.2rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-cmempy"
-version = "23.1.1"
+version = "23.1.2rc1"
 license = "Apache-2.0"
 description = "API for eccenca Corporate Memory"
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 maintainers = ["Sebastian Tramp <sebastian.tramp@eccenca.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -28,14 +28,15 @@
 certifi = ">=2023.5.7"
 pyparsing = "^3.0.9"
 pysocks = "^1.7.1"
 rdflib = "^6.3.2"
 requests = "^2.31.0"
 requests-toolbelt = "^0.10.1"
 six = "^1.16.0"
+email-validator = "^2.0.0.post2"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.2"
 black = "^22.1.0"
 coverage = "^6.3.2"
 coverage-badge = "^1.1.0"
 defusedxml = "^0.7.1"
@@ -46,14 +47,15 @@
 pylint-junit = "^0.3.2"
 pytest = "^7.0"
 pytest-cov = "^4.0.0"
 pytest-memray = "^1.3.0"
 safety = "^1.10.3"
 types-requests = "^2.28.11.5"
 wheel = "^0.38.4"
+urllib3 = "^1.26.15"
 
 [build-system]
 requires = ["poetry-core>=1.2.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `cmem_cmempy-23.1.1/PKG-INFO` & `cmem_cmempy-23.1.2rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-cmempy
-Version: 23.1.1
+Version: 23.1.2rc1
 Summary: API for eccenca Corporate Memory
 Home-page: https://eccenca.com/go/cmempy
 License: Apache-2.0
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Maintainer: Sebastian Tramp
 Maintainer-email: sebastian.tramp@eccenca.com
@@ -15,18 +15,20 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Dist: certifi (>=2023.5.7)
+Requires-Dist: email-validator (>=2.0.0.post2,<3.0.0)
 Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
 Requires-Dist: pysocks (>=1.7.1,<2.0.0)
 Requires-Dist: rdflib (>=6.3.2,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: requests-toolbelt (>=0.10.1,<0.11.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Description-Content-Type: text/markdown
```

