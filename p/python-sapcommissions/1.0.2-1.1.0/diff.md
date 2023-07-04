# Comparing `tmp/python-sapcommissions-1.0.2.tar.gz` & `tmp/python-sapcommissions-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sapcommissions-1.0.2.tar", last modified: Tue Jun 27 14:08:07 2023, max compression
+gzip compressed data, was "python-sapcommissions-1.1.0.tar", last modified: Tue Jul  4 11:54:43 2023, max compression
```

## Comparing `python-sapcommissions-1.0.2.tar` & `python-sapcommissions-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.967275 python-sapcommissions-1.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.967275 python-sapcommissions-1.0.2/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.github/workflows/pr-labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    12172 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/docs/ENDPOINTS.md
--rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/python_sapcommissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-06-27 14:08:07.000000 python-sapcommissions-1.0.2/python_sapcommissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-27 14:08:07.000000 python-sapcommissions-1.0.2/python_sapcommissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:08:07.000000 python-sapcommissions-1.0.2/python_sapcommissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 14:08:07.000000 python-sapcommissions-1.0.2/python_sapcommissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 14:08:07.000000 python-sapcommissions-1.0.2/python_sapcommissions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/sapcommissions/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/sapcommissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25047 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/sapcommissions/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/sapcommissions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)   112297 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/sapcommissions/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:08:07.971275 python-sapcommissions-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/tests/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-27 14:08:00.000000 python-sapcommissions-1.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:54:43.641547 python-sapcommissions-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:54:43.637547 python-sapcommissions-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:54:43.637547 python-sapcommissions-1.1.0/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:54:43.637547 python-sapcommissions-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/.github/workflows/pr-labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:54:43.637547 python-sapcommissions-1.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-04 11:54:43.641547 python-sapcommissions-1.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:54:43.637547 python-sapcommissions-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    57710 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/docs/ENDPOINTS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/docs/METHODS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:54:43.637547 python-sapcommissions-1.1.0/python_sapcommissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-04 11:54:43.000000 python-sapcommissions-1.1.0/python_sapcommissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-04 11:54:43.000000 python-sapcommissions-1.1.0/python_sapcommissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 11:54:43.000000 python-sapcommissions-1.1.0/python_sapcommissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-04 11:54:43.000000 python-sapcommissions-1.1.0/python_sapcommissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-04 11:54:43.000000 python-sapcommissions-1.1.0/python_sapcommissions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:54:43.641547 python-sapcommissions-1.1.0/sapcommissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/sapcommissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58092 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/sapcommissions/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/sapcommissions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114107 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/sapcommissions/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 11:54:43.641547 python-sapcommissions-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:54:43.641547 python-sapcommissions-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/tests/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-04 11:54:34.000000 python-sapcommissions-1.1.0/tox.ini
```

### Comparing `python-sapcommissions-1.0.2/.github/scripts/release.py` & `python-sapcommissions-1.1.0/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.0.2/.github/workflows/lint.yml` & `python-sapcommissions-1.1.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.0.2/.github/workflows/publish.yml` & `python-sapcommissions-1.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.0.2/.pre-commit-config.yaml` & `python-sapcommissions-1.1.0/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 default_language_version:
-  python: python3.11
+  python: python3.10
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-added-large-files
       - id: check-ast
       - id: check-builtin-literals
@@ -32,11 +32,15 @@
       - id: black
 
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
 
-  - repo: https://github.com/pycqa/pylint
-    rev: v2.17.4
+  - repo: local
     hooks:
       - id: pylint
+        name: pylint
+        entry: .venv/Scripts/pylint.exe
+        language: system
+        types: [python]
+        require_serial: true
```

### Comparing `python-sapcommissions-1.0.2/LICENSE` & `python-sapcommissions-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.0.2/PKG-INFO` & `python-sapcommissions-1.1.0/docs/METHODS.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,169 +1,84 @@
-Metadata-Version: 2.1
-Name: python-sapcommissions
-Version: 1.0.2
-Summary: A Python wrapper for the SAP Commissions API
-Author-email: Niels Perfors <niels.perfors1987@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/niro1987/python-sapcommissions
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# SAP Commissions
-
-A Python wrapper for the SAP Commissions API.
-
-- [SAP Commissions](#sap-commissions)
-  - [Installation](#installation)
-    - [REST API](#rest-api)
-    - [Terminology](#terminology)
-  - [Usage](#usage)
-  - [Methods](#methods)
-    - [List](#list)
-    - [Get](#get)
-    - [Get ID](#get-id)
-    - [Get Versions](#get-versions)
-    - [Create](#create)
-    - [Create Versions](#create-versions)
-    - [Update](#update)
-    - [Update Versions](#update-versions)
-    - [Delete](#delete)
-    - [Delete Versions](#delete-versions)
+# Methods
 
-## Installation
+Every endpoint exposes a number of methods. The most common are `list()` and `get()`. Some endpoints also expose
+`create()`, `update()`, and `delete()` methods. Versioned endpoints like `Participants` also expose `get_versions()`,
+`create_versions()`, `update_versions()` and `delete_versions()` methods.
 
-To install the project, run the following command:
+## List
 
-```text
-pip install python-sapcommissions
-```
-
-### REST API
-
-This project mimics the usage of the SAP Commissions REST API. Visit
-`https://{CALD}-{ENV}.callidusondemand.com/APIDocument` to read the full specification,
-replacing `CALD` with your tenant name, and `ENV` with your environment name.
-
-### Terminology
-
-In this documentation, we talk about endpoints and resources, here is what that means.
-
-| Keyword  | Description                                                                      |
-| -------- | -------------------------------------------------------------------------------- |
-| Endpoint | A type of object that we can interact with, like `Participants` and `Positions`. |
-| Method   | An action to perform on an endpoint. See [Methods](#methods) below.              |
-| Resource | An instance of an endpoint, a single `Participant` or `Position` for example.    |
+The `list()` method is used to retrieve multiple resources from the endpoint. By default, it returns the current
+effective version of the resource (if the endpoint is versioned). To retrieve a different effective version, you must
+provide both `startDate` and `endDate` parameters.
 
-## Usage
+Due to the potentially huge amount of requests to the endpoint, the `list()` method actually returns a `generator`
+object, not a `list`. Depending on the `limit` parameter, the `list()` method requests up to 100 resources at a time.
 
-To get started, import `Connection` and an endpoint of your choosing. In this
-example, we'll use `Participants` as the endpoint.
-
-```py
-from sapcommissions import Connection
-from sapcommissions.endpoints import Participants
-```
-
-Initialize a Connection by providing the tenant, environment, username,
-and password. Optionally, you can disable ssl verification, if you have problems
-connecting to the API from your corporate network.
-
-```python
-prod = Connection("CALD", "PRD", "MyUserName", "MySuperSecretPassword", verify_ssl=False)
-```
+In most cases, you will want to apply some kind of filter. For a complete list of available filter options please visit
+the [REST API Documentation](README.md#rest-api).
 
-We'll use the `Participants` endpoint to get a list of all participants in the environment.
+You can limit the number of results returned by providing a `limit`, this is usefull if you want to explore the data if
+the endpoint holds a lot of instances. Provide the `raw = True` parameter to return the json response from the API
+without converting it to a Python object.
 
-```py
-all_users = Participants(prod).list()
-```
-
-## Methods
-
-Every endpoint exposes a number of methods. The most common are `list()` and `get()`.
-Some endpoints also expose `create()`, `update()`, and `delete()` methods. Versioned
-endpoints like `Participants` also expose `get_versions()`, `create_versions()`, `update_versions()`
-and `delete_versions()` methods.
-
-### List
-
-The `list()` method is used to retrieve multiple resources from the endpoint. By default, it returns
-the current effective version of the resource (if the endpoint is versioned). To retrieve a
-different effective version, you must provide both `startDate` and `endDate` parameters.
-
-In most cases, you will want to apply some kind of filter. For a complete list of available filter
-options please visit the [REST API Documentation](#rest-api).
-
-You can limit the number of results returned by providing a `limit`, this is usefull if you want to
-explore the data if the endpoint holds a lot of instances. Provide the `raw = True` parameter to
-return the json response from the API without converting it to a Python object.
-
-Provide `filter_kwargs` keyword arguments to apply a quick filter. For example
-`Positions(prod).list(name='John Doe')` is equivalent to
-`Positions(prod).list(filter="name eq 'John Doe'")`. Providing `filter` and `filter_kwargs` will
+Provide `filter_kwargs` keyword arguments to apply a quick filter. For example `Positions(prod).list(name='John Doe')`
+is equivalent to `Positions(prod).list(filter="name eq 'John Doe'")`. Providing `filter` and `filter_kwargs` will
 combine the arguments using the `and` operator, as will multiple `filter_kwargs` arguments.
 
 ```py
-# Get a list of all positions in the environment.
+# Get all positions.
 positions = Positions(prod).list()
 
-# Get a list of all positions with title 'Sales Manager'.
+# Get all positions with title 'Sales Manager'.
 sales_managers = Positions(prod).list(filter="title/name eq 'Sales Manager'")
 ```
 
 | Argument      | Type   | Required                   | Description                                      |
 | ------------- | ------ | -------------------------- | ------------------------------------------------ |
 | filter        | `str`  | False                      | A filter string to apply to the list             |
 | startDate     | `date` | False if endDate is None   | Filter list of resources effective for startDate |
 | endDate       | `date` | False if startDate is None | Filter list of resources effective for endDate   |
 | limit         | `int`  | False                      | Limit the number of returned resources           |
 | raw           | `bool` | False                      | Return the raw json response from the API        |
 | filter_kwargs | `dict` | False                      | Keyword arguments to apply to the filter         |
 
-| Returns          | Description                               |
-| ---------------- | ----------------------------------------- |
-| `list[Resource]` | A list of resources, single valid version |
-
-### Get
-
-The `get()` method is used to retrieve an existing resource, single (latest) version.
-The method takes a single parameter, `seq` (system unique identifier) of the object to
-retrieve. The `seq` value for a resource is stored in the first attribute, for
-simplicity, it can also be read from the `_seq` property.
+| Returns               | Description                                    |
+| --------------------- | ---------------------------------------------- |
+| `generator<Resource>` | A generator of resources, single valid version |
+
+## Get
+
+The `get()` method is used to retrieve an existing resource, single (latest) version. The method takes a single
+parameter, `seq` (system unique identifier) of the object to retrieve. The `seq` value for a resource is stored in the
+first attribute, for simplicity, it can also be read from the `_seq` property.
 
 | Argument | Type  | Required | Description                                   |
 | -------- | ----- | -------- | --------------------------------------------- |
 | seq      | `int` | True     | The system unique identifier for the resource |
 
 | Returns    | Description                              |
 | ---------- | ---------------------------------------- |
 | `Resource` | Requested resource, single valid version |
 
 ```py
-# Let's say we retrieve a list of positions from the API. The manager attribute refers to a
-# position, but does not contain any meaningfull information about the manager yet.
-# We can use the `get()` method to enrich the manager data.
+# Let's say you retrieve a list of positions from the API. The manager attribute refers
+# to a position, but does not contain any meaningfull information about the manager yet.
+# You can use the `get()` method to enrich the manager data.
 positions = Positions(prod).list()
 
 for position in positions:
   if position.manager:
-    position.manager = Positions(prod).get(position.manager._seq)
+    position.manager = Positions(prod).get(position.manager.ruleElementOwnerSeq)
 ```
 
-### Get ID
+## Get ID
 
-`get_id()` is a helper method to simplify the retrieval of a resource by its ID (user
-unique identifier). The method takes a single parameter, `id`. If the resource does not provide an
-id, or the specified `id` could not be found, it returns `None`.
+`get_id()` is a helper method to simplify the retrieval of a resource by its ID (user unique identifier). The method
+takes a single parameter, `id`. If the resource does not provide an id, or the specified `id` could not be found, it
+returns `None`.
 
 | Argument | Type  | Required | Description                                 |
 | -------- | ----- | -------- | ------------------------------------------- |
 | id       | `str` | True     | The user unique identifier for the resource |
 
 | Returns    | Description                                        |
 | ---------- | -------------------------------------------------- |
@@ -175,161 +90,158 @@
 
 # What would have been required without this method.
 position_id_attr = Position._id_attr  # returns 'name'
 positions = Positions(prod).list(filter=f"{position_id_attr} eq 'John Doe'")
 position = positions[0] if positions else None
 ```
 
-### Get Versions
+## Get Versions
 
-The `get_versions()` method is simmilar to the [Get](#get) method, it returns a list
-of all versions of the resource.
+The `get_versions()` method is simmilar to the [Get](#get) method, it returns a list of all versions of the resource.
 
 | Argument | Type  | Required | Description                                   |
 | -------- | ----- | -------- | --------------------------------------------- |
 | seq      | `int` | True     | The system unique identifier for the resource |
 
-| Returns          | Description                             |
-| ---------------- | --------------------------------------- |
-| `list[Resource]` | A list of all versions for a  resources |
+| Returns          | Description                            |
+| ---------------- | -------------------------------------- |
+| `list[Resource]` | A list of all versions for a resources |
 
 ```py
 # Get all versions for a position.
 positions = Positions(prod).list()
 position = positions[0]
 
-position_versions = Positions(prod).get_versions(first_position._seq)
+position_versions = Positions(prod).get_versions(first_position.ruleElementOwnerSeq)
 ```
 
-### Create
+## Create
 
-With the `create()` method, you can create a new instance of the resource. Unlike the
-REST API, the `create()` method accepts only a single resource as a parameter.
-If successful, the created resource will be returned.
+With the `create()` method, you can create a new instance of the resource. Unlike the REST API, the `create()` method
+accepts only a single resource as a parameter. If successful, the created resource will be returned.
 
 | Argument | Type       | Required | Description                     |
 | -------- | ---------- | -------- | ------------------------------- |
 | instance | `Resource` | True     | The resource instance to create |
 
 | Returns    | Description             |
 | ---------- | ----------------------- |
 | `Resource` | Created resource object |
 
-Make sure to provide all required attributes for the resource. Check the documentation
-for the resource to see which attributes are required.
+Make sure to provide all required attributes for the resource. Check the documentation for the resource to see which
+attributes are required.
 
 ```py
 # Create a new position, with title 'Account Manager'.
 new_position = Position(
   name="John Doe",
   effectiveStartDate=date(2020, 1, 1),
   effectiveEndDate=date(2200, 1, 1),
   title=Title(name="Account Manager"),
 )
 created_position = Positions(prod).create(new_position)
 ```
 
-### Create Versions
+## Create Versions
 
-The `create_versions()` method is used to create new versions of an existing resource.
-It is imperative that you provide all versions of the resource, as this method will
-overwrite all pre-existing versions with the ones provide. This method can also be used
-to end-date an existing resource. All pre-existing versions of the resource will be
-overwritten.
+The `create_versions()` method is used to create new versions of an existing resource. It is imperative that you provide
+all versions of the resource, as this method will overwrite all pre-existing versions with the ones provide. This method
+can also be used to end-date an existing resource. All pre-existing versions of the resource will be overwritten.
 
 | Argument  | Type             | Required | Description                                   |
 | --------- | ---------------- | -------- | --------------------------------------------- |
 | seq       | `int`            | True     | The system unique identifier for the resource |
 | instances | `list[Resource]` | True     | The list of resource instances to create      |
 
 | Returns          | Description                       |
 | ---------------- | --------------------------------- |
 | `list[Resource]` | List of created resource versions |
 
 ```py
-# Let's create a new version of the position that we just created.
+# Let's create a new version of the position that you just created.
 first_version = Position(
   name="John Doe",
   effectiveStartDate=date(2020, 1, 1),
   effectiveEndDate=date(2020, 12, 31),
   title=Title(name="Account Manager"),
 )
 second_version = Position(
   name="John Doe",
   effectiveStartDate=date(2021, 1, 1),
   effectiveEndDate=date(2200, 1, 1),
   title=Title(name="Sales Manager"),
 )
 versions = [first_version, second_version]
 
-created_versions = Positions(prod).create_versions(created_position._seq, versions)
+created_versions = Positions(prod).create_versions(
+  created_position.ruleElementOwnerSeq,
+  versions,
+)
 ```
 
-### Update
+## Update
 
-With the `update()` method, you can update an existing resource. If the endpoint is
-versioned, this methid only updates a single valid version, matching the effective date
-range provided.
+With the `update()` method, you can update an existing resource. If the endpoint is versioned, this methid only updates
+a single valid version, matching the effective date range provided.
 
 | Argument | Type       | Required | Description                   |
 | -------- | ---------- | -------- | ----------------------------- |
 | update   | `Resource` | True     | The updated resource instance |
 
 | Returns    | Description                                   |
 | ---------- | --------------------------------------------- |
 | `Resource` | Updated resource object, single valid version |
 
 ```py
-#  Say that you want to assign all positions with title 'Account Manager' or 'Sales Manager'
-# to a position group 'Sales'. We'll assume that the position group already exists.
+# Say that you want to assign all positions with title 'Account Manager' or
+# 'Sales Manager' to a position group 'Sales'. Let's assume that the position group
+# already exists.
 
 # Get a list of all positions with title 'Account Manager' or 'Sales Manager'.
 positions = (
   Positions(prod)
   .list(filter="title/name eq 'Account Manager' or title/name eq 'Sales Manager'")
 )
 
 # Now update the position group and update the position.
-for position in positions
+for position in positions:
   position.positionGroup = PositionGroup(name="Sales")
   Positions(prod).update(position)
 ```
 
-### Update Versions
+## Update Versions
 
-The `update_versions()` method is used to update the versions of an existing resource.
-It is important to understand the differance between `update()` and `update_versions()`.
-[Update](#update) allows a single valid version of the resource to be updated, it must
-pre-exist in the environment. With `update_versions()`, you can update multiple versions
-at once, and even apply an update without any prior knowledge of pre-existing versions.
-The provided versions will be applied to the current existing versions in the
-environment.
+The `update_versions()` method is used to update the versions of an existing resource. It is important to understand the
+differance between `update()` and `update_versions()`. [Update](#update) allows a single valid version of the resource
+to be updated, it must pre-exist in the environment. With `update_versions()`, you can update multiple versions at once,
+and even apply an update without any prior knowledge of pre-existing versions. The provided versions will be applied to
+the current existing versions in the environment.
 
 | Argument | Type             | Required | Description                                   |
 | -------- | ---------------- | -------- | --------------------------------------------- |
 | seq      | `int`            | True     | The system unique identifier for the resource |
 | versions | `list[Resource]` | True     | The list of resource version update to apply  |
 
 | Returns          | Description                                                |
 | ---------------- | ---------------------------------------------------------- |
 | `list[Resource]` | List of all resource versions after the update was applied |
 
 **Example:**
 
 ```py
-# Let's revisit our previous example where a position is promoted to a different title. Our position
-# already has two versions, the first with a title of 'Account Manager', the second with a title of
-# 'Sales Manager' and position group 'Sales'. We can update the position without any pre-existing
-# knowledge of these versions.
+# Let's revisit our previous example where a position is promoted to a different title.
+# Our position already has two versions, the first with a title of 'Account Manager',
+# the second with a title of 'Sales Manager' and position group 'Sales'. You can update
+# the position without any pre-existing knowledge of these versions.
 
-# We'll need to seq number for the position that we are going to update.
+# You'll need to seq number for the position that you are going to update.
 positions = Positions(prod).list(filter="name eq 'John Doe'")
 position = positions[0]
 
-# Now we can update the position
+# Now you can update the position
 updated_position = Position(
   name="John Doe",
   effectiveStartDate=date(2022, 1, 1),
   effectiveEndDate=date(2200, 1, 1),
   title=Title(name="Director"),
   positionGroup=PositionGroup(name="Management"),
 )
@@ -356,62 +268,62 @@
 #     effectiveEndDate=date(2200, 1, 1)
 #     title=Title(name="Director"),
 #     positionGroup=PositionGroup(name="Management"),
 #   ),
 # ]
 ```
 
-### Delete
+## Delete
 
-With the `delete()` method, you can fully delete a resource from the environment, all
-effective versions of the resource will be deleted.
+With the `delete()` method, you can fully delete a resource from the environment, all effective versions of the resource
+will be deleted.
 
 | Argument | Type  | Required | Description                                   |
 | -------- | ----- | -------- | --------------------------------------------- |
 | seq      | `int` | True     | The system unique identifier for the resource |
 
 | Returns | Description                                                |
 | ------- | ---------------------------------------------------------- |
 | `str`   | Confirmation message `The record is successfully deleted.` |
 
 ```py
 # Delete a position with the name 'John Doe'.
 positions = Positions(prod).list(filter="name eq 'John Doe'")
 position = positions[0]
 
-message = Positions(prod).delete(position._seq)
+message = Positions(prod).delete(position.ruleElementOwnerSeq)
 assert message == "The record is successfully deleted."
 ```
 
-### Delete Versions
+## Delete Versions
 
-The `delete_versions()` method deletes the given versions of the resource. The resulting
-gap will either be filled from the previous or next available version of the resource.
-The effective dates provided must match an existing version of the resource.
+The `delete_versions()` method deletes the given versions of the resource. The resulting gap will either be filled from
+the previous or next available version of the resource. The effective dates provided must match an existing version of
+the resource.
 
 | Argument           | Type   | Required | Description                                          |
 | ------------------ | ------ | -------- | ---------------------------------------------------- |
 | seq                | `int`  | True     | The system unique identifier for the resource        |
 | effectiveStartDate | `date` | True     | The start date of the version to delete              |
 | effectiveEndDate   | `date` | True     | The end date of the version to delete                |
 | fillFromRight      | `bool` | False    | Default `True`, fill from the next available version |
 
 | Returns | Description                                                                  |
 | ------- | ---------------------------------------------------------------------------- |
 | `str`   | Confirmation message `All versions in given range are deleted successfully.` |
 
 ```py
-# Remove the latest version of a position with the name 'John Doe' and fill the gap from the
-# previous version.
+# Remove the latest version of a position with the name 'John Doe' and fill the gap from
+# the previous version.
 positions = Positions(prod).list(filter="name eq 'John Doe'")
 position = positions[0]
 
 message = (
   Positions(prod)
   .delete_versions(
-    seq=position._seq,
+    seq=position.ruleElementOwnerSeq,
     effectiveStartDate=position.effectiveStartDate,
     effectiveEndDate=position.effectiveEndDate,
     fillFromRight=False
   )
 )
 ```
```

### Comparing `python-sapcommissions-1.0.2/pyproject.toml` & `python-sapcommissions-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [project]
 name = "python-sapcommissions"
 description = "A Python wrapper for the SAP Commissions API"
 authors = [
     {name = "Niels Perfors", email = "niels.perfors1987@gmail.com"},
 ]
 license = {text = "MIT"}
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
@@ -40,27 +40,26 @@
 [project.optional-dependencies]
 dev = [
     "pycodestyle",
     "pylint",
     "flake8",
     "black",
     "isort",
+    "pre-commit",
 ]
 
 [tool.black]
 line-length = 88
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint.MAIN]
 py-version = "3.11"
-ignore = [
-    "tests"
-]
+ignore-patterns="tests/*"
 
 load-plugins = [
     "pylint.extensions.code_style",
     "pylint.extensions.typing"
 ]
 
 [tool.pylint.BASIC]
```

### Comparing `python-sapcommissions-1.0.2/python_sapcommissions.egg-info/SOURCES.txt` & `python-sapcommissions-1.1.0/python_sapcommissions.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 .github/scripts/release.py
 .github/workflows/lint.yml
 .github/workflows/pr-labeler.yml
 .github/workflows/publish.yml
 .github/workflows/release.yml
 .vscode/settings.json
 docs/ENDPOINTS.md
+docs/METHODS.md
 docs/README.md
 python_sapcommissions.egg-info/PKG-INFO
 python_sapcommissions.egg-info/SOURCES.txt
 python_sapcommissions.egg-info/dependency_links.txt
 python_sapcommissions.egg-info/requires.txt
 python_sapcommissions.egg-info/top_level.txt
 sapcommissions/__init__.py
```

### Comparing `python-sapcommissions-1.0.2/sapcommissions/resources.py` & `python-sapcommissions-1.1.0/sapcommissions/resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 from datetime import date, datetime, timezone
 from types import UnionType
 from typing import ClassVar, get_args, get_origin, get_type_hints
 
 LOGGER = logging.getLogger(__name__)
 
 
-def _decode(value, astype):  # pylint: disable=too-many-return-statements
+def _deserialize(value, astype):  # pylint: disable=too-many-return-statements
     if isinstance(value, list):
         if astype is list:
             LOGGER.error("Unknown type for list elements: %s", astype)
             raise TypeError("Unknown type for list elements")
         if get_origin(astype) is list:
             if len(subtypes := get_args(astype)) > 1:
                 LOGGER.error("Impropper type for list elements: %s", subtypes)
                 raise TypeError("Impropper type for list elements")
-            return [_decode(v, subtypes[0]) for v in value]
+            return [_deserialize(v, subtypes[0]) for v in value]
         LOGGER.error("Impropper type, value is list: %s", astype)
         raise TypeError("Impropper type, value is list")
     if isinstance(astype, UnionType):
         LOGGER.error("UnionType is not supported: %s", astype)
         raise NotImplementedError("Unsupported type")
     if value is None:
         return None
@@ -38,24 +38,24 @@
     if issubclass(astype, _Resource) and isinstance(value, dict):
         return astype.from_dict(value)
     if issubclass(astype, _Resource) and isinstance(value, (str, int)):
         return astype(**{astype._seqAttr: value})  # pylint: disable=protected-access
     return astype(value)
 
 
-def _encode(value, fromtype):
+def _serialize(value, fromtype):
     if isinstance(value, list):
         if fromtype is list:
             LOGGER.error("Unknown type for list elements: %s", fromtype)
             raise TypeError("Unknown type for list elements")
         if get_origin(fromtype) is list:
             if len(subtypes := get_args(fromtype)) > 1:
                 LOGGER.error("Impropper type for list elements: %s", subtypes)
                 raise TypeError("Impropper type for list elements")
-            return [_decode(v, subtypes[0]) for v in value]
+            return [_serialize(v, subtypes[0]) for v in value]
         LOGGER.error("Impropper type, value is list: %s", fromtype)
         raise TypeError("Impropper type, value is list")
     if isinstance(fromtype, UnionType):
         LOGGER.error("UnionType is not supported: %s", fromtype)
         raise NotImplementedError("Unsupported type")
     if value is None:
         return None
@@ -64,83 +64,120 @@
     if isinstance(value, _Resource):
         return value.to_dict(ignoreSeq=False)
     if isinstance(value, int):
         return value
     return str(value)
 
 
+def _meta(
+    seq: bool = False,
+    id: bool = False,  # pylint: disable=redefined-builtin
+    expand: bool = False,
+    json_ignore: bool = False,  # pylint: disable=invalid-name
+):
+    """Helper function to create metadata for a field."""
+    return {
+        "seq": seq,
+        "id": id,
+        "expand": expand,
+        "json_ignore": json_ignore,
+    }
+
+
 class _Resource:
     _endpoint_name: ClassVar[str]
 
     @classmethod
     @property
     def _name(cls) -> str:
         """Returns the name resource."""
         return cls._endpoint_name
 
     @classmethod
     @property
     def _seqAttr(cls) -> str | None:
         """Returns the name of the sequence attribute or None."""
         for fld in fields(cls):
-            if fld.metadata.get("seq"):
+            if fld.metadata.get("seq") is True:
                 return fld.name
         return None
 
     @property
     def _seq(self) -> int | None:
         """Returns the sequence or None."""
         seq_attr = self._seqAttr
         return self[seq_attr] if seq_attr else None
 
     @classmethod
     @property
     def _idAttr(cls) -> str | None:
         """Returns the name of the identifier attribute or None."""
         for fld in fields(cls):
-            if fld.metadata.get("id"):
+            if fld.metadata.get("id") is True:
                 return fld.name
         return None
 
     @property
     def _id(self) -> str | None:
         """Returns the identifier or None."""
         id_attr = self._idAttr
         return self[id_attr] if id_attr else None
 
     @classmethod
     @property
     def _expands(cls) -> tuple:
         """Returns the name of the expandable attributes."""
-        return tuple(f.name for f in fields(cls) if f.metadata.get("expand"))
+        return tuple(
+            fld.name
+            for fld in fields(cls)
+            if fld.type not in ("str", "int", "date", "datetime", "bool", "Value")
+            or fld.metadata.get("expand") is True
+        )
 
     @classmethod
     def from_dict(cls, json: dict) -> _Resource:
         """Convert dictionary to _Resource instance."""
+        reference_keys = ("objectType", "key", "displayName")
+        if all(key in json for key in reference_keys):
+            if (object_type := json["objectType"]) != cls.__name__:
+                LOGGER.error("Reference mismatch %s -> %s", object_type, cls.__name__)
+                raise TypeError("Reference mismatch")
+            seq_value = json["key"]
+            id_value = json["displayName"]
+            json.clear()
+            if (seq_attr := cls._seqAttr) is not None:
+                json[seq_attr] = seq_value
+            if (id_attr := cls._idAttr) is not None:
+                json[id_attr] = id_value
+
         types = get_type_hints(cls)
-        invalid_json = {k: v for k, v in json.items() if k not in types.keys()}
-        for field_name in invalid_json.keys():
-            LOGGER.warning("%s is not a valid field for %s", field_name, cls.__name__)
-        valid_json = {k: v for k, v in json.items() if k in types.keys()}
-        for field_name, value in valid_json.items():
-            valid_json[field_name] = _decode(value, types[field_name])
+        valid_json = {}
+
+        for field_name, value in json.items():
+            if field_name in types:
+                valid_json[field_name] = _deserialize(value, types[field_name])
+            else:
+                LOGGER.warning(
+                    "%s is not a valid field for %s", field_name, cls.__name__
+                )
+
         return cls(**valid_json)
 
     def to_dict(self, ignoreSeq: bool = True) -> dict:
         """Convert _Resource instance to dictionary."""
         types = get_type_hints(self.__class__)
         data = {}
         for fld in fields(self):
             if (value := self[fld.name]) is None:
                 continue
-            if fld.metadata.get("json_ignore"):
+            if fld.metadata.get("json_ignore") is True:
                 continue
-            if ignoreSeq and fld.metadata.get("seq"):
+            if ignoreSeq and fld.metadata.get("seq") is True:
                 continue
-            data[fld.name] = _encode(value, types[fld.name])
+            data[fld.name] = _serialize(value, types[fld.name])
         return data
 
     def __getitem__(self, attribute: str):
         return getattr(self, attribute)
 
 
 @dataclass(frozen=True)
@@ -168,116 +205,116 @@
     custId: str = field(default=None, repr=False)
     company: str = field(default=None, repr=False)
 
 
 @dataclass
 class AppliedDeposit(_Resource):
     _endpoint_name: ClassVar[str] = "appliedDeposits"
-    appliedDepositSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    appliedDepositSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     position: Position = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     earningGroupId: str = field(default=None, repr=False)
     earningCodeId: str = field(default=None, repr=False)
     trialPipelineRun: Pipeline = field(default=None, repr=False)
     trialPipelineRunDate: datetime = field(default=None, repr=False)
     postPipelineRun: Pipeline = field(default=None, repr=False)
     postPipelineRunDate: datetime = field(default=None, repr=False)
     entryNumber: int = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class AuditLog(_Resource):
     _endpoint_name: ClassVar[str] = "auditLogs"
-    auditLogSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    auditLogSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     businessUnit: BusinessUnit = field(default=None, repr=False)
     objectSeq: str = field(default=None, repr=False)
     eventDescription: str = field(default=None, repr=True)
     objectName: str = field(default=None, repr=False)
     eventType: str = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     userId: str = field(default=None, repr=False)
-    eventDate: date = field(default=None, repr=False)
+    eventDate: date = field(default=None, repr=True)
     objectType: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Balance(_Resource):
     _endpoint_name: ClassVar[str] = "balances"
-    balanceSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    balanceSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     position: Position = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     earningGroupId: str = field(default=None, repr=False)
     earningCodeId: str = field(default=None, repr=False)
     trialPipelineRun: Pipeline = field(default=None, repr=False)
     trialPipelineRunDate: datetime = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     applyPipelineRun: Pipeline = field(default=None, repr=False)
     applyPipelineRunDate: datetime = field(default=None, repr=False)
     postPipelineRun: Pipeline = field(default=None, repr=False)
     postPipelineRunDate: datetime = field(default=None, repr=False)
     balanceStatusId: str = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class BusinessUnit(_Resource):
     _endpoint_name: ClassVar[str] = "businessUnits"
-    businessUnitSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    businessUnitSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     mask: int = field(default=None, repr=False)
     smask: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Calendar(_Resource):
     _endpoint_name: ClassVar[str] = "calendars"
-    calendarSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    calendarSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     minorPeriodType: PeriodType = field(default=None, repr=False)
     majorPeriodType: PeriodType = field(default=None, repr=False)
-    periods: Period = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    periods: list[Period] = field(default=None, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Category(_Resource):
     _endpoint_name: ClassVar[str] = "categories"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    ruleElementSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     owner: CategoryTree = field(default=None, repr=False)
     parent: Category = field(default=None, repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     returnType: str = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=date(2200, 1, 1), repr=True)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     createDate: datetime = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
     genericAttribute3: str = field(default=None, repr=False)
     genericAttribute4: str = field(default=None, repr=False)
     genericAttribute5: str = field(default=None, repr=False)
     genericAttribute6: str = field(default=None, repr=False)
     genericAttribute7: str = field(default=None, repr=False)
@@ -306,85 +343,85 @@
     genericBoolean2: bool = field(default=None, repr=False)
     genericBoolean3: bool = field(default=None, repr=False)
     genericBoolean4: bool = field(default=None, repr=False)
     genericBoolean5: bool = field(default=None, repr=False)
     genericBoolean6: bool = field(default=None, repr=False)
     calendar: Calendar = field(default=None, repr=False)
     owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    ruleUsage: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class CategoryClassifier(_Resource):
     _endpoint_name: ClassVar[str] = "categoryClassifiers"
     categoryClassifiersSeq: int = field(
-        default=None, metadata={"seq": True}, repr=False
+        default=None, metadata=_meta(seq=True), repr=False
     )
     categoryTree: CategoryTree = field(default=None, repr=False)
     category: Category = field(default=None, repr=False)
     classifier: str = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=date(2200, 1, 1), repr=True)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class CategoryTree(_Resource):
     _endpoint_name: ClassVar[str] = "categoryTrees"
-    categoryTreeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    categoryTreeSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     name: str = field(default=None, repr=False)
     classifierSelectorId: str = field(default=None, repr=False)
     classifierClass: str = field(default=None, repr=False)
     description: str = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     ruleExpression: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Commission(_Resource):
     _endpoint_name: ClassVar[str] = "commissions"
-    commissionSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    commissionSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     position: Position = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     incentive: Incentive = field(default=None, repr=False)
     credit: Credit = field(default=None, repr=False)
     pipelineRun: Pipeline = field(default=None, repr=False)
     pipelineRunDate: datetime = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
     rateValue: Value = field(default=None, repr=False)
     entryNumber: str = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     isPrivate: bool = field(default=None, repr=False)
     originTypeId: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Credit(_Resource):
     _endpoint_name: ClassVar[str] = "credits"
-    creditSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    creditSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     name: str = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     position: Position = field(default=None, repr=False)
     salesOrder: SalesOrder = field(default=None, repr=False)
     salesTransaction: SalesTransaction = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     creditType: CreditType = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
@@ -398,15 +435,15 @@
     releaseDate: date = field(default=None, repr=False)
     pipelineRun: Pipeline = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     compensationDate: date = field(default=None, repr=False)
     comments: str = field(default=None, repr=False)
     pipelineRunDate: datetime = field(default=None, repr=False)
     isPrivate: bool = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
     genericAttribute3: str = field(default=None, repr=False)
     genericAttribute4: str = field(default=None, repr=False)
     genericAttribute5: str = field(default=None, repr=False)
     genericAttribute6: str = field(default=None, repr=False)
     genericAttribute7: str = field(default=None, repr=False)
@@ -433,62 +470,62 @@
     genericDate6: date = field(default=None, repr=False)
     genericBoolean1: bool = field(default=None, repr=False)
     genericBoolean2: bool = field(default=None, repr=False)
     genericBoolean3: bool = field(default=None, repr=False)
     genericBoolean4: bool = field(default=None, repr=False)
     genericBoolean5: bool = field(default=None, repr=False)
     genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class CreditType(_Resource):
     _endpoint_name: ClassVar[str] = "creditTypes"
-    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    creditTypeId: str = field(default=None, metadata={"id": True}, repr=True)
+    dataTypeSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    creditTypeId: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Customer(_Resource):
     _endpoint_name: ClassVar[str] = "customers"
-    classifierSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    classifierId: str = field(default=None, metadata={"id": True}, repr=True)
+    classifierSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    classifierId: str = field(default=None, metadata=_meta(id=True), repr=True)
     name: str = field(default=None, repr=False)
     description: str = field(default=None, repr=False)
     selectorId: str = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     address1: str = field(default=None, repr=False)
     address2: str = field(default=None, repr=False)
     address3: str = field(default=None, repr=False)
     city: str = field(default=None, repr=False)
     state: str = field(default=None, repr=False)
     country: str = field(default=None, repr=False)
     phone: str = field(default=None, repr=False)
     areaCode: str = field(default=None, repr=False)
     postalCode: str = field(default=None, repr=False)
     geography: str = field(default=None, repr=False)
     fax: str = field(default=None, repr=False)
     email: str = field(default=None, repr=False)
     industry: str = field(default=None, repr=False)
     contact: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
     genericAttribute3: str = field(default=None, repr=False)
     genericAttribute4: str = field(default=None, repr=False)
     genericAttribute5: str = field(default=None, repr=False)
     genericAttribute6: str = field(default=None, repr=False)
     genericAttribute7: str = field(default=None, repr=False)
@@ -515,42 +552,42 @@
     genericDate6: date = field(default=None, repr=False)
     genericBoolean1: bool = field(default=None, repr=False)
     genericBoolean2: bool = field(default=None, repr=False)
     genericBoolean3: bool = field(default=None, repr=False)
     genericBoolean4: bool = field(default=None, repr=False)
     genericBoolean5: bool = field(default=None, repr=False)
     genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Deposit(_Resource):
     _endpoint_name: ClassVar[str] = "deposits"
-    depositSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    depositSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     name: str = field(default=None, repr=False)
     earningGroupId: str = field(default=None, repr=False)
     earningCodeId: str = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     position: Position = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
     preadjustedValue: Value = field(default=None, repr=False)
     originTypeId: str = field(default=None, repr=False)
     reason: Reason = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     rule: Rule = field(default=None, repr=False)
     depositDate: date = field(default=None, repr=False)
     isHeld: bool = field(default=None, repr=False)
     releaseDate: date = field(default=None, repr=False)
     pipelineRun: Pipeline = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     comments: str = field(default=None, repr=False)
     pipelineRunDate: datetime = field(default=None, repr=False)
     isPrivate: bool = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
     genericAttribute3: str = field(default=None, repr=False)
     genericAttribute4: str = field(default=None, repr=False)
     genericAttribute5: str = field(default=None, repr=False)
     genericAttribute6: str = field(default=None, repr=False)
     genericAttribute7: str = field(default=None, repr=False)
@@ -577,191 +614,191 @@
     genericDate6: date = field(default=None, repr=False)
     genericBoolean1: bool = field(default=None, repr=False)
     genericBoolean2: bool = field(default=None, repr=False)
     genericBoolean3: bool = field(default=None, repr=False)
     genericBoolean4: bool = field(default=None, repr=False)
     genericBoolean5: bool = field(default=None, repr=False)
     genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class EarningCode(_Resource):
     _endpoint_name: ClassVar[str] = "earningCodes"
-    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    earningCodeId: str = field(default=None, metadata={"id": True}, repr=True)
+    dataTypeSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    earningCodeId: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class EarningGroup(_Resource):
     _endpoint_name: ClassVar[str] = "earningGroups"
-    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    earningGroupId: str = field(default=None, metadata={"id": True}, repr=True)
+    dataTypeSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    earningGroupId: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class EarningGroupCode(_Resource):
     _endpoint_name: ClassVar[str] = "earningGroupCodes"
-    earningGroupCodeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    earningGroupCode: str = field(default=None, metadata={"id": True}, repr=True)
+    earningGroupCodeSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    earningGroupCode: str = field(default=None, metadata=_meta(id=True), repr=True)
     earningCodeId: str = field(default=None, repr=False)
     earningGroupId: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class EventType(_Resource):
     _endpoint_name: ClassVar[str] = "eventTypes"
-    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    eventTypeId: str = field(default=None, metadata={"id": True}, repr=True)
+    dataTypeSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    eventTypeId: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class FixedValue(_Resource):
     _endpoint_name: ClassVar[str] = "fixedValues"
-    ruleElementOwnerSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    ruleElementOwnerSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
     calendar: Calendar = field(default=None, repr=False)
     periodType: PeriodType = field(default=None, repr=False)
     fixedValueType: FixedValueType = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
     unitTypeSeq: UnitType = field(default=None, repr=False)
     owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    ruleUsage: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     ruleElementSeq: str = field(default=None, repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     inputSignature: str = field(default=None, repr=False)
     returnType: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class FixedValueType(_Resource):
     _endpoint_name: ClassVar[str] = "fixedValueTypes"
-    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    fixedValueTypeId: str = field(default=None, metadata={"id": True}, repr=True)
+    dataTypeSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    fixedValueTypeId: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class FixedValueVariable(_Resource):
     _endpoint_name: ClassVar[str] = "fixedValueVariables"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    ruleElementSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     calendar: Calendar = field(default=None, repr=False)
     requiredPeriodType: PeriodType = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
     defaultElement: FixedValue = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     referenceClassType: str = field(default=None, repr=False)
     returnType: str = field(default=None, repr=False)
     owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    ruleUsage: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Formula(_Resource):
     _endpoint_name: ClassVar[str] = "formulas"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    ruleElementSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     calendar: Calendar = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
     returnType: str = field(default=None, repr=False)
     owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    ruleUsage: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class GenericClassifier(_Resource):
     _endpoint_name: ClassVar[str] = "genericClassifiers"
-    classifierSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    classifierId: str = field(default=None, metadata={"id": True}, repr=True)
+    classifierSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    classifierId: str = field(default=None, metadata=_meta(id=True), repr=True)
     name: str = field(default=None, repr=False)
     description: str = field(default=None, repr=False)
     selectorId: str = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
     genericAttribute3: str = field(default=None, repr=False)
     genericAttribute4: str = field(default=None, repr=False)
     genericAttribute5: str = field(default=None, repr=False)
     genericAttribute6: str = field(default=None, repr=False)
     genericAttribute7: str = field(default=None, repr=False)
@@ -788,67 +825,67 @@
     genericDate6: date = field(default=None, repr=False)
     genericBoolean1: bool = field(default=None, repr=False)
     genericBoolean2: bool = field(default=None, repr=False)
     genericBoolean3: bool = field(default=None, repr=False)
     genericBoolean4: bool = field(default=None, repr=False)
     genericBoolean5: bool = field(default=None, repr=False)
     genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class GenericClassifierType(_Resource):
     _endpoint_name: ClassVar[str] = "genericClassifierTypes"
     genericClassifierTypeSeq: int = field(
-        default=None, metadata={"seq": True}, repr=False
+        default=None, metadata=_meta(seq=True), repr=False
     )
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class GlobalFieldName(_Resource):
     _endpoint_name: ClassVar[str] = "globalFieldNames"
-    globalFieldNameSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    globalFieldNameSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     globalFieldNameDataTypeLength: int = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Group(_Resource):
     _endpoint_name: ClassVar[str] = "groups"
-    groupSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    groupSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     policy: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Incentive(_Resource):
     _endpoint_name: ClassVar[str] = "incentives"
-    incentiveSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    incentiveSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     name: str = field(default=None, repr=False)
     ruleElementOwnerSeq: str = field(default=None, repr=False)
     isActive: bool = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     quota: Quota = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     pipelineRunDate: datetime = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     releaseDate: datetime = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     attainment: str = field(default=None, repr=False)
     pipelineRun: Pipeline = field(default=None, repr=False)
     position: Position = field(default=None, repr=False)
     rule: Rule = field(default=None, repr=False)
     isPrivate: bool = field(default=None, repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
@@ -880,78 +917,74 @@
     genericDate6: date = field(default=None, repr=False)
     genericBoolean1: bool = field(default=None, repr=False)
     genericBoolean2: bool = field(default=None, repr=False)
     genericBoolean3: bool = field(default=None, repr=False)
     genericBoolean4: bool = field(default=None, repr=False)
     genericBoolean5: bool = field(default=None, repr=False)
     genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class LookUpTable(_Resource):
     _endpoint_name: ClassVar[str] = "relationalMDLTs"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    ruleElementSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    businessUnit: BusinessUnit = field(default=None, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    businessUnit: list[BusinessUnit] = field(default=None, repr=False)
     calendar: Calendar = field(default=None, repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     returnType: str = field(default=None, repr=False)
     returnUnitType: UnitType = field(default=None, repr=False)
     owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    ruleUsage: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     inputSignature: str = field(default=None, repr=False)
     treatNullAsZero: bool = field(default=None, repr=False)
     expressionTypeCounts: str = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    dimensions: LookUpTableDimension = field(
-        default=None, metadata={"expand": True}, repr=False
-    )
-    indices: LookUpTableIndice = field(
-        default=None, metadata={"expand": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    dimensions: list[LookUpTableDimension] = field(default=None, repr=False)
+    indices: list[LookUpTableIndice] = field(default=None, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class LookUpTableDimension(_Resource):
     _endpoint_name: ClassVar[str] = "lookupTableDimension"
-    dimensionSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    dimensionSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
     removeDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
     displayOrder: int = field(default=None, repr=False)
     dimensionType: int = field(default=None, repr=False)
     dimensionSlot: int = field(default=None, repr=False)
     dimensionUnitType: UnitType = field(default=None, repr=False)
     isRanged: bool = field(default=None, repr=False)
     includeStartInRange: bool = field(default=None, repr=False)
     includeEndInRange: bool = field(default=None, repr=False)
     flags: str = field(default=None, repr=False)
     MDLT: LookUpTable = field(default=None, repr=False)  # pylint: disable=invalid-name
     categoryTree: CategoryTree = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class LookUpTableIndice(_Resource):
     _endpoint_name: ClassVar[str] = "lookuptableIndice"
     ordinal: int = field(default=None, repr=False)
     displayOrder: int = field(default=None, repr=False)
@@ -967,60 +1000,60 @@
     category: str = field(default=None, repr=False)  # Implement Category
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
     createDate: datetime = field(default=None, repr=False)
     removeDate: datetime = field(default=None, repr=False)
     MDLT: LookUpTable = field(default=None, repr=False)  # pylint: disable=invalid-name
     dimensionSeq: LookUpTableDimension = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class LookUpTableVariable(_Resource):
     _endpoint_name: ClassVar[str] = "lookUpTableVariables"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    ruleElementSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     calendar: Calendar = field(default=None, repr=False)
     requiredPeriodType: PeriodType = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
     defaultElement: str = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     referenceClassType: str = field(default=None, repr=False)
     returnType: str = field(default=None, repr=False)
     owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    ruleUsage: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Measurement(_Resource):
     _endpoint_name: ClassVar[str] = "measurements"
-    measurementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    measurementSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     position: Position = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     rule: Rule = field(default=None, repr=False)
     pipelineRun: Pipeline = field(default=None, repr=False)
     pipelineRunDate: datetime = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
     numberOfCredits: Value = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     isPrivate: bool = field(default=None, repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
     genericAttribute3: str = field(default=None, repr=False)
     genericAttribute4: str = field(default=None, repr=False)
     genericAttribute5: str = field(default=None, repr=False)
     genericAttribute6: str = field(default=None, repr=False)
@@ -1048,32 +1081,32 @@
     genericDate6: date = field(default=None, repr=False)
     genericBoolean1: bool = field(default=None, repr=False)
     genericBoolean2: bool = field(default=None, repr=False)
     genericBoolean3: bool = field(default=None, repr=False)
     genericBoolean4: bool = field(default=None, repr=False)
     genericBoolean5: bool = field(default=None, repr=False)
     genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class PrimaryMeasurement(_Resource):
     _endpoint_name: ClassVar[str] = "primaryMeasurements"
-    measurementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    measurementSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     position: Position = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     rule: Rule = field(default=None, repr=False)
     pipelineRun: Pipeline = field(default=None, repr=False)
     pipelineRunDate: datetime = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
     numberOfCredits: Value = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     isPrivate: bool = field(default=None, repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
     genericAttribute3: str = field(default=None, repr=False)
     genericAttribute4: str = field(default=None, repr=False)
     genericAttribute5: str = field(default=None, repr=False)
     genericAttribute6: str = field(default=None, repr=False)
@@ -1101,32 +1134,32 @@
     genericDate6: date = field(default=None, repr=False)
     genericBoolean1: bool = field(default=None, repr=False)
     genericBoolean2: bool = field(default=None, repr=False)
     genericBoolean3: bool = field(default=None, repr=False)
     genericBoolean4: bool = field(default=None, repr=False)
     genericBoolean5: bool = field(default=None, repr=False)
     genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class SecondaryMeasurement(_Resource):
     _endpoint_name: ClassVar[str] = "secondaryMeasurements"
-    measurementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    measurementSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     position: Position = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     rule: Rule = field(default=None, repr=False)
     pipelineRun: Pipeline = field(default=None, repr=False)
     pipelineRunDate: datetime = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
     numberOfCredits: Value = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     isPrivate: bool = field(default=None, repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
     genericAttribute3: str = field(default=None, repr=False)
     genericAttribute4: str = field(default=None, repr=False)
     genericAttribute5: str = field(default=None, repr=False)
     genericAttribute6: str = field(default=None, repr=False)
@@ -1154,55 +1187,55 @@
     genericDate6: date = field(default=None, repr=False)
     genericBoolean1: bool = field(default=None, repr=False)
     genericBoolean2: bool = field(default=None, repr=False)
     genericBoolean3: bool = field(default=None, repr=False)
     genericBoolean4: bool = field(default=None, repr=False)
     genericBoolean5: bool = field(default=None, repr=False)
     genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Message(_Resource):
     _endpoint_name: ClassVar[str] = "messages"
-    messageSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    messageKey: str = field(default=None, metadata={"id": True}, repr=True)
+    messageSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    messageKey: str = field(default=None, metadata=_meta(id=True), repr=True)
     messageTimeStamp: datetime = field(default=None, repr=False)
     argumentCount: int = field(default=None, repr=False)
     subCategory: str = field(default=None, repr=False)
     messageLog: MessageLog = field(default=None, repr=False)
     module: str = field(default=None, repr=False)
     rule: Rule = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     messageType: str = field(default=None, repr=False)
     runPeriod: Period = field(default=None, repr=False)
     objectSeq: str = field(default=None, repr=False)
     salesTransaction: SalesTransaction = field(default=None, repr=False)
     position: Position = field(default=None, repr=False)
     category: str = field(default=None, repr=False)
     credit: Credit = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class MessageLog(_Resource):
     _endpoint_name: ClassVar[str] = "messageLogs"
-    messageLogSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    messageLogSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     sourceSeq: str = field(default=None, repr=False)
     componentName: str = field(default=None, repr=False)
     logDate: datetime = field(default=None, repr=False)
     logName: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Model(_Resource):
     _endpoint_name: ClassVar[str] = "models"
-    modelSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    modelName: str = field(default=None, metadata={"id": True}, repr=True)
+    modelSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    modelName: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     status: str = field(default=None, repr=False)
     calendar: Calendar = field(default=None, repr=False)
     budgetType: str = field(default=None, repr=False)
     budgetValue: Value = field(default=None, repr=False)
     useSourcePeriodAsInput: str = field(default=None, repr=False)
     sourceAdjustment: Value = field(default=None, repr=False)
@@ -1210,22 +1243,22 @@
     sourceEndPeriod: Period = field(default=None, repr=False)
     modelStartPeriod: Period = field(default=None, repr=False)
     modelEndPeriod: Period = field(default=None, repr=False)
     modificationDate: datetime = field(default=None, repr=False)
     budgetPercentValue: Value = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     useNewTransactionAsInput: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Participant(_Resource):
     _endpoint_name: ClassVar[str] = "participants"
-    payeeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    payeeId: str = field(default=None, metadata={"id": True}, repr=True)
+    payeeSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    payeeId: str = field(default=None, metadata=_meta(id=True), repr=True)
     firstName: str = field(default=None, repr=False)
     lastName: str = field(default=None, repr=False)
     middleName: str = field(default=None, repr=False)
     prefix: str = field(default=None, repr=False)
     suffix: str = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
@@ -1233,20 +1266,20 @@
     terminationDate: date = field(default=None, repr=False)
     salary: Value = field(default=None, repr=False)
     userId: str = field(default=None, repr=False)
     participantEmail: str = field(default=None, repr=False)
     preferredLanguage: str = field(default=None, repr=False)
     eventCalendar: str = field(default=None, repr=False)
     taxId: str = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
     genericAttribute3: str = field(default=None, repr=False)
     genericAttribute4: str = field(default=None, repr=False)
     genericAttribute5: str = field(default=None, repr=False)
     genericAttribute6: str = field(default=None, repr=False)
     genericAttribute7: str = field(default=None, repr=False)
@@ -1273,21 +1306,21 @@
     genericDate6: date = field(default=None, repr=False)
     genericBoolean1: bool = field(default=None, repr=False)
     genericBoolean2: bool = field(default=None, repr=False)
     genericBoolean3: bool = field(default=None, repr=False)
     genericBoolean4: bool = field(default=None, repr=False)
     genericBoolean5: bool = field(default=None, repr=False)
     genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Payment(_Resource):
     _endpoint_name: ClassVar[str] = "payments"
-    paymentSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    paymentSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     position: Position = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     earningGroupId: str = field(default=None, repr=False)
     earningCodeId: str = field(default=None, repr=False)
     trialPipelineRun: Pipeline = field(default=None, repr=False)
@@ -1326,173 +1359,171 @@
     genericDate6: date = field(default=None, repr=False)
     genericBoolean1: bool = field(default=None, repr=False)
     genericBoolean2: bool = field(default=None, repr=False)
     genericBoolean3: bool = field(default=None, repr=False)
     genericBoolean4: bool = field(default=None, repr=False)
     genericBoolean5: bool = field(default=None, repr=False)
     genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class PaymentMapping(_Resource):
     _endpoint_name: ClassVar[str] = "paymentMappings"
-    paymentMappingSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    paymentMappingSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     sourceTableName: str = field(default=None, repr=False)
     sourceAttribute: str = field(default=None, repr=False)
     paymentAttribute: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class PaymentSummary(_Resource):
     _endpoint_name: ClassVar[str] = "paymentSummarys"
-    paymentSummarySeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    paymentSummarySeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     position: Position = field(default=None, repr=False)
     participant: Participant = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     earningGroupId: str = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     pipelineRun: Pipeline = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     pipelineRunDate: datetime = field(default=None, repr=False)
     appliedDeposit: Value = field(default=None, repr=False)
     priorBalance: Value = field(default=None, repr=False)
     balance: Value = field(default=None, repr=False)
     payment: Value = field(default=None, repr=False)
     Deposit: Value = field(default=None, repr=False)  # pylint: disable=invalid-name
     outstandingBalance: Value = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Period(_Resource):
     _endpoint_name: ClassVar[str] = "periods"
-    periodSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    periodSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     shortName: str = field(default=None, repr=False)
     description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     calendar: Calendar = field(default=None, repr=False)
-    periodType: PeriodType = field(default=None, repr=False)
+    periodType: PeriodType = field(default=None, repr=True)
     parent: Period = field(default=None, repr=False)
     startDate: date = field(default=None, repr=False)
     endDate: date = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class PeriodType(_Resource):
     _endpoint_name: ClassVar[str] = "periodTypes"
-    periodTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    periodTypeSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     level: int = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Pipeline(_Resource):
     _endpoint_name: ClassVar[str] = "pipelines"
-    pipelineRunSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    pipelineRunSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     batchName: str = field(default=None, repr=False)
     command: str = field(default=None, repr=False)
     dateSubmitted: datetime = field(default=None, repr=False)
-    description: str = field(default=None, repr=False)
+    description: str = field(default=None, repr=True)
     endDateScheduled: datetime = field(default=None, repr=False)
     groupName: str = field(default=None, repr=False)
     isolationLevel: str = field(default=None, repr=False)
     message: str = field(default=None, repr=False)
     modelRun: str = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     numErrors: int = field(default=None, repr=False)
     numWarnings: int = field(default=None, repr=False)
     period: str = field(default=None, repr=False)
     priority: str = field(default=None, repr=False)
     processingUnit: str = field(default=None, repr=False)
     productVersion: str = field(default=None, repr=False)
     removeDate: datetime = field(default=None, repr=False)
     reportTypeName: str = field(default=None, repr=False)
     runMode: str = field(default=None, repr=False)
     runParameters: str = field(default=None, repr=False)
     runProgress: str = field(default=None, repr=False)
     scheduleDay: str = field(default=None, repr=False)
     scheduleFrequency: str = field(default=None, repr=False)
     schemaVersion: str = field(default=None, repr=False)
-    stageTables: list = field(default=None, metadata={"type": str}, repr=False)
+    stageTables: list[str] = field(default=None, repr=False)
     stageType: str = field(default=None, repr=False)
     startDateScheduled: datetime = field(default=None, repr=False)
-    startTime: datetime = field(default=None, repr=False)
-    state: str = field(default=None, repr=False)
+    startTime: datetime = field(default=None, repr=True)
+    state: str = field(default=None, repr=True)
     status: str = field(default=None, repr=False)
     stopTime: datetime = field(default=None, repr=False)
     storedProcVersion: str = field(default=None, repr=False)
     targetDatabase: str = field(default=None, repr=False)
     traceLevel: str = field(default=None, repr=False)
     userId: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Plan(_Resource):
     _endpoint_name: ClassVar[str] = "plans"
-    ruleElementOwnerSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    ruleElementOwnerSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     calendar: Calendar = field(default=None, repr=False)
-    variableAssignments: VariableAssignment = field(
-        default=None, metadata={"expand": True}, repr=False
-    )
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    variableAssignments: VariableAssignment = field(default=None, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Position(_Resource):
     _endpoint_name: ClassVar[str] = "positions"
-    ruleElementOwnerSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    ruleElementOwnerSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=date(2200, 1, 1), repr=True)
     creditStartDate: date = field(default=None, repr=False)
     creditEndDate: date = field(default=None, repr=False)
     processingStartDate: date = field(default=None, repr=False)
     processingEndDate: date = field(default=None, repr=False)
     targetCompensation: Value = field(default=None, repr=False)
     businessUnits: list[BusinessUnit] = field(default_factory=list, repr=False)
     manager: Position = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     title: Title = field(default=None, repr=False)
     positionGroup: PositionGroup = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     plan: Plan = field(default=None, repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
@@ -1525,94 +1556,94 @@
     genericBoolean1: bool = field(default=None, repr=False)
     genericBoolean2: bool = field(default=None, repr=False)
     genericBoolean3: bool = field(default=None, repr=False)
     genericBoolean4: bool = field(default=None, repr=False)
     genericBoolean5: bool = field(default=None, repr=False)
     genericBoolean6: bool = field(default=None, repr=False)
     variableAssignments: list[VariableAssignment] = field(
-        default_factory=list, metadata={"expand": True}, repr=False
+        default_factory=list, repr=False
     )
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class PositionGroup(_Resource):
     _endpoint_name: ClassVar[str] = "positionGroups"
-    positionGroupSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    businessUnits: list = field(default=None, metadata={"type": str}, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    positionGroupSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class PositionRelation(_Resource):
     _endpoint_name: ClassVar[str] = "positionRelations"
-    positionRelationSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    positionRelationSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     parentPosition: Position = field(default=None, repr=False)
     positionRelationType: PositionRelationType = field(default=None, repr=False)
     childPosition: Position = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class PositionRelationType(_Resource):
     _endpoint_name: ClassVar[str] = "positionRelationTypes"
-    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    dataTypeSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
     relations: PositionRelation = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class ProcessingUnit(_Resource):
     _endpoint_name: ClassVar[str] = "processingUnits"
-    processingUnitSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    processingUnitSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Product(_Resource):
     _endpoint_name: ClassVar[str] = "products"
-    classifierSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    classifierId: str = field(default=None, metadata={"id": True}, repr=True)
+    classifierSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    classifierId: str = field(default=None, metadata=_meta(id=True), repr=True)
     name: str = field(default=None, repr=False)
     description: str = field(default=None, repr=False)
     selectorId: str = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
     cost: Value = field(default=None, repr=False)
     price: Value = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
     genericAttribute3: str = field(default=None, repr=False)
     genericAttribute4: str = field(default=None, repr=False)
     genericAttribute5: str = field(default=None, repr=False)
     genericAttribute6: str = field(default=None, repr=False)
     genericAttribute7: str = field(default=None, repr=False)
@@ -1639,149 +1670,149 @@
     genericDate6: date = field(default=None, repr=False)
     genericBoolean1: bool = field(default=None, repr=False)
     genericBoolean2: bool = field(default=None, repr=False)
     genericBoolean3: bool = field(default=None, repr=False)
     genericBoolean4: bool = field(default=None, repr=False)
     genericBoolean5: bool = field(default=None, repr=False)
     genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Quota(_Resource):
     _endpoint_name: ClassVar[str] = "quotas"
-    quotaSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    quotaSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     name: str = field(default=None, repr=False)
     description: str = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    businessUnit: BusinessUnit = field(default=None, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    businessUnit: list[BusinessUnit] = field(default=None, repr=False)
     calendar: Calendar = field(default=None, repr=False)
     unitType: UnitType = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class RateTable(_Resource):
     _endpoint_name: ClassVar[str] = "rateTables"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    ruleElementSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    businessUnit: BusinessUnit = field(default=None, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    businessUnit: list[BusinessUnit] = field(default=None, repr=False)
     calendar: Calendar = field(default=None, repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     returnType: str = field(default=None, repr=False)
     owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    ruleUsage: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class RateTableVariable(_Resource):
     _endpoint_name: ClassVar[str] = "rateTableVariables"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    ruleElementSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
     requiredPeriodType: PeriodType = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     calendar: Calendar = field(default=None, repr=False)
     unitType: UnitType = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
     defaultElement: str = field(default=None, repr=False)
     referenceClassType: str = field(default=None, repr=False)
     returnType: str = field(default=None, repr=False)
     owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    ruleUsage: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Reason(_Resource):
     _endpoint_name: ClassVar[str] = "reasons"
-    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    reasonId: str = field(default=None, metadata={"id": True}, repr=True)
+    dataTypeSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    reasonId: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Rule(_Resource):
     _endpoint_name: ClassVar[str] = "rules"
-    ruleSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    ruleSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    businessUnit: BusinessUnit = field(default=None, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    businessUnit: list[BusinessUnit] = field(default=None, repr=False)
     calendar: Calendar = field(default=None, repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
     type: RuleType = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class RuleType(_Resource):
     _endpoint_name: ClassVar[str] = "ruleType"
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     id: int = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class SalesOrder(_Resource):
     _endpoint_name: ClassVar[str] = "salesOrders"
-    salesOrderSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    orderId: str = field(default=None, metadata={"id": True}, repr=True)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    salesOrderSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    orderId: str = field(default=None, metadata=_meta(id=True), repr=True)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     pipelineRun: Pipeline = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
     genericAttribute3: str = field(default=None, repr=False)
     genericAttribute4: str = field(default=None, repr=False)
     genericAttribute5: str = field(default=None, repr=False)
     genericAttribute6: str = field(default=None, repr=False)
     genericAttribute7: str = field(default=None, repr=False)
@@ -1808,46 +1839,46 @@
     genericDate6: date = field(default=None, repr=False)
     genericBoolean1: bool = field(default=None, repr=False)
     genericBoolean2: bool = field(default=None, repr=False)
     genericBoolean3: bool = field(default=None, repr=False)
     genericBoolean4: bool = field(default=None, repr=False)
     genericBoolean5: bool = field(default=None, repr=False)
     genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class SalesTransaction(_Resource):
     _endpoint_name: ClassVar[str] = "salesTransactions"
-    salesTransactionSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    salesTransactionSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     salesOrder: SalesOrder = field(default=None, repr=False)
     lineNumber: Value = field(default=None, repr=False)
     subLineNumber: Value = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
     preadjustedValue: Value = field(default=None, repr=False)
     isRunnable: bool = field(default=None, repr=False)
     compensationDate: date = field(default=None, repr=False)
     eventType: EventType = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     modificationDate: datetime = field(default=None, repr=False)
     reason: Reason = field(default=None, repr=False)
     channel: str = field(default=None, repr=False)
     poNumber: str = field(default=None, repr=False)
     dataSource: str = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     shipToAddress: Address = field(default=None, repr=False)
     otherToAddress: Address = field(default=None, repr=False)
     billToAddress: Address = field(default=None, repr=False)
-    transactionAssignments: TransactionAssignment = field(
-        default=None, metadata={"expand": True}, repr=False
+    transactionAssignments: list[TransactionAssignment] = field(
+        default=None, repr=False
     )
     discountType: str = field(default=None, repr=False)
     productName: str = field(default=None, repr=False)
     productDescription: str = field(default=None, repr=False)
     paymentTerms: str = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     unitValue: Value = field(default=None, repr=False)
@@ -1907,103 +1938,104 @@
     genericDate6: date = field(default=None, repr=False)
     genericBoolean1: bool = field(default=None, repr=False)
     genericBoolean2: bool = field(default=None, repr=False)
     genericBoolean3: bool = field(default=None, repr=False)
     genericBoolean4: bool = field(default=None, repr=False)
     genericBoolean5: bool = field(default=None, repr=False)
     genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    isPurged: bool = field(default=None, repr=False)
 
 
 @dataclass
 class StatusCode(_Resource):
     _endpoint_name: ClassVar[str] = "statusCodes"
-    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    dataTypeSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
     type: str = field(default=None, repr=False)
     isActive: bool = field(default=None, repr=False)
     status: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Territory(_Resource):
     _endpoint_name: ClassVar[str] = "territories"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    ruleElementSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     calendar: Calendar = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
     definition: str = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     returnType: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    ruleUsage: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     owningElement: str = field(default=None, repr=False)
     inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class TerritoryVariable(_Resource):
     _endpoint_name: ClassVar[str] = "territoryVariables"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    ruleElementSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     calendar: Calendar = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
     defaultElement: str = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     referenceClassType: str = field(default=None, repr=False)
     returnType: str = field(default=None, repr=False)
     owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    ruleUsage: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     requiredPeriodType: PeriodType = field(default=None, repr=False)
     inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Title(_Resource):
     _endpoint_name: ClassVar[str] = "titles"
-    ruleElementOwnerSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    ruleElementOwnerSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: list = field(default=None, metadata={"type": str}, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     plan: str = field(default=None, repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
     genericAttribute3: str = field(default=None, repr=False)
     genericAttribute4: str = field(default=None, repr=False)
     genericAttribute5: str = field(default=None, repr=False)
     genericAttribute6: str = field(default=None, repr=False)
     genericAttribute7: str = field(default=None, repr=False)
@@ -2030,116 +2062,114 @@
     genericDate6: date = field(default=None, repr=False)
     genericBoolean1: bool = field(default=None, repr=False)
     genericBoolean2: bool = field(default=None, repr=False)
     genericBoolean3: bool = field(default=None, repr=False)
     genericBoolean4: bool = field(default=None, repr=False)
     genericBoolean5: bool = field(default=None, repr=False)
     genericBoolean6: bool = field(default=None, repr=False)
-    variableAssignments: VariableAssignment = field(
-        default=None, metadata={"expand": True}, repr=False
-    )
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    variableAssignments: list[VariableAssignment] = field(default=None, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class TransactionAssignment(_Resource):
     _endpoint_name: ClassVar[str] = "transactionAssignment"
     titleName: str = field(default=None, repr=False)
     payeeId: str = field(default=None, repr=False)
     positionName: str = field(default=None, repr=False)
     salesOrder: SalesOrder = field(default=None, repr=False)
     salesTransactionSeq: int = field(default=None, repr=False)
     setNumber: int = field(default=None, repr=False)
     compensationDate: date = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class UnitType(_Resource):
     _endpoint_name: ClassVar[str] = "unitTypes"
-    unitTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    unitTypeSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     symbol: str = field(default=None, repr=False)
     currencyLocale: str = field(default=None, repr=False)
     formatting: str = field(default=None, repr=False)
     positionOfSymbol: int = field(default=None, repr=False)
     reportingScale: str = field(default=None, repr=False)
     scale: int = field(default=None, repr=False)
     valueClass: dict = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class User(_Resource):
     _endpoint_name: ClassVar[str] = "users"
-    userSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    id: str = field(default=None, metadata={"id": True}, repr=True)
+    userSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    id: str = field(default=None, metadata=_meta(id=True), repr=True)
     userName: str = field(default=None, repr=False)
     description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    readOnlyBusinessUnitList: BusinessUnit = field(default=None, repr=False)
-    fullAccessBusinessUnitList: BusinessUnit = field(default=None, repr=False)
-    groups: Group = field(default=None, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    readOnlyBusinessUnitList: list[BusinessUnit] = field(default=None, repr=False)
+    fullAccessBusinessUnitList: list[BusinessUnit] = field(default=None, repr=False)
+    groups: list[Group] = field(default=None, repr=False)
     email: str = field(default=None, repr=False)
     preferredLanguage: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Value(_Resource):
     _endpoint_name: ClassVar[str] = "value"
     value: float = field(default=None, repr=False)
     unitType: UnitType = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class Variable(_Resource):
     _endpoint_name: ClassVar[str] = "variables"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
+    ruleElementSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
+    name: str = field(default=None, metadata=_meta(id=True), repr=True)
     description: str = field(default=None, repr=False)
     calendar: Calendar = field(default=None, repr=False)
     requiredPeriodType: PeriodType = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: list = field(default=None, metadata={"type": str}, repr=False)
+    businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     plan: str = field(default=None, repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     notAllowUpdate: bool = field(default=None, repr=False)
     defaultElement: str = field(default=None, repr=False)
     referenceClassType: str = field(default=None, repr=False)
     returnType: str = field(default=None, repr=False)
     owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    ruleUsage: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
 class VariableAssignment(_Resource):
     _endpoint_name: ClassVar[str] = "variableAssignment"
     owner: str = field(default=None, repr=False)
     variable: str = field(default=None, repr=False)
     assignment: str = field(default=None, repr=False)
     effectiveStartDate: date = field(default=None, repr=True)
     effectiveEndDate: date = field(default=None, repr=False)
     createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
+        default=None, metadata=_meta(json_ignore=True), repr=False
     )
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
```

### Comparing `python-sapcommissions-1.0.2/tests/test_base.py` & `python-sapcommissions-1.1.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.0.2/tests/test_endpoints.py` & `python-sapcommissions-1.1.0/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.0.2/tests/test_resources.py` & `python-sapcommissions-1.1.0/tests/test_resources.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,138 +1,182 @@
+"""Tests for the sapcommissions.resources module."""
+from __future__ import annotations
+
 import unittest
 from dataclasses import dataclass, field
 from datetime import date, datetime
-from typing import ClassVar, List
+from typing import ClassVar
+
+from sapcommissions.resources import _deserialize, _Resource, _serialize
 
-from sapcommissions.resources import _decode, _encode, _Resource
+# pylint: skip-file
 
 
 @dataclass
 class DummyResource(_Resource):
     _endpoint_name: ClassVar[str] = "test"
-    id: str = field(metadata={"id": True})
-    name: str = field(default=None)
-    items: List[str] = field(default_factory=list)
-    expands: bool = field(default=None, metadata={"expand": True})
+    id: str = field(metadata={"seq": True})
+    name: str = field(default=None, metadata={"id": True})
+    items: list[str] = field(default_factory=list)
+    parent: DummyResource = field(default=None)
 
 
 class TestResourceMethods(unittest.TestCase):
     def setUp(self):
         self.resource_dict = {
             "id": "123",
             "name": "Test Resource",
             "items": ["item1", "item2"],
-            "expands": False,
         }
-        self.resource: DummyResource = DummyResource.from_dict(self.resource_dict)
+        self.resource: DummyResource = DummyResource(
+            id="123",
+            name="Test Resource",
+            items=["item1", "item2"],
+        )
 
     def test_name_property(self):
         self.assertEqual(DummyResource._name, "test")
 
     def test_seq_attr_property(self):
-        self.assertIsNone(DummyResource._seqAttr)
+        self.assertEqual(DummyResource._seqAttr, "id")
 
     def test_seq_property(self):
-        self.assertIsNone(self.resource._seq)
+        self.assertEqual(self.resource._seq, "123")
 
     def test_id_attr_property(self):
-        self.assertEqual(DummyResource._idAttr, "id")
+        self.assertEqual(DummyResource._idAttr, "name")
 
     def test_id_property(self):
-        self.assertEqual(self.resource._id, "123")
+        self.assertEqual(self.resource._id, "Test Resource")
 
     def test_expands_property(self):
-        self.assertEqual(DummyResource._expands, ("expands",))
+        self.assertEqual(DummyResource._expands, ("items", "parent"))
+
+    def test_to_dict_with_seq(self):
+        self.assertEqual(self.resource.to_dict(False), self.resource_dict)
+
+    def test_to_dict_without_seq(self):
+        resource_dict = self.resource_dict.copy()
+        del resource_dict["id"]
+        self.assertEqual(self.resource.to_dict(), resource_dict)
 
-    def test_from_dict_method(self):
-        self.assertIsInstance(self.resource, DummyResource)
+    def test_from_dict_with_valid_dict(self):
+        self.assertEqual(self.resource, DummyResource.from_dict(self.resource_dict))
         self.assertEqual(self.resource.id, "123")
         self.assertEqual(self.resource.name, "Test Resource")
         self.assertEqual(self.resource.items, ["item1", "item2"])
-        self.assertEqual(self.resource.expands, False)
+        self.assertEqual(self.resource.parent, None)
 
-    def test_to_dict_method(self):
-        expected_dict = {
-            "id": "123",
-            "name": "Test Resource",
-            "items": ["item1", "item2"],
-            "expands": False,
+    def test_from_dict_with_invalid_dict(self):
+        resource_dict = {
+            "spam": "eggs",
+            "ham": "cheese",
+            "foo": "bar",
         }
-        self.assertEqual(self.resource.to_dict(), expected_dict)
+        with self.assertRaises(TypeError):
+            DummyResource.from_dict(resource_dict)
+
+    def test_from_dict_with_invalid_field(self):
+        resource_dict = self.resource_dict.copy()
+        resource_dict["invalidField"] = "spam"
+        resource: DummyResource = DummyResource.from_dict(resource_dict)
+
+        self.assertEqual(resource, self.resource)
+
+    def test_from_dict_with_valid_reference(self):
+        resource_dict = {
+            "objectType": "DummyResource",
+            "key": "spam",
+            "displayName": "eggs",
+        }
+        resource: DummyResource = DummyResource.from_dict(resource_dict)
+        self.assertIsInstance(resource, DummyResource)
+        self.assertEqual(resource.id, "spam")
+        self.assertEqual(resource.name, "eggs")
+
+    def test_from_dict_with_invalid_reference(self):
+        resource_dict = {
+            "objectType": "Sausages",
+            "key": "spam",
+            "displayName": "eggs",
+        }
+
+        with self.assertRaises(TypeError):
+            DummyResource.from_dict(resource_dict)
 
 
 class TestEncodeDecode(unittest.TestCase):
     def test_decode_datetime(self):
         dt_str = "2000-01-02T03:04:05.000-06:00"
-        decoded_dt = _decode(dt_str, datetime)
+        decoded_dt = _deserialize(dt_str, datetime)
         self.assertEqual(decoded_dt, datetime.fromisoformat(dt_str))
 
     def test_encode_datetime(self):
         dt = datetime(2000, 1, 2, 3, 4, 5)
-        encoded_dt = _encode(dt, datetime)
+        encoded_dt = _serialize(dt, datetime)
         self.assertEqual(encoded_dt, "2000-01-02T03:04:05")
 
     def test_decode_date(self):
         date_str = "2000-01-02T03:04:05.000-06:00"
-        decoded_date = _decode(date_str, date)
+        decoded_date = _deserialize(date_str, date)
         self.assertEqual(decoded_date, datetime.fromisoformat(date_str).date())
 
     def test_encode_date(self):
         dt = date(2000, 1, 2)
-        encoded_dt = _encode(dt, date)
+        encoded_dt = _serialize(dt, date)
         self.assertEqual(encoded_dt, "2000-01-02")
 
     def test_decode_none(self):
-        decoded_none = _decode(None, str)
+        decoded_none = _deserialize(None, str)
         self.assertIs(decoded_none, None)
 
     def test_encode_none(self):
-        encoded_none = _encode(None, str)
+        encoded_none = _serialize(None, str)
         self.assertIs(encoded_none, None)
 
     def test_decode_string(self):
         test_str = "SPAM"
-        decoded_str = _decode(test_str, str)
+        decoded_str = _deserialize(test_str, str)
         self.assertEqual(decoded_str, "SPAM")
 
     def test_encode_string(self):
         test_str = "SPAM"
-        encoded_str = _encode(test_str, str)
+        encoded_str = _serialize(test_str, str)
         self.assertEqual(encoded_str, "SPAM")
 
     def test_decode_int(self):
         test_int = 1
-        decoded_int = _decode(test_int, int)
+        decoded_int = _deserialize(test_int, int)
         self.assertEqual(decoded_int, 1)
 
     def test_decode_str_int(self):
         test_int_str = "1"
-        decoded_int_str = _decode(test_int_str, int)
+        decoded_int_str = _deserialize(test_int_str, int)
         self.assertEqual(decoded_int_str, 1)
 
     def test_encode_int(self):
         test_int = 1
-        encoded_int = _encode(test_int, int)
+        encoded_int = _serialize(test_int, int)
         self.assertEqual(encoded_int, 1)
 
     def test_decode_list_str(self):
         test_list = ["SPAM", "EGGS"]
-        decoded_list = _decode(test_list, list[str])
+        decoded_list = _deserialize(test_list, list[str])
         self.assertListEqual(decoded_list, test_list)
 
     def test_decode_list_error(self):
         test_list = ["SPAM", "EGGS"]
         with self.assertRaises(TypeError):
-            _decode(test_list, list[str, int])
+            _deserialize(test_list, list[str, int])
         with self.assertRaises(TypeError):
-            _decode(test_list, list)
+            _deserialize(test_list, list)
         with self.assertRaises(TypeError):
-            _decode(test_list, str)
+            _deserialize(test_list, str)
 
     def test_decode_unions(self):
         test_value = 1
         with self.assertRaises(NotImplementedError):
-            _decode(test_value, int | dict)
+            _deserialize(test_value, int | dict)
 
 
 if __name__ == "__main__":
     unittest.main()
```

