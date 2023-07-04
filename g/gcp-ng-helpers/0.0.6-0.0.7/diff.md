# Comparing `tmp/gcp_ng_helpers-0.0.6.tar.gz` & `tmp/gcp_ng_helpers-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp_ng_helpers-0.0.6.tar", last modified: Fri May  5 09:13:20 2023, max compression
+gzip compressed data, was "gcp_ng_helpers-0.0.7.tar", last modified: Tue Jul  4 10:56:27 2023, max compression
```

## Comparing `gcp_ng_helpers-0.0.6.tar` & `gcp_ng_helpers-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:13:20.662565 gcp_ng_helpers-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-05 09:13:20.662565 gcp_ng_helpers-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:13:20.658565 gcp_ng_helpers-0.0.6/gcp_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/gcp_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:13:20.658565 gcp_ng_helpers-0.0.6/gcp_helpers/cloud_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/gcp_helpers/cloud_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/gcp_helpers/cloud_tasks/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:13:20.662565 gcp_ng_helpers-0.0.6/gcp_helpers/functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/gcp_helpers/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/gcp_helpers/functions/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/gcp_helpers/functions/routers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:13:20.662565 gcp_ng_helpers-0.0.6/gcp_ng_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-05 09:13:20.000000 gcp_ng_helpers-0.0.6/gcp_ng_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-05 09:13:20.000000 gcp_ng_helpers-0.0.6/gcp_ng_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:13:20.000000 gcp_ng_helpers-0.0.6/gcp_ng_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 09:13:20.000000 gcp_ng_helpers-0.0.6/gcp_ng_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 09:13:20.000000 gcp_ng_helpers-0.0.6/gcp_ng_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-05 09:13:20.662565 gcp_ng_helpers-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:56:27.393393 gcp_ng_helpers-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-04 10:56:27.393393 gcp_ng_helpers-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:56:27.393393 gcp_ng_helpers-0.0.7/gcp_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/gcp_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:56:27.393393 gcp_ng_helpers-0.0.7/gcp_helpers/cloud_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/gcp_helpers/cloud_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/gcp_helpers/cloud_tasks/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:56:27.393393 gcp_ng_helpers-0.0.7/gcp_helpers/firestore/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/gcp_helpers/firestore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/gcp_helpers/firestore/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:56:27.393393 gcp_ng_helpers-0.0.7/gcp_helpers/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/gcp_helpers/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/gcp_helpers/functions/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/gcp_helpers/functions/routers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:56:27.393393 gcp_ng_helpers-0.0.7/gcp_ng_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-04 10:56:27.000000 gcp_ng_helpers-0.0.7/gcp_ng_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-04 10:56:27.000000 gcp_ng_helpers-0.0.7/gcp_ng_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:56:27.000000 gcp_ng_helpers-0.0.7/gcp_ng_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 10:56:27.000000 gcp_ng_helpers-0.0.7/gcp_ng_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 10:56:27.000000 gcp_ng_helpers-0.0.7/gcp_ng_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-04 10:56:27.393393 gcp_ng_helpers-0.0.7/setup.cfg
```

### Comparing `gcp_ng_helpers-0.0.6/LICENSE` & `gcp_ng_helpers-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.6/PKG-INFO` & `gcp_ng_helpers-0.0.7/gcp_ng_helpers.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gcp_ng_helpers
-Version: 0.0.6
+Name: gcp-ng-helpers
+Version: 0.0.7
 Summary: Various helper functions for Google Cloud services
 Home-page: https://github.com/NGhostClub/gcp-helpers
 Author: Dmitriy Tischenko aka NGhost
 Author-email: nghostik@gmail.com
 Project-URL: Source, https://github.com/NGhostClub/gcp-helpers
 Project-URL: Bug Tracker, https://github.com/NGhostClub/gcp-helpers/issues
 Classifier: Intended Audience :: Developers
@@ -26,15 +26,15 @@
 ```commandline
 pip install gcp-ng-helpers
 ```
 
 # Functions submodule
 ## Http Router
 Cloud function by default only serves single '/' (root) http endpoint.
-With this Http Router you can easy serve much more, without need to parse 
+With this Http Router you can easily serve much more, without need to parse 
 Request object for method and path
 ### Usage
 Define a function with flask.Request argument
 returning the flaks.Response object
 Import HttpRouter from functions submodule and register defined function
 as route with path and method
 Then inside cloud function entry point function return router.response
@@ -50,7 +50,16 @@
 
 router = HttpRouter()
 router.register(hello_route, '/hello', 'GET')
 
 def main(request):
     return router.response(request)
 ```
+# Tasks submodule
+## Manager
+CloudTasksManager class is wrapper for cloud task api. Allows to shorten task creation.
+Currently, supports only http task creation
+
+# Firestore
+## Collection
+FirestoreCollection and FirestoreCollectionGroup are wrappers for firestore read/write operations
+bounded to the defined collection or collection group.
```

### Comparing `gcp_ng_helpers-0.0.6/gcp_helpers/cloud_tasks/manager.py` & `gcp_ng_helpers-0.0.7/gcp_helpers/cloud_tasks/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 
 class CloudTasksManager:
     def __init__(self, project, location, queue_name, key_path=None):
         self._project = project
         self._location = location
         self._queue_name = queue_name
         self._key_path = key_path
-        self._cli = self._new_client()
+        self.cli = self._new_client()
         self._queue_path = self._new_queue()
-        self.http = HttpCloudTasks(self._cli, self._queue_path)
+        self.http = HttpCloudTasks(self.cli, self._queue_path)
 
     def _new_client(self):
         if not self._key_path:
             return tasks_v2.CloudTasksClient()
         else:
             return tasks_v2.CloudTasksClient(
                 credentials=service_account.Credentials.from_service_account_file(self._key_path)
             )
 
     def _new_queue(self):
-        return self._cli.queue_path(self._project, self._location, self._queue_name)
+        return self.cli.queue_path(self._project, self._location, self._queue_name)
 
 
 class HttpCloudTasks:
     METHODS = {
         "POST": tasks_v2.HttpMethod.POST,
         "GET": tasks_v2.HttpMethod.GET,
         "PUT": tasks_v2.HttpMethod.PUT,
```

### Comparing `gcp_ng_helpers-0.0.6/gcp_helpers/functions/decorators.py` & `gcp_ng_helpers-0.0.7/gcp_helpers/functions/decorators.py`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.6/gcp_helpers/functions/routers.py` & `gcp_ng_helpers-0.0.7/gcp_helpers/functions/routers.py`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.6/gcp_ng_helpers.egg-info/PKG-INFO` & `gcp_ng_helpers-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gcp-ng-helpers
-Version: 0.0.6
+Name: gcp_ng_helpers
+Version: 0.0.7
 Summary: Various helper functions for Google Cloud services
 Home-page: https://github.com/NGhostClub/gcp-helpers
 Author: Dmitriy Tischenko aka NGhost
 Author-email: nghostik@gmail.com
 Project-URL: Source, https://github.com/NGhostClub/gcp-helpers
 Project-URL: Bug Tracker, https://github.com/NGhostClub/gcp-helpers/issues
 Classifier: Intended Audience :: Developers
@@ -26,15 +26,15 @@
 ```commandline
 pip install gcp-ng-helpers
 ```
 
 # Functions submodule
 ## Http Router
 Cloud function by default only serves single '/' (root) http endpoint.
-With this Http Router you can easy serve much more, without need to parse 
+With this Http Router you can easily serve much more, without need to parse 
 Request object for method and path
 ### Usage
 Define a function with flask.Request argument
 returning the flaks.Response object
 Import HttpRouter from functions submodule and register defined function
 as route with path and method
 Then inside cloud function entry point function return router.response
@@ -50,7 +50,16 @@
 
 router = HttpRouter()
 router.register(hello_route, '/hello', 'GET')
 
 def main(request):
     return router.response(request)
 ```
+# Tasks submodule
+## Manager
+CloudTasksManager class is wrapper for cloud task api. Allows to shorten task creation.
+Currently, supports only http task creation
+
+# Firestore
+## Collection
+FirestoreCollection and FirestoreCollectionGroup are wrappers for firestore read/write operations
+bounded to the defined collection or collection group.
```

### Comparing `gcp_ng_helpers-0.0.6/setup.cfg` & `gcp_ng_helpers-0.0.7/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 license_file = LICENSE
 name = gcp_ng_helpers
-version = 0.0.6
+version = 0.0.7
 author = Dmitriy Tischenko aka NGhost
 author_email = nghostik@gmail.com
 description = Various helper functions for Google Cloud services
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/NGhostClub/gcp-helpers
 project_urls = 
@@ -18,18 +18,20 @@
 	Operating System :: OS Independent
 
 [options]
 packages = 
 	gcp_helpers
 	gcp_helpers.functions
 	gcp_helpers.cloud_tasks
+	gcp_helpers.firestore
 python_requires = >=3.10
 install_requires = 
 	flask
 	google-cloud-tasks
+	google-cloud-firestore
 
 [options.packages.find]
 where = gcp_helpers
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

