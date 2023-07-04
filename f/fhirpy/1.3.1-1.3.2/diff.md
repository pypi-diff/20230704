# Comparing `tmp/fhirpy-1.3.1.tar.gz` & `tmp/fhirpy-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhirpy-1.3.1.tar", last modified: Mon Jan  9 09:23:22 2023, max compression
+gzip compressed data, was "fhirpy-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fhirpy-1.3.1.tar` & `fhirpy-1.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1087 2023-01-09 09:23:11.715129 fhirpy-1.3.1/LICENSE.md
--rw-r--r--   0        0        0    18503 2023-01-09 09:23:11.715129 fhirpy-1.3.1/README.md
--rw-r--r--   0        0        0      232 2023-01-09 09:23:11.719129 fhirpy-1.3.1/fhirpy/__init__.py
--rw-r--r--   0        0        0      260 2023-01-09 09:23:11.719129 fhirpy-1.3.1/fhirpy/base/__init__.py
--rw-r--r--   0        0        0     1872 2023-01-09 09:23:11.719129 fhirpy-1.3.1/fhirpy/base/exceptions.py
--rw-r--r--   0        0        0    15821 2023-01-09 09:23:11.719129 fhirpy-1.3.1/fhirpy/base/lib.py
--rw-r--r--   0        0        0     5958 2023-01-09 09:23:11.719129 fhirpy-1.3.1/fhirpy/base/resource.py
--rw-r--r--   0        0        0     9545 2023-01-09 09:23:11.719129 fhirpy-1.3.1/fhirpy/base/searchset.py
--rw-r--r--   0        0        0     5521 2023-01-09 09:23:11.719129 fhirpy-1.3.1/fhirpy/base/utils.py
--rw-r--r--   0        0        0     2591 2023-01-09 09:23:11.719129 fhirpy-1.3.1/fhirpy/lib.py
--rw-r--r--   0        0        0     1656 2023-01-09 09:23:11.719129 fhirpy-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    19779 1970-01-01 00:00:00.000000 fhirpy-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-07-04 11:18:27.121445 fhirpy-1.3.2/LICENSE.md
+-rw-r--r--   0        0        0    19460 2023-07-04 11:18:27.125445 fhirpy-1.3.2/README.md
+-rw-r--r--   0        0        0      232 2023-07-04 11:18:27.129445 fhirpy-1.3.2/fhirpy/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-04 11:18:27.129445 fhirpy-1.3.2/fhirpy/base/__init__.py
+-rw-r--r--   0        0        0     1872 2023-07-04 11:18:27.129445 fhirpy-1.3.2/fhirpy/base/exceptions.py
+-rw-r--r--   0        0        0    15826 2023-07-04 11:18:27.129445 fhirpy-1.3.2/fhirpy/base/lib.py
+-rw-r--r--   0        0        0     5958 2023-07-04 11:18:27.129445 fhirpy-1.3.2/fhirpy/base/resource.py
+-rw-r--r--   0        0        0     9545 2023-07-04 11:18:27.129445 fhirpy-1.3.2/fhirpy/base/searchset.py
+-rw-r--r--   0        0        0     6127 2023-07-04 11:18:27.129445 fhirpy-1.3.2/fhirpy/base/utils.py
+-rw-r--r--   0        0        0     2591 2023-07-04 11:18:27.129445 fhirpy-1.3.2/fhirpy/lib.py
+-rw-r--r--   0        0        0     1656 2023-07-04 11:18:27.129445 fhirpy-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0    20736 1970-01-01 00:00:00.000000 fhirpy-1.3.2/PKG-INFO
```

### Comparing `fhirpy-1.3.1/LICENSE.md` & `fhirpy-1.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fhirpy-1.3.1/README.md` & `fhirpy-1.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-[![Build Status](https://travis-ci.com/beda-software/fhir-py.svg?branch=master)](https://travis-ci.com/beda-software/fhir-py)
+[![build status](https://github.com/beda-software/fhir-py/actions/workflows/build.yaml/badge.svg)](https://github.com/beda-software/fhir-py/actions/workflows/build.yaml)
 [![codecov](https://codecov.io/gh/beda-software/fhir-py/branch/master/graph/badge.svg)](https://codecov.io/gh/beda-software/fhir-py)
-[![pypi](https://img.shields.io/pypi/v/fhirpy.svg)](https://pypi.python.org/pypi/fhirpy)
-[![Supported Python version](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
+[![pypi](https://img.shields.io/pypi/v/fhirpy.svg)](https://pypi.org/project/fhirpy)
+[![Supported Python version](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 
 # fhir-py
 async/sync FHIR client for python3.
 This package provides an API for CRUD operations over FHIR resources
 
 ```pip install fhirpy```
 
@@ -41,14 +41,15 @@
     - [Wild card (any search parameter of type=reference be included)](#wild-card-any-search-parameter-of-typereference-be-included)
   - [Revinclude](#revinclude)
     - [Wild card (any search parameter of type=reference be included)](#wild-card-any-search-parameter-of-typereference-be-included-1)
 - [Resource and helper methods](#resource-and-helper-methods)
   - [Validate resource using operation $validate](#validate-resource-using-operation-validate)
   - [Accessing resource attributes](#accessing-resource-attributes)
   - [get_by_path(path, default=None)](#get_by_pathpath-defaultnone)
+  - [set_by_path(obj, path, value)](#set_by_pathpath)
   - [serialize()](#serialize)
 - [Reference](#reference-1)
   - [Main class structure](#main-class-structure)
   - [Acync client (based on _aiohttp_) – AsyncFHIRClient](#acync-client-based-on-_aiohttp_--asyncfhirclient)
     - [AsyncFHIRResource](#asyncfhirresource)
     - [AsyncFHIRReference](#asyncfhirreference)
     - [AsyncFHIRSearchSet](#asyncfhirsearchset)
@@ -361,14 +362,26 @@
 # Work with the resource as a dictionary
 patient_family = patient['name'][0]['family']
 
 # Or access value by an attribute
 patient_given_name = patient.name[0].given[0]
 ```
 
+## Static type checking with [mypy](https://github.com/python/mypy) and [fhir-py-types](https://github.com/beda-software/fhir-py-types)
+```Python
+from fhir_py_types.generated.resources import Patient
+
+patient: Patient = await client.resources('Patient').first()
+
+# Works only with dictionary-like resource access
+patient_family = patient['name'][0]['family1']
+# 'TypedDict "HumanName" has no key "family1" note: Did you mean "family"?'
+```
+Check [fhir-py-types](https://github.com/beda-software/fhir-py-types) for more details on generating type definitions from FHIR `StructureDefintion`
+
 ## get_by_path(path, default=None)
 ```Python
 patient_postal = patient.get_by_path(['resource', 'address', 0, 'postalCode'])
 
 # get_by_path can be also used on any nested attribute
 patient_name = patient.name[0]
 patient_fullname = '{} {}'.format(
@@ -387,14 +400,26 @@
 invoice = await client.resources('Invoice').first()
 base_value = invoice.get_by_path([
     'totalPriceComponent',
     {'type': 'base'},
     'amount', 'value'], 0)
 ```
 
+## set_by_path(obj, path, value)
+```python
+resource = {
+    "name": [{"given": ["Firstname"], "family": "Lastname"}],
+}
+
+set_by_path(resource, ["name", 0, "given", 0], "FirstnameUpdated")
+
+# resource
+# {"name": [{"given": ["FirstnameUpdated"], "family": "Lastname"}]}
+```
+
 ## serialize()
 ```Python
 # Returns resources as dict
 patient = await client.reference('Patient', '1').to_resource()
 patient.serialize()
 # Or 
 await client.reference('Patient', '1').to_resource().serialize()
```

### Comparing `fhirpy-1.3.1/fhirpy/base/exceptions.py` & `fhirpy-1.3.2/fhirpy/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `fhirpy-1.3.1/fhirpy/base/lib.py` & `fhirpy-1.3.2/fhirpy/base/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         pass
 
     @abstractmethod  # pragma: no cover
     def _fetch_resource(self, path, params=None):
         pass
 
     def _build_request_headers(self):
-        headers = {"Accept": "application/json"}
+        headers = {"Accept": "application/fhir+json"}
 
         if self.authorization:
             headers["Authorization"] = self.authorization
 
         if self.extra_headers is not None:
             headers = {**headers, **self.extra_headers}
```

### Comparing `fhirpy-1.3.1/fhirpy/base/resource.py` & `fhirpy-1.3.2/fhirpy/base/resource.py`

 * *Files identical despite different names*

### Comparing `fhirpy-1.3.1/fhirpy/base/searchset.py` & `fhirpy-1.3.2/fhirpy/base/searchset.py`

 * *Files identical despite different names*

### Comparing `fhirpy-1.3.1/fhirpy/base/utils.py` & `fhirpy-1.3.2/fhirpy/base/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -198,9 +198,30 @@
                 rv = rv[key]
 
         return rv
     except (IndexError, KeyError, AttributeError):
         return default
 
 
+def set_by_path(obj, path, value):
+    cursor = obj
+    last_part = path.pop()
+
+    for index, part in enumerate(path):
+        if isinstance(cursor, dict) and part not in cursor:
+            nextpart = (path + [last_part])[index + 1]
+            try:
+                nnextpart = (path + [last_part])[index + 2]
+            except IndexError:
+                nnextpart = ""
+
+            if isinstance(nextpart, int):
+                cursor[part] = [[] if isinstance(nnextpart, int) else {}]
+            else:
+                cursor[part] = {}
+
+        cursor = cursor[part]
+    cursor[last_part] = value
+
+
 def remove_prefix(s, prefix):
     return s[len(prefix) :] if s.startswith(prefix) else s
```

### Comparing `fhirpy-1.3.1/fhirpy/lib.py` & `fhirpy-1.3.2/fhirpy/lib.py`

 * *Files identical despite different names*

### Comparing `fhirpy-1.3.1/pyproject.toml` & `fhirpy-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fhirpy-1.3.1/PKG-INFO` & `fhirpy-1.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhirpy
-Version: 1.3.1
+Version: 1.3.2
 Summary: FHIR client for python
 Keywords: fhir
 Author-email: "beda.software" <fhirpy@beda.software>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -25,18 +25,18 @@
 Requires-Dist: pytest-asyncio>=0.15.1 ; extra == "test"
 Requires-Dist: responses>=0.13.3 ; extra == "test"
 Project-URL: Documentation, https://github.com/beda-software/fhir-py#readme
 Project-URL: Homepage, https://github.com/beda-software/fhir-py
 Project-URL: Source, https://github.com/beda-software/fhir-py.git
 Provides-Extra: test
 
-[![Build Status](https://travis-ci.com/beda-software/fhir-py.svg?branch=master)](https://travis-ci.com/beda-software/fhir-py)
+[![build status](https://github.com/beda-software/fhir-py/actions/workflows/build.yaml/badge.svg)](https://github.com/beda-software/fhir-py/actions/workflows/build.yaml)
 [![codecov](https://codecov.io/gh/beda-software/fhir-py/branch/master/graph/badge.svg)](https://codecov.io/gh/beda-software/fhir-py)
-[![pypi](https://img.shields.io/pypi/v/fhirpy.svg)](https://pypi.python.org/pypi/fhirpy)
-[![Supported Python version](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
+[![pypi](https://img.shields.io/pypi/v/fhirpy.svg)](https://pypi.org/project/fhirpy)
+[![Supported Python version](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 
 # fhir-py
 async/sync FHIR client for python3.
 This package provides an API for CRUD operations over FHIR resources
 
 ```pip install fhirpy```
 
@@ -72,14 +72,15 @@
     - [Wild card (any search parameter of type=reference be included)](#wild-card-any-search-parameter-of-typereference-be-included)
   - [Revinclude](#revinclude)
     - [Wild card (any search parameter of type=reference be included)](#wild-card-any-search-parameter-of-typereference-be-included-1)
 - [Resource and helper methods](#resource-and-helper-methods)
   - [Validate resource using operation $validate](#validate-resource-using-operation-validate)
   - [Accessing resource attributes](#accessing-resource-attributes)
   - [get_by_path(path, default=None)](#get_by_pathpath-defaultnone)
+  - [set_by_path(obj, path, value)](#set_by_pathpath)
   - [serialize()](#serialize)
 - [Reference](#reference-1)
   - [Main class structure](#main-class-structure)
   - [Acync client (based on _aiohttp_) – AsyncFHIRClient](#acync-client-based-on-_aiohttp_--asyncfhirclient)
     - [AsyncFHIRResource](#asyncfhirresource)
     - [AsyncFHIRReference](#asyncfhirreference)
     - [AsyncFHIRSearchSet](#asyncfhirsearchset)
@@ -392,14 +393,26 @@
 # Work with the resource as a dictionary
 patient_family = patient['name'][0]['family']
 
 # Or access value by an attribute
 patient_given_name = patient.name[0].given[0]
 ```
 
+## Static type checking with [mypy](https://github.com/python/mypy) and [fhir-py-types](https://github.com/beda-software/fhir-py-types)
+```Python
+from fhir_py_types.generated.resources import Patient
+
+patient: Patient = await client.resources('Patient').first()
+
+# Works only with dictionary-like resource access
+patient_family = patient['name'][0]['family1']
+# 'TypedDict "HumanName" has no key "family1" note: Did you mean "family"?'
+```
+Check [fhir-py-types](https://github.com/beda-software/fhir-py-types) for more details on generating type definitions from FHIR `StructureDefintion`
+
 ## get_by_path(path, default=None)
 ```Python
 patient_postal = patient.get_by_path(['resource', 'address', 0, 'postalCode'])
 
 # get_by_path can be also used on any nested attribute
 patient_name = patient.name[0]
 patient_fullname = '{} {}'.format(
@@ -418,14 +431,26 @@
 invoice = await client.resources('Invoice').first()
 base_value = invoice.get_by_path([
     'totalPriceComponent',
     {'type': 'base'},
     'amount', 'value'], 0)
 ```
 
+## set_by_path(obj, path, value)
+```python
+resource = {
+    "name": [{"given": ["Firstname"], "family": "Lastname"}],
+}
+
+set_by_path(resource, ["name", 0, "given", 0], "FirstnameUpdated")
+
+# resource
+# {"name": [{"given": ["FirstnameUpdated"], "family": "Lastname"}]}
+```
+
 ## serialize()
 ```Python
 # Returns resources as dict
 patient = await client.reference('Patient', '1').to_resource()
 patient.serialize()
 # Or 
 await client.reference('Patient', '1').to_resource().serialize()
```

