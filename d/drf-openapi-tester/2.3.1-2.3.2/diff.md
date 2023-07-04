# Comparing `tmp/drf_openapi_tester-2.3.1.tar.gz` & `tmp/drf_openapi_tester-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_openapi_tester-2.3.1.tar", max compression
+gzip compressed data, was "drf_openapi_tester-2.3.2.tar", max compression
```

## Comparing `drf_openapi_tester-2.3.1.tar` & `drf_openapi_tester-2.3.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     2195 2022-12-02 08:37:45.729417 drf_openapi_tester-2.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     1500 2022-12-02 08:37:45.729417 drf_openapi_tester-2.3.1/LICENSE
--rw-r--r--   0        0        0     7754 2022-12-02 08:37:45.729417 drf_openapi_tester-2.3.1/README.md
--rw-r--r--   0        0        0      554 2022-12-02 08:37:45.729417 drf_openapi_tester-2.3.1/openapi_tester/__init__.py
--rw-r--r--   0        0        0     1134 2022-12-02 08:37:45.729417 drf_openapi_tester-2.3.1/openapi_tester/case_testers.py
--rw-r--r--   0        0        0     1131 2022-12-02 08:37:45.729417 drf_openapi_tester-2.3.1/openapi_tester/clients.py
--rw-r--r--   0        0        0     2812 2022-12-02 08:37:45.729417 drf_openapi_tester-2.3.1/openapi_tester/constants.py
--rw-r--r--   0        0        0      742 2022-12-02 08:37:45.729417 drf_openapi_tester-2.3.1/openapi_tester/exceptions.py
--rw-r--r--   0        0        0    10830 2022-12-02 08:37:45.729417 drf_openapi_tester-2.3.1/openapi_tester/loaders.py
--rw-r--r--   0        0        0        0 2022-12-02 08:37:45.729417 drf_openapi_tester-2.3.1/openapi_tester/py.typed
--rw-r--r--   0        0        0    17394 2022-12-02 08:37:45.729417 drf_openapi_tester-2.3.1/openapi_tester/schema_tester.py
--rw-r--r--   0        0        0     2150 2022-12-02 08:37:45.729417 drf_openapi_tester-2.3.1/openapi_tester/utils.py
--rw-r--r--   0        0        0     7855 2022-12-02 08:37:45.729417 drf_openapi_tester-2.3.1/openapi_tester/validators.py
--rw-r--r--   0        0        0     3456 2022-12-02 08:37:45.729417 drf_openapi_tester-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     9056 1970-01-01 00:00:00.000000 drf_openapi_tester-2.3.1/setup.py
--rw-r--r--   0        0        0    10491 1970-01-01 00:00:00.000000 drf_openapi_tester-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2195 2023-07-04 08:51:53.566787 drf_openapi_tester-2.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1500 2023-07-04 08:51:53.566787 drf_openapi_tester-2.3.2/LICENSE
+-rw-r--r--   0        0        0     7754 2023-07-04 08:51:53.566787 drf_openapi_tester-2.3.2/README.md
+-rw-r--r--   0        0        0      554 2023-07-04 08:51:53.566787 drf_openapi_tester-2.3.2/openapi_tester/__init__.py
+-rw-r--r--   0        0        0     1134 2023-07-04 08:51:53.566787 drf_openapi_tester-2.3.2/openapi_tester/case_testers.py
+-rw-r--r--   0        0        0     1131 2023-07-04 08:51:53.566787 drf_openapi_tester-2.3.2/openapi_tester/clients.py
+-rw-r--r--   0        0        0     2812 2023-07-04 08:51:53.566787 drf_openapi_tester-2.3.2/openapi_tester/constants.py
+-rw-r--r--   0        0        0      742 2023-07-04 08:51:53.566787 drf_openapi_tester-2.3.2/openapi_tester/exceptions.py
+-rw-r--r--   0        0        0    10870 2023-07-04 08:51:53.566787 drf_openapi_tester-2.3.2/openapi_tester/loaders.py
+-rw-r--r--   0        0        0        0 2023-07-04 08:51:53.566787 drf_openapi_tester-2.3.2/openapi_tester/py.typed
+-rw-r--r--   0        0        0    18170 2023-07-04 08:51:53.566787 drf_openapi_tester-2.3.2/openapi_tester/schema_tester.py
+-rw-r--r--   0        0        0     2150 2023-07-04 08:51:53.566787 drf_openapi_tester-2.3.2/openapi_tester/utils.py
+-rw-r--r--   0        0        0     7855 2023-07-04 08:51:53.566787 drf_openapi_tester-2.3.2/openapi_tester/validators.py
+-rw-r--r--   0        0        0     3395 2023-07-04 08:51:53.566787 drf_openapi_tester-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0    10172 1970-01-01 00:00:00.000000 drf_openapi_tester-2.3.2/PKG-INFO
```

### Comparing `drf_openapi_tester-2.3.1/CHANGELOG.md` & `drf_openapi_tester-2.3.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `drf_openapi_tester-2.3.1/LICENSE` & `drf_openapi_tester-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_openapi_tester-2.3.1/README.md` & `drf_openapi_tester-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `drf_openapi_tester-2.3.1/openapi_tester/__init__.py` & `drf_openapi_tester-2.3.2/openapi_tester/__init__.py`

 * *Files identical despite different names*

### Comparing `drf_openapi_tester-2.3.1/openapi_tester/case_testers.py` & `drf_openapi_tester-2.3.2/openapi_tester/case_testers.py`

 * *Files identical despite different names*

### Comparing `drf_openapi_tester-2.3.1/openapi_tester/clients.py` & `drf_openapi_tester-2.3.2/openapi_tester/clients.py`

 * *Files identical despite different names*

### Comparing `drf_openapi_tester-2.3.1/openapi_tester/constants.py` & `drf_openapi_tester-2.3.2/openapi_tester/constants.py`

 * *Files identical despite different names*

### Comparing `drf_openapi_tester-2.3.1/openapi_tester/exceptions.py` & `drf_openapi_tester-2.3.2/openapi_tester/exceptions.py`

 * *Files identical despite different names*

### Comparing `drf_openapi_tester-2.3.1/openapi_tester/loaders.py` & `drf_openapi_tester-2.3.2/openapi_tester/loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,11 +276,13 @@
 
         :return: Schema contents as a dict
         :raises: ImproperlyConfigured
         """
         response = requests.get(self.url, timeout=20)
         return cast(
             "dict",
-            json.loads(response.content)
-            if ".json" in self.url
-            else yaml.load(response.content, Loader=yaml.FullLoader),
+            (
+                json.loads(response.content)
+                if ".json" in self.url
+                else yaml.load(response.content, Loader=yaml.FullLoader)
+            ),
         )
```

### Comparing `drf_openapi_tester-2.3.1/openapi_tester/schema_tester.py` & `drf_openapi_tester-2.3.2/openapi_tester/schema_tester.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,24 +146,28 @@
             parameterized_path,
             f"\n\nUndocumented route {parameterized_path}.\n\nDocumented routes: " + "\n\t• ".join(paths_object.keys()),
         )
 
         method_object = self.get_key_value(
             route_object,
             response_method,
-            f"\n\nUndocumented method: {response_method}.\n\nDocumented methods: "
-            f"{[method.lower() for method in route_object.keys() if method.lower() != 'parameters']}.",
+            (
+                f"\n\nUndocumented method: {response_method}.\n\nDocumented methods: "
+                f"{[method.lower() for method in route_object.keys() if method.lower() != 'parameters']}."
+            ),
         )
 
         responses_object = self.get_key_value(method_object, "responses")
         status_code_object = self.get_status_code(
             responses_object,
             response.status_code,
-            f"\n\nUndocumented status code: {response.status_code}.\n\n"
-            f"Documented status codes: {list(responses_object.keys())}. ",
+            (
+                f"\n\nUndocumented status code: {response.status_code}.\n\n"
+                f"Documented status codes: {list(responses_object.keys())}. "
+            ),
         )
 
         if "openapi" not in schema:
             # openapi 2.0, i.e. "swagger" has a different structure than openapi 3.0 status sub-schemas
             return self.get_key_value(status_code_object, "schema")
 
         if status_code_object.get("content"):
@@ -171,16 +175,18 @@
                 status_code_object,
                 "content",
                 f"\n\nNo content documented for method: {response_method}, path: {parameterized_path}",
             )
             json_object = self.get_key_value(
                 content_object,
                 r"^application\/.*json$",
-                "\n\nNo `application/json` responses documented for method: "
-                f"{response_method}, path: {parameterized_path}",
+                (
+                    "\n\nNo `application/json` responses documented for method: "
+                    f"{response_method}, path: {parameterized_path}"
+                ),
                 use_regex=True,
             )
             return self.get_key_value(json_object, "schema")
 
         if response.data and response.json():  # type: ignore
             raise UndocumentedSchemaSectionError(
                 UNDOCUMENTED_SCHEMA_SECTION_ERROR.format(
@@ -229,14 +235,28 @@
         OpenApi 2 ref: https://help.apiary.io/api_101/swagger-extensions/
 
         :param schema_item: schema item
         :return: whether or not the item can be None
         """
         openapi_schema_3_nullable = "nullable"
         swagger_2_nullable = "x-nullable"
+        if "oneOf" in schema_item:
+            one_of: list[dict[str, Any]] = schema_item.get("oneOf", [])
+            return any(
+                nullable_key in schema and schema[nullable_key]
+                for schema in one_of
+                for nullable_key in [openapi_schema_3_nullable, swagger_2_nullable]
+            )
+        if "anyOf" in schema_item:
+            any_of: list[dict[str, Any]] = schema_item.get("anyOf", [])
+            return any(
+                nullable_key in schema and schema[nullable_key]
+                for schema in any_of
+                for nullable_key in [openapi_schema_3_nullable, swagger_2_nullable]
+            )
         return any(
             nullable_key in schema_item and schema_item[nullable_key]
             for nullable_key in [openapi_schema_3_nullable, swagger_2_nullable]
         )
 
     def test_key_casing(
         self,
```

### Comparing `drf_openapi_tester-2.3.1/openapi_tester/utils.py` & `drf_openapi_tester-2.3.2/openapi_tester/utils.py`

 * *Files identical despite different names*

### Comparing `drf_openapi_tester-2.3.1/openapi_tester/validators.py` & `drf_openapi_tester-2.3.2/openapi_tester/validators.py`

 * *Files identical despite different names*

### Comparing `drf_openapi_tester-2.3.1/pyproject.toml` & `drf_openapi_tester-2.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [tool.poetry]
 name = "drf-openapi-tester"
-version = "2.3.1"
+version = "2.3.2"
 description = "Test utility for validating OpenAPI response documentation"
 authors = ["Sondre Lillebø Gundersen <sondrelg@live.no>", "Na'aman Hirschfeld <nhirschfeld@gmail.com>"]
-maintainers = ["Na'aman Hirschfeld <nhirschfeld@gmail.com>"]
 license = "BSD-4-Clause"
 readme = "README.md"
 homepage = "https://github.com/snok/drf-openapi-tester"
 repository = "https://github.com/snok/drf-openapi-tester"
 documentation = "https://github.com/snok/drf-openapi-tester"
 keywords = ["openapi", "swagger", "api", "testing", "schema", "django", "drf"]
 classifiers = [
```

### Comparing `drf_openapi_tester-2.3.1/PKG-INFO` & `drf_openapi_tester-2.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-openapi-tester
-Version: 2.3.1
+Version: 2.3.2
 Summary: Test utility for validating OpenAPI response documentation
 Home-page: https://github.com/snok/drf-openapi-tester
 License: BSD-4-Clause
 Keywords: openapi,swagger,api,testing,schema,django,drf
 Author: Sondre Lillebø Gundersen
 Author-email: sondrelg@live.no
-Maintainer: Na'aman Hirschfeld
-Maintainer-email: nhirschfeld@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
@@ -28,35 +26,30 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Provides-Extra: drf-spectacular
 Provides-Extra: drf-yasg
-Requires-Dist: django (>=3,<4); python_full_version <= "3.7.0"
-Requires-Dist: django (>=3,<5); python_version >= "3.8"
+Requires-Dist: django (>=3,<4) ; python_full_version <= "3.7.0"
+Requires-Dist: django (>=3,<5) ; python_version >= "3.8"
 Requires-Dist: djangorestframework
-Requires-Dist: drf-spectacular; extra == "drf-spectacular"
-Requires-Dist: drf-yasg; extra == "drf-yasg"
+Requires-Dist: drf-spectacular ; extra == "drf-spectacular"
+Requires-Dist: drf-yasg ; extra == "drf-yasg"
 Requires-Dist: inflection
 Requires-Dist: openapi-spec-validator (>=0.4)
 Requires-Dist: prance
 Requires-Dist: pyYAML
 Project-URL: Documentation, https://github.com/snok/drf-openapi-tester
 Project-URL: Repository, https://github.com/snok/drf-openapi-tester
 Description-Content-Type: text/markdown
```

