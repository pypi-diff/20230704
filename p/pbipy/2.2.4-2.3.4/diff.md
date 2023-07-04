# Comparing `tmp/pbipy-2.2.4.tar.gz` & `tmp/pbipy-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbipy-2.2.4.tar", last modified: Fri Jun 30 01:52:58 2023, max compression
+gzip compressed data, was "pbipy-2.3.4.tar", last modified: Tue Jul  4 08:10:01 2023, max compression
```

## Comparing `pbipy-2.2.4.tar` & `pbipy-2.3.4.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 01:52:58.020313 pbipy-2.2.4/
--rw-rw-rw-   0        0        0    11523 2022-10-28 08:16:15.000000 pbipy-2.2.4/LICENSE
--rw-rw-rw-   0        0        0    10239 2023-06-30 01:52:58.019312 pbipy-2.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     9455 2023-06-30 01:32:50.000000 pbipy-2.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 01:52:58.006313 pbipy-2.2.4/pbipy/
--rw-rw-rw-   0        0        0       29 2022-10-28 07:52:32.000000 pbipy-2.2.4/pbipy/__init__.py
--rw-rw-rw-   0        0        0      335 2023-06-30 01:51:21.000000 pbipy-2.2.4/pbipy/__version__.py
--rw-rw-rw-   0        0        0    19984 2023-06-20 20:08:48.000000 pbipy-2.2.4/pbipy/datasets.py
--rw-rw-rw-   0        0        0     5861 2023-06-20 20:12:45.000000 pbipy-2.2.4/pbipy/groups.py
--rw-rw-rw-   0        0        0    11659 2023-06-25 19:35:31.000000 pbipy-2.2.4/pbipy/powerbi.py
--rw-rw-rw-   0        0        0    12848 2023-06-30 01:50:56.000000 pbipy-2.2.4/pbipy/reports.py
--rw-rw-rw-   0        0        0     1312 2023-06-19 20:24:41.000000 pbipy-2.2.4/pbipy/resources.py
--rw-rw-rw-   0        0        0      110 2023-06-18 05:21:13.000000 pbipy-2.2.4/pbipy/settings.py
--rw-rw-rw-   0        0        0    11125 2023-06-29 21:51:58.000000 pbipy-2.2.4/pbipy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:52:58.017311 pbipy-2.2.4/pbipy.egg-info/
--rw-rw-rw-   0        0        0    10239 2023-06-30 01:52:57.000000 pbipy-2.2.4/pbipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-06-30 01:52:57.000000 pbipy-2.2.4/pbipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 01:52:57.000000 pbipy-2.2.4/pbipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-30 01:52:57.000000 pbipy-2.2.4/pbipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-30 01:52:57.000000 pbipy-2.2.4/pbipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 01:52:58.021316 pbipy-2.2.4/setup.cfg
--rw-rw-rw-   0        0        0     3594 2022-12-05 03:27:44.000000 pbipy-2.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:10:01.427516 pbipy-2.3.4/
+-rw-rw-rw-   0        0        0    11523 2022-10-28 08:16:15.000000 pbipy-2.3.4/LICENSE
+-rw-rw-rw-   0        0        0    11017 2023-07-04 08:10:01.426513 pbipy-2.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    10233 2023-07-04 08:02:15.000000 pbipy-2.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 08:10:01.412516 pbipy-2.3.4/pbipy/
+-rw-rw-rw-   0        0        0       29 2022-10-28 07:52:32.000000 pbipy-2.3.4/pbipy/__init__.py
+-rw-rw-rw-   0        0        0      335 2023-07-04 08:07:00.000000 pbipy-2.3.4/pbipy/__version__.py
+-rw-rw-rw-   0        0        0     4932 2023-07-03 17:56:42.000000 pbipy-2.3.4/pbipy/apps.py
+-rw-rw-rw-   0        0        0     1630 2023-07-03 09:18:23.000000 pbipy-2.3.4/pbipy/dashboards.py
+-rw-rw-rw-   0        0        0    19984 2023-06-20 20:08:48.000000 pbipy-2.3.4/pbipy/datasets.py
+-rw-rw-rw-   0        0        0     5861 2023-06-20 20:12:45.000000 pbipy-2.3.4/pbipy/groups.py
+-rw-rw-rw-   0        0        0    12471 2023-07-02 19:39:59.000000 pbipy-2.3.4/pbipy/powerbi.py
+-rw-rw-rw-   0        0        0    12848 2023-06-30 01:50:56.000000 pbipy-2.3.4/pbipy/reports.py
+-rw-rw-rw-   0        0        0     1312 2023-06-19 20:24:41.000000 pbipy-2.3.4/pbipy/resources.py
+-rw-rw-rw-   0        0        0      110 2023-06-18 05:21:13.000000 pbipy-2.3.4/pbipy/settings.py
+-rw-rw-rw-   0        0        0    11125 2023-06-29 21:51:58.000000 pbipy-2.3.4/pbipy/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:10:01.423517 pbipy-2.3.4/pbipy.egg-info/
+-rw-rw-rw-   0        0        0    11017 2023-07-04 08:10:01.000000 pbipy-2.3.4/pbipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2023-07-04 08:10:01.000000 pbipy-2.3.4/pbipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 08:10:01.000000 pbipy-2.3.4/pbipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-04 08:10:01.000000 pbipy-2.3.4/pbipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-04 08:10:01.000000 pbipy-2.3.4/pbipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 08:10:01.427516 pbipy-2.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     3594 2022-12-05 03:27:44.000000 pbipy-2.3.4/setup.py
```

### Comparing `pbipy-2.2.4/LICENSE` & `pbipy-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pbipy-2.2.4/PKG-INFO` & `pbipy-2.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbipy
-Version: 2.2.4
+Version: 2.3.4
 Summary: A Python Library for interacting with the Power BI Rest API.
 Home-page: https://github.com/andrewvillazon/pbipy
 Author: Andrew Villazon
 Author-email: andrew.villazon@gmail.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -21,15 +21,15 @@
 # pbipy
 
 ![PyPI](https://img.shields.io/pypi/v/pbipy) ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/andrewvillazon/pbipy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pbipy) ![GitHub](https://img.shields.io/github/license/andrewvillazon/pbipy) ![Static Badge](https://img.shields.io/badge/Python-blue?logo=python&logoColor=yellow) ![Static Badge](https://img.shields.io/badge/power-bi-yellow?logoColor=yellow&labelColor=yellow&color=black)
 
 
 `pbipy` is a Python Library for interacting with the Power BI Rest API. It aims to simplyify working with the Power BI Rest API and support programatic administration of Power BI in Python.
 
-`pbipy` supports operations for Reports, Datasets, and Groups (Workspaces), allowing users to perform actions on their PowerBI instance using Python.
+`pbipy` supports operations for Apps, Datasets, Groups (Workspaces) and Reports, allowing users to perform actions on their PowerBI instance using Python.
 
 See [development progress](#development-progress) below for what's been implemented and what's coming.
 
 ## Installation
 
 ```console
 pip install pbipy
@@ -57,15 +57,15 @@
 
 * [Power BI REST API with Python and MSAL. Part II.](https://www.datalineo.com/post/power-bi-rest-api-with-python-and-msal-part-ii)
 * [Power BI REST API with Python Part III, azure-identity](https://www.datalineo.com/post/power-bi-rest-api-with-python-part-iii-azure-identity)
 * [Monitoring Power BI using REST APIs from Python](https://data-goblins.com/power-bi/power-bi-api-python)
 
 The example below uses the `msal` library to to get a `bearer_token`.
 
-## Quickstart
+## Useage
 
 Start by creating the `PowerBI()` client. All interactions with the Power BI Rest API go through this object. 
 
 ```python
 import msal
 
 from pbipy import PowerBI
@@ -86,16 +86,14 @@
     scopes=["https://analysis.windows.net/powerbi/api/.default"],
 )
 
 # Create Client
 pbi = PowerBI(bearer_token)
 ```
 
-### Functionality
-
 To interact with the API, simply call the relevant method from the client.
 
 ```python
 # Grab the datasets from a workspace
 
 pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
 ```
@@ -138,40 +136,39 @@
 #   "name": "SalesMarketing",
 #   "addRowsAPIEnabled": False,
 #   "configuredBy": "john@contoso.com",
 #   ...
 # }
 ```
 
-## Examples
+## Example: Working with Datasets
+
+Let's see how `pbipy` works by performing some operations on a Dataset.
 
-### Datasets
+First, we need to load the Dataset from the API. To do this, we call the `dataset()` method from the `pbi` client we created above. 
 
-#### Get a dataset
+The Power BI Rest API will look for the Dataset in the current user's workspace if we don't provide a group argument.
 
 ```python
 sales = pbi.dataset(id="cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 print(sales)
 
 # <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
 ```
 
-#### Get a list of Datasets in a Workspace (Group)
+But we likely want to target a Dataset in a *Workspace*. To do this, we provide the `group_id` when we call the `dataset()` method.
 
 ```python
-datasets = pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
-
-for dataset in datasets:
-    print(dataset)
-
-# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', ...>
-# <Dataset id='f7fc6510-e151-42a3-850b-d0805a391db0', ...>
+sales = pbi.dataset(
+    "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
+    group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
+)
 ```
 
-#### Refresh History of a Dataset
+Now that we've got our target Dataset let's look at its Refresh History. We call the `refresh_history()` method on our Dataset. Easy.
 
 ```python
 dataset = pbi.dataset(
     "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
     group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
 )
 
@@ -179,24 +176,24 @@
 
 for entry in refresh_history:
     print(entry)
 
 # {"refreshType":"ViaApi", "startTime":"2017-06-13T09:25:43.153Z", "status": "Completed" ...}
 ```
 
-#### Add user permissions to a Dataset
+How about adding some user permissions to our Dataset? That's easy too. Just call the `add_user()` method with the User's details and permissions.
 
 ```python
 sales_ds = pbi.dataset( "cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 
 # Give John 'Read' access on the dataset
 sales_ds.add_user("john@contoso.com", "User", "Read")
 ```
 
-### Execute a DAX Query
+Lastly, if we're feeling adventurous, we can execute DAX against a Dataset and use the results in Python.
 
 ```python
 dataset = pbi.dataset( "cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 
 dxq_result = dataset.execute_queries("EVALUATE VALUES(MyTable)")
 print(dxq_result)
 
@@ -210,40 +207,50 @@
 #               "MyTable[Year]": 2010,
 #               "MyTable[Quarter]": "Q1"
 #             },
 # ...
 # }
 ```
 
-### Workspaces (Groups) *
+## More examples
+
+### Datasets in a Workspace
+
+```python
+datasets = pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
 
-*\* In the Power BI Rest API, workspaces are referred to as "groups".*
+for dataset in datasets:
+    print(dataset)
+
+# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', ...>
+# <Dataset id='f7fc6510-e151-42a3-850b-d0805a391db0', ...>
+```
 
-#### List Workspaces
+### List Workspaces
 
 ```python
 groups = pbi.groups()
 
 for group in groups:
     print(group)
 
 # <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
 # <Group id='3d9b93c6-7b6d-4801-a491-1738910904fd', name='marketing'>
 ```
 
-#### Create a Workspace
+### Create a Workspace
 
 ```python
 group = pbi.create_group("contoso")
 print(group)
 
 # <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
 ```
 
-#### Users and their access
+### Users and their access
 
 ```python
 group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
 users = group.users()
 
 for user in users:
     print(user)
@@ -257,23 +264,24 @@
 `pbipy` methods wrap around the Operations described in the Power BI Rest API Reference:
 
 [Power BI REST APIs for embedded analytics and automation - Power BI REST API](https://learn.microsoft.com/en-us/rest/api/power-bi/)
 
 
 ## Development Progress
 
-`pbipy` is in the early stages of development so expect a few features to be missing. The aim is to cover off most of the core stuff like Datasets, Workspaces (Groups), Reports, Apps, etc., and the rest later on. Check back regularly to see what's been added or still in the pipeline.
+`pbipy` is in development so expect a few features to be missing. The aim is to cover off most of the core stuff like Datasets, Workspaces (Groups), Reports, Apps, etc., and the rest later on. Check back regularly to see what's been added or still in the pipeline.
 
 | PowerBI Component   	| Progress 	| Notes 	|
 |---------------------	|----------	|-------	|
 | Datasets            	| Done     	|       	|
 | Groups (Workspaces) 	| Done    	|       	|
 | Reports             	| Done      |       	|
-| Apps                	| Doing   	|       	|
-| Dataflows           	| Todo     	|       	|
+| Apps                	| Done   	|       	|
+| Dataflows           	| Doing    	|       	|
+| Admin Operations     	| Todo     	|       	|
 | Dashboards          	| Todo     	|       	|
 | Everything else     	| Backlog  	|       	|
 
 ## Contributing
 
 Contributions such as bug reports, fixes, documentation or docstrings, enhancements, and ideas are welcome. `pbipy` uses github to host code, track issues, record feature requests, and accept pull requests.
```

### Comparing `pbipy-2.2.4/README.md` & `pbipy-2.3.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pbipy
 
 ![PyPI](https://img.shields.io/pypi/v/pbipy) ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/andrewvillazon/pbipy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pbipy) ![GitHub](https://img.shields.io/github/license/andrewvillazon/pbipy) ![Static Badge](https://img.shields.io/badge/Python-blue?logo=python&logoColor=yellow) ![Static Badge](https://img.shields.io/badge/power-bi-yellow?logoColor=yellow&labelColor=yellow&color=black)
 
 
 `pbipy` is a Python Library for interacting with the Power BI Rest API. It aims to simplyify working with the Power BI Rest API and support programatic administration of Power BI in Python.
 
-`pbipy` supports operations for Reports, Datasets, and Groups (Workspaces), allowing users to perform actions on their PowerBI instance using Python.
+`pbipy` supports operations for Apps, Datasets, Groups (Workspaces) and Reports, allowing users to perform actions on their PowerBI instance using Python.
 
 See [development progress](#development-progress) below for what's been implemented and what's coming.
 
 ## Installation
 
 ```console
 pip install pbipy
@@ -37,15 +37,15 @@
 
 * [Power BI REST API with Python and MSAL. Part II.](https://www.datalineo.com/post/power-bi-rest-api-with-python-and-msal-part-ii)
 * [Power BI REST API with Python Part III, azure-identity](https://www.datalineo.com/post/power-bi-rest-api-with-python-part-iii-azure-identity)
 * [Monitoring Power BI using REST APIs from Python](https://data-goblins.com/power-bi/power-bi-api-python)
 
 The example below uses the `msal` library to to get a `bearer_token`.
 
-## Quickstart
+## Useage
 
 Start by creating the `PowerBI()` client. All interactions with the Power BI Rest API go through this object. 
 
 ```python
 import msal
 
 from pbipy import PowerBI
@@ -66,16 +66,14 @@
     scopes=["https://analysis.windows.net/powerbi/api/.default"],
 )
 
 # Create Client
 pbi = PowerBI(bearer_token)
 ```
 
-### Functionality
-
 To interact with the API, simply call the relevant method from the client.
 
 ```python
 # Grab the datasets from a workspace
 
 pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
 ```
@@ -118,40 +116,39 @@
 #   "name": "SalesMarketing",
 #   "addRowsAPIEnabled": False,
 #   "configuredBy": "john@contoso.com",
 #   ...
 # }
 ```
 
-## Examples
+## Example: Working with Datasets
+
+Let's see how `pbipy` works by performing some operations on a Dataset.
 
-### Datasets
+First, we need to load the Dataset from the API. To do this, we call the `dataset()` method from the `pbi` client we created above. 
 
-#### Get a dataset
+The Power BI Rest API will look for the Dataset in the current user's workspace if we don't provide a group argument.
 
 ```python
 sales = pbi.dataset(id="cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 print(sales)
 
 # <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
 ```
 
-#### Get a list of Datasets in a Workspace (Group)
+But we likely want to target a Dataset in a *Workspace*. To do this, we provide the `group_id` when we call the `dataset()` method.
 
 ```python
-datasets = pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
-
-for dataset in datasets:
-    print(dataset)
-
-# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', ...>
-# <Dataset id='f7fc6510-e151-42a3-850b-d0805a391db0', ...>
+sales = pbi.dataset(
+    "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
+    group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
+)
 ```
 
-#### Refresh History of a Dataset
+Now that we've got our target Dataset let's look at its Refresh History. We call the `refresh_history()` method on our Dataset. Easy.
 
 ```python
 dataset = pbi.dataset(
     "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
     group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
 )
 
@@ -159,24 +156,24 @@
 
 for entry in refresh_history:
     print(entry)
 
 # {"refreshType":"ViaApi", "startTime":"2017-06-13T09:25:43.153Z", "status": "Completed" ...}
 ```
 
-#### Add user permissions to a Dataset
+How about adding some user permissions to our Dataset? That's easy too. Just call the `add_user()` method with the User's details and permissions.
 
 ```python
 sales_ds = pbi.dataset( "cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 
 # Give John 'Read' access on the dataset
 sales_ds.add_user("john@contoso.com", "User", "Read")
 ```
 
-### Execute a DAX Query
+Lastly, if we're feeling adventurous, we can execute DAX against a Dataset and use the results in Python.
 
 ```python
 dataset = pbi.dataset( "cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 
 dxq_result = dataset.execute_queries("EVALUATE VALUES(MyTable)")
 print(dxq_result)
 
@@ -190,40 +187,50 @@
 #               "MyTable[Year]": 2010,
 #               "MyTable[Quarter]": "Q1"
 #             },
 # ...
 # }
 ```
 
-### Workspaces (Groups) *
+## More examples
+
+### Datasets in a Workspace
+
+```python
+datasets = pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
 
-*\* In the Power BI Rest API, workspaces are referred to as "groups".*
+for dataset in datasets:
+    print(dataset)
+
+# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', ...>
+# <Dataset id='f7fc6510-e151-42a3-850b-d0805a391db0', ...>
+```
 
-#### List Workspaces
+### List Workspaces
 
 ```python
 groups = pbi.groups()
 
 for group in groups:
     print(group)
 
 # <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
 # <Group id='3d9b93c6-7b6d-4801-a491-1738910904fd', name='marketing'>
 ```
 
-#### Create a Workspace
+### Create a Workspace
 
 ```python
 group = pbi.create_group("contoso")
 print(group)
 
 # <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
 ```
 
-#### Users and their access
+### Users and their access
 
 ```python
 group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
 users = group.users()
 
 for user in users:
     print(user)
@@ -237,23 +244,24 @@
 `pbipy` methods wrap around the Operations described in the Power BI Rest API Reference:
 
 [Power BI REST APIs for embedded analytics and automation - Power BI REST API](https://learn.microsoft.com/en-us/rest/api/power-bi/)
 
 
 ## Development Progress
 
-`pbipy` is in the early stages of development so expect a few features to be missing. The aim is to cover off most of the core stuff like Datasets, Workspaces (Groups), Reports, Apps, etc., and the rest later on. Check back regularly to see what's been added or still in the pipeline.
+`pbipy` is in development so expect a few features to be missing. The aim is to cover off most of the core stuff like Datasets, Workspaces (Groups), Reports, Apps, etc., and the rest later on. Check back regularly to see what's been added or still in the pipeline.
 
 | PowerBI Component   	| Progress 	| Notes 	|
 |---------------------	|----------	|-------	|
 | Datasets            	| Done     	|       	|
 | Groups (Workspaces) 	| Done    	|       	|
 | Reports             	| Done      |       	|
-| Apps                	| Doing   	|       	|
-| Dataflows           	| Todo     	|       	|
+| Apps                	| Done   	|       	|
+| Dataflows           	| Doing    	|       	|
+| Admin Operations     	| Todo     	|       	|
 | Dashboards          	| Todo     	|       	|
 | Everything else     	| Backlog  	|       	|
 
 ## Contributing
 
 Contributions such as bug reports, fixes, documentation or docstrings, enhancements, and ideas are welcome. `pbipy` uses github to host code, track issues, record feature requests, and accept pull requests.
```

### Comparing `pbipy-2.2.4/pbipy/datasets.py` & `pbipy-2.3.4/pbipy/datasets.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.2.4/pbipy/groups.py` & `pbipy-2.3.4/pbipy/groups.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.2.4/pbipy/powerbi.py` & `pbipy-2.3.4/pbipy/powerbi.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 https://learn.microsoft.com/en-us/rest/api/power-bi/
 """
 
 import requests
 from requests.exceptions import HTTPError
 
 from pbipy import settings
+from pbipy.apps import App
 from pbipy.groups import Group
 from pbipy.datasets import Dataset
 from pbipy.reports import Report
 from pbipy.utils import RequestsMixin, remove_no_values
 
 
 class PowerBI(RequestsMixin):
@@ -52,14 +53,58 @@
         self.bearer_token = bearer_token
 
         if not session:
             self.session = requests.Session()
 
         self.session.headers.update({"Authorization": f"Bearer {self.bearer_token}"})
 
+    def app(
+        self,
+        app: str,
+    ) -> App:
+        """
+        Return the specified installed app.
+
+        Parameters
+        ----------
+        `app` : `str`
+            App id of the App to retrieve.
+
+        Returns
+        -------
+        `App`
+            The specified App.
+
+        """
+
+        if isinstance(app, App):
+            return app
+
+        app = App(app, self.session)
+        app.load()
+
+        return app
+
+    def apps(
+        self,
+    ) -> list[App]:
+        resource = self.BASE_URL + "/apps"
+        raw = self.get_raw(resource, self.session)
+
+        apps = [
+            App(
+                app_js.get("id"),
+                self.session,
+                raw=app_js,
+            )
+            for app_js in raw
+        ]
+
+        return apps
+
     # TODO: Add support for passing in a group obj
     def dataset(
         self,
         dataset: str | Dataset,
         group: str = None,
     ) -> Dataset:
         """
@@ -222,15 +267,15 @@
             Returns only the first n results.
 
         Returns
         -------
         `list[Group]`
             List of `Group` objects the user has access to, and/or
             that matched the specified filters.
-        
+
         Notes
         -----
         See below for more details on filter syntax:
         https://learn.microsoft.com/en-us/power-bi/collaborate-share/service-url-filters
 
         """
 
@@ -397,46 +442,46 @@
 
     def delete_report(
         self,
         report: str | Report,
         group: str | Group = None,
     ) -> None:
         """
-        Delete the specified report. 
-        
-        If a `Report` type is provided as `report`, then it's `group_id` 
+        Delete the specified report.
+
+        If a `Report` type is provided as `report`, then it's `group_id`
         will be taken as the `group` value.
 
         Parameters
         ----------
         `report` : `str | Report`
             Report Id or `Report` object to delete.
         `group` : `str | Group`, optional
             The Group Id or `Group` object where the report resides. If
             a `Report` object is provided then the `group_id` of that report
             will override the provided group value.
 
             If no group value is provided, it is assumed the report resides
             in the current user's workspace.
-        
+
         """
 
         if isinstance(report, Report):
             report_id = report.id
         else:
             report_id = report
-        
+
         # If we got report, use its group_id and ignore provided
         if isinstance(report, Report):
             group_id = report.group_id
         else:
             if isinstance(group, Group):
                 group_id = group.id
             else:
                 group_id = group
-        
+
         if group_id:
             resource = self.BASE_URL + f"/groups/{group_id}/reports/{report_id}"
         else:
             resource = self.BASE_URL + f"/reports/{report_id}"
-        
+
         self.delete(resource, self.session)
```

### Comparing `pbipy-2.2.4/pbipy/reports.py` & `pbipy-2.3.4/pbipy/reports.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.2.4/pbipy/resources.py` & `pbipy-2.3.4/pbipy/resources.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.2.4/pbipy/utils.py` & `pbipy-2.3.4/pbipy/utils.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.2.4/pbipy.egg-info/PKG-INFO` & `pbipy-2.3.4/pbipy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbipy
-Version: 2.2.4
+Version: 2.3.4
 Summary: A Python Library for interacting with the Power BI Rest API.
 Home-page: https://github.com/andrewvillazon/pbipy
 Author: Andrew Villazon
 Author-email: andrew.villazon@gmail.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -21,15 +21,15 @@
 # pbipy
 
 ![PyPI](https://img.shields.io/pypi/v/pbipy) ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/andrewvillazon/pbipy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pbipy) ![GitHub](https://img.shields.io/github/license/andrewvillazon/pbipy) ![Static Badge](https://img.shields.io/badge/Python-blue?logo=python&logoColor=yellow) ![Static Badge](https://img.shields.io/badge/power-bi-yellow?logoColor=yellow&labelColor=yellow&color=black)
 
 
 `pbipy` is a Python Library for interacting with the Power BI Rest API. It aims to simplyify working with the Power BI Rest API and support programatic administration of Power BI in Python.
 
-`pbipy` supports operations for Reports, Datasets, and Groups (Workspaces), allowing users to perform actions on their PowerBI instance using Python.
+`pbipy` supports operations for Apps, Datasets, Groups (Workspaces) and Reports, allowing users to perform actions on their PowerBI instance using Python.
 
 See [development progress](#development-progress) below for what's been implemented and what's coming.
 
 ## Installation
 
 ```console
 pip install pbipy
@@ -57,15 +57,15 @@
 
 * [Power BI REST API with Python and MSAL. Part II.](https://www.datalineo.com/post/power-bi-rest-api-with-python-and-msal-part-ii)
 * [Power BI REST API with Python Part III, azure-identity](https://www.datalineo.com/post/power-bi-rest-api-with-python-part-iii-azure-identity)
 * [Monitoring Power BI using REST APIs from Python](https://data-goblins.com/power-bi/power-bi-api-python)
 
 The example below uses the `msal` library to to get a `bearer_token`.
 
-## Quickstart
+## Useage
 
 Start by creating the `PowerBI()` client. All interactions with the Power BI Rest API go through this object. 
 
 ```python
 import msal
 
 from pbipy import PowerBI
@@ -86,16 +86,14 @@
     scopes=["https://analysis.windows.net/powerbi/api/.default"],
 )
 
 # Create Client
 pbi = PowerBI(bearer_token)
 ```
 
-### Functionality
-
 To interact with the API, simply call the relevant method from the client.
 
 ```python
 # Grab the datasets from a workspace
 
 pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
 ```
@@ -138,40 +136,39 @@
 #   "name": "SalesMarketing",
 #   "addRowsAPIEnabled": False,
 #   "configuredBy": "john@contoso.com",
 #   ...
 # }
 ```
 
-## Examples
+## Example: Working with Datasets
+
+Let's see how `pbipy` works by performing some operations on a Dataset.
 
-### Datasets
+First, we need to load the Dataset from the API. To do this, we call the `dataset()` method from the `pbi` client we created above. 
 
-#### Get a dataset
+The Power BI Rest API will look for the Dataset in the current user's workspace if we don't provide a group argument.
 
 ```python
 sales = pbi.dataset(id="cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 print(sales)
 
 # <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
 ```
 
-#### Get a list of Datasets in a Workspace (Group)
+But we likely want to target a Dataset in a *Workspace*. To do this, we provide the `group_id` when we call the `dataset()` method.
 
 ```python
-datasets = pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
-
-for dataset in datasets:
-    print(dataset)
-
-# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', ...>
-# <Dataset id='f7fc6510-e151-42a3-850b-d0805a391db0', ...>
+sales = pbi.dataset(
+    "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
+    group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
+)
 ```
 
-#### Refresh History of a Dataset
+Now that we've got our target Dataset let's look at its Refresh History. We call the `refresh_history()` method on our Dataset. Easy.
 
 ```python
 dataset = pbi.dataset(
     "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
     group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
 )
 
@@ -179,24 +176,24 @@
 
 for entry in refresh_history:
     print(entry)
 
 # {"refreshType":"ViaApi", "startTime":"2017-06-13T09:25:43.153Z", "status": "Completed" ...}
 ```
 
-#### Add user permissions to a Dataset
+How about adding some user permissions to our Dataset? That's easy too. Just call the `add_user()` method with the User's details and permissions.
 
 ```python
 sales_ds = pbi.dataset( "cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 
 # Give John 'Read' access on the dataset
 sales_ds.add_user("john@contoso.com", "User", "Read")
 ```
 
-### Execute a DAX Query
+Lastly, if we're feeling adventurous, we can execute DAX against a Dataset and use the results in Python.
 
 ```python
 dataset = pbi.dataset( "cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 
 dxq_result = dataset.execute_queries("EVALUATE VALUES(MyTable)")
 print(dxq_result)
 
@@ -210,40 +207,50 @@
 #               "MyTable[Year]": 2010,
 #               "MyTable[Quarter]": "Q1"
 #             },
 # ...
 # }
 ```
 
-### Workspaces (Groups) *
+## More examples
+
+### Datasets in a Workspace
+
+```python
+datasets = pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
 
-*\* In the Power BI Rest API, workspaces are referred to as "groups".*
+for dataset in datasets:
+    print(dataset)
+
+# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', ...>
+# <Dataset id='f7fc6510-e151-42a3-850b-d0805a391db0', ...>
+```
 
-#### List Workspaces
+### List Workspaces
 
 ```python
 groups = pbi.groups()
 
 for group in groups:
     print(group)
 
 # <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
 # <Group id='3d9b93c6-7b6d-4801-a491-1738910904fd', name='marketing'>
 ```
 
-#### Create a Workspace
+### Create a Workspace
 
 ```python
 group = pbi.create_group("contoso")
 print(group)
 
 # <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
 ```
 
-#### Users and their access
+### Users and their access
 
 ```python
 group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
 users = group.users()
 
 for user in users:
     print(user)
@@ -257,23 +264,24 @@
 `pbipy` methods wrap around the Operations described in the Power BI Rest API Reference:
 
 [Power BI REST APIs for embedded analytics and automation - Power BI REST API](https://learn.microsoft.com/en-us/rest/api/power-bi/)
 
 
 ## Development Progress
 
-`pbipy` is in the early stages of development so expect a few features to be missing. The aim is to cover off most of the core stuff like Datasets, Workspaces (Groups), Reports, Apps, etc., and the rest later on. Check back regularly to see what's been added or still in the pipeline.
+`pbipy` is in development so expect a few features to be missing. The aim is to cover off most of the core stuff like Datasets, Workspaces (Groups), Reports, Apps, etc., and the rest later on. Check back regularly to see what's been added or still in the pipeline.
 
 | PowerBI Component   	| Progress 	| Notes 	|
 |---------------------	|----------	|-------	|
 | Datasets            	| Done     	|       	|
 | Groups (Workspaces) 	| Done    	|       	|
 | Reports             	| Done      |       	|
-| Apps                	| Doing   	|       	|
-| Dataflows           	| Todo     	|       	|
+| Apps                	| Done   	|       	|
+| Dataflows           	| Doing    	|       	|
+| Admin Operations     	| Todo     	|       	|
 | Dashboards          	| Todo     	|       	|
 | Everything else     	| Backlog  	|       	|
 
 ## Contributing
 
 Contributions such as bug reports, fixes, documentation or docstrings, enhancements, and ideas are welcome. `pbipy` uses github to host code, track issues, record feature requests, and accept pull requests.
```

### Comparing `pbipy-2.2.4/setup.py` & `pbipy-2.3.4/setup.py`

 * *Files identical despite different names*

