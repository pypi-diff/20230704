# Comparing `tmp/aistudio-scheduler-lock-1.0.6a1.tar.gz` & `tmp/aistudio-scheduler-lock-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aistudio-scheduler-lock-1.0.6a1.tar", max compression
+gzip compressed data, was "aistudio-scheduler-lock-1.0.7.tar", max compression
```

## Comparing `aistudio-scheduler-lock-1.0.6a1.tar` & `aistudio-scheduler-lock-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0        0 2022-09-02 06:46:57.612688 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/__init__.py
--rwxr-xr-x   0        0        0       63 2022-09-02 06:46:57.614636 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/admin.py
--rwxr-xr-x   0        0        0     2020 2023-04-10 05:49:04.342584 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/apps.py
--rwxr-xr-x   0        0        0      645 2023-04-10 05:49:04.342910 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/base_lock.py
--rwxr-xr-x   0        0        0     1078 2022-09-05 07:32:43.545338 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/database_advisory_lock.py
--rwxr-xr-x   0        0        0     4853 2023-04-10 05:49:04.343353 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/database_lock.py
--rwxr-xr-x   0        0        0     5732 2023-04-10 05:49:04.345163 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/file_lock.py
--rwxr-xr-x   0        0        0     1104 2023-04-10 05:49:04.345653 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/utils.py
--rwxr-xr-x   0        0        0      773 2022-09-02 06:46:57.623569 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2022-09-02 06:46:57.623676 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/migrations/__init__.py
--rwxr-xr-x   0        0        0     6015 2022-09-05 08:49:04.799827 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/models.py
--rwxr-xr-x   0        0        0       92 2023-04-10 05:49:04.345892 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/schedules/enums.py
--rwxr-xr-x   0        0        0     8932 2023-04-10 05:50:54.414395 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/schedules/scheduler_lock_job.py
--rwxr-xr-x   0        0        0     1658 2023-04-10 05:49:04.346624 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/schedules/schedules_master_base.py
--rwxr-xr-x   0        0        0       60 2022-09-02 06:46:57.624105 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/tests.py
--rwxr-xr-x   0        0        0      457 2023-05-30 11:07:21.899173 aistudio-scheduler-lock-1.0.6a1/pyproject.toml
--rw-r--r--   0        0        0      869 1970-01-01 00:00:00.000000 aistudio-scheduler-lock-1.0.6a1/setup.py
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 aistudio-scheduler-lock-1.0.6a1/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2022-09-02 06:46:57.612688 aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/__init__.py
+-rwxr-xr-x   0        0        0       63 2022-09-02 06:46:57.614636 aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/admin.py
+-rwxr-xr-x   0        0        0     2020 2023-04-10 05:49:04.342584 aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/apps.py
+-rwxr-xr-x   0        0        0      645 2023-04-10 05:49:04.342910 aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/locks/base_lock.py
+-rwxr-xr-x   0        0        0     1078 2022-09-05 07:32:43.545338 aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/locks/database_advisory_lock.py
+-rwxr-xr-x   0        0        0     4853 2023-04-10 05:49:04.343353 aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/locks/database_lock.py
+-rwxr-xr-x   0        0        0     5732 2023-04-10 05:49:04.345163 aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/locks/file_lock.py
+-rwxr-xr-x   0        0        0     1104 2023-04-10 05:49:04.345653 aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/locks/utils.py
+-rwxr-xr-x   0        0        0      773 2022-09-02 06:46:57.623569 aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2022-09-02 06:46:57.623676 aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/migrations/__init__.py
+-rwxr-xr-x   0        0        0     6015 2022-09-05 08:49:04.799827 aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/models.py
+-rwxr-xr-x   0        0        0       92 2023-04-10 05:49:04.345892 aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/schedules/enums.py
+-rwxr-xr-x   0        0        0     8932 2023-04-10 05:50:54.414395 aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/schedules/scheduler_lock_job.py
+-rwxr-xr-x   0        0        0     1658 2023-04-10 05:49:04.346624 aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/schedules/schedules_master_base.py
+-rwxr-xr-x   0        0        0       60 2022-09-02 06:46:57.624105 aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/tests.py
+-rwxr-xr-x   0        0        0      456 2023-07-04 10:53:10.635577 aistudio-scheduler-lock-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 aistudio-scheduler-lock-1.0.7/setup.py
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 aistudio-scheduler-lock-1.0.7/PKG-INFO
```

### Comparing `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/apps.py` & `aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/apps.py`

 * *Files identical despite different names*

### Comparing `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/base_lock.py` & `aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/locks/base_lock.py`

 * *Files identical despite different names*

### Comparing `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/database_advisory_lock.py` & `aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/locks/database_advisory_lock.py`

 * *Files identical despite different names*

### Comparing `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/database_lock.py` & `aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/locks/database_lock.py`

 * *Files identical despite different names*

### Comparing `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/file_lock.py` & `aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/locks/file_lock.py`

 * *Files identical despite different names*

### Comparing `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/utils.py` & `aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/locks/utils.py`

 * *Files identical despite different names*

### Comparing `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/migrations/0001_initial.py` & `aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/models.py` & `aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/models.py`

 * *Files identical despite different names*

### Comparing `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/schedules/scheduler_lock_job.py` & `aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/schedules/scheduler_lock_job.py`

 * *Files identical despite different names*

### Comparing `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/schedules/schedules_master_base.py` & `aistudio-scheduler-lock-1.0.7/aistudio_scheduler_lock/schedules/schedules_master_base.py`

 * *Files identical despite different names*

### Comparing `aistudio-scheduler-lock-1.0.6a1/setup.py` & `aistudio-scheduler-lock-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
  'aistudio_scheduler_lock.migrations',
  'aistudio_scheduler_lock.schedules']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Django==3.2.19', 'django-apscheduler==0.6.2', 'setuptools==65.5.1']
+['Django>=3.2.20,<4.0.0', 'django-apscheduler==0.6.2', 'setuptools==65.5.1']
 
 setup_kwargs = {
     'name': 'aistudio-scheduler-lock',
-    'version': '1.0.6a1',
+    'version': '1.0.7',
     'description': 'Implements a distributed locking scheme for schedulers running on HA mode.',
     'long_description': 'None',
     'author': 'Yogesh Ketkar',
     'author_email': 'yogesh.ketkar@automationedge.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `aistudio-scheduler-lock-1.0.6a1/PKG-INFO` & `aistudio-scheduler-lock-1.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aistudio-scheduler-lock
-Version: 1.0.6a1
+Version: 1.0.7
 Summary: Implements a distributed locking scheme for schedulers running on HA mode.
 Author: Yogesh Ketkar
 Author-email: yogesh.ketkar@automationedge.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: Django (==3.2.19)
+Requires-Dist: Django (>=3.2.20,<4.0.0)
 Requires-Dist: django-apscheduler (==0.6.2)
 Requires-Dist: setuptools (==65.5.1)
```

