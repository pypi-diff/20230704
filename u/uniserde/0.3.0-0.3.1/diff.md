# Comparing `tmp/uniserde-0.3.0.tar.gz` & `tmp/uniserde-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniserde-0.3.0.tar", max compression
+gzip compressed data, was "uniserde-0.3.1.tar", max compression
```

## Comparing `uniserde-0.3.0.tar` & `uniserde-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     7626 2023-07-04 14:25:24.085255 uniserde-0.3.0/README.md
--rw-r--r--   0        0        0      645 2023-07-04 19:22:20.798470 uniserde-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      328 2023-07-04 19:27:50.392268 uniserde-0.3.0/uniserde/__init__.py
--rw-r--r--   0        0        0     1505 2023-07-04 19:24:43.375352 uniserde-0.3.0/uniserde/bson_deserialize.py
--rw-r--r--   0        0        0     7833 2023-07-04 19:25:42.112100 uniserde-0.3.0/uniserde/caching_deserializer.py
--rw-r--r--   0        0        0     1210 2023-07-04 19:24:43.375352 uniserde-0.3.0/uniserde/case_convert.py
--rw-r--r--   0        0        0     4091 2023-07-04 18:37:13.467910 uniserde-0.3.0/uniserde/common.py
--rw-r--r--   0        0        0     5686 2023-07-04 19:25:42.118767 uniserde-0.3.0/uniserde/json_deserialize.py
--rw-r--r--   0        0        0     1974 2023-07-04 19:24:43.382018 uniserde-0.3.0/uniserde/objectid_proxy.py
--rw-r--r--   0        0        0     7094 2023-07-04 19:24:43.378685 uniserde-0.3.0/uniserde/schema_mongodb.py
--rw-r--r--   0        0        0     2152 2023-07-04 19:24:43.382018 uniserde-0.3.0/uniserde/serde_bson.py
--rw-r--r--   0        0        0     2697 2023-07-04 19:28:59.365686 uniserde-0.3.0/uniserde/serde_class.py
--rw-r--r--   0        0        0     5275 2023-07-04 19:24:43.378685 uniserde-0.3.0/uniserde/serde_json.py
--rw-r--r--   0        0        0      487 2023-07-04 19:24:43.382018 uniserde-0.3.0/uniserde/typedefs.py
--rw-r--r--   0        0        0     8352 1970-01-01 00:00:00.000000 uniserde-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     7626 2023-07-04 14:25:24.085255 uniserde-0.3.1/README.md
+-rw-r--r--   0        0        0      645 2023-07-04 19:33:56.512688 uniserde-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-07-04 19:27:50.392268 uniserde-0.3.1/uniserde/__init__.py
+-rw-r--r--   0        0        0     1505 2023-07-04 19:33:35.559332 uniserde-0.3.1/uniserde/bson_deserialize.py
+-rw-r--r--   0        0        0     7941 2023-07-04 19:33:02.725963 uniserde-0.3.1/uniserde/caching_deserializer.py
+-rw-r--r--   0        0        0     1210 2023-07-04 19:24:43.375352 uniserde-0.3.1/uniserde/case_convert.py
+-rw-r--r--   0        0        0     4091 2023-07-04 18:37:13.467910 uniserde-0.3.1/uniserde/common.py
+-rw-r--r--   0        0        0     5686 2023-07-04 19:32:32.782597 uniserde-0.3.1/uniserde/json_deserialize.py
+-rw-r--r--   0        0        0     1974 2023-07-04 19:24:43.382018 uniserde-0.3.1/uniserde/objectid_proxy.py
+-rw-r--r--   0        0        0     7094 2023-07-04 19:24:43.378685 uniserde-0.3.1/uniserde/schema_mongodb.py
+-rw-r--r--   0        0        0     2152 2023-07-04 19:24:43.382018 uniserde-0.3.1/uniserde/serde_bson.py
+-rw-r--r--   0        0        0     2697 2023-07-04 19:28:59.365686 uniserde-0.3.1/uniserde/serde_class.py
+-rw-r--r--   0        0        0     5275 2023-07-04 19:24:43.378685 uniserde-0.3.1/uniserde/serde_json.py
+-rw-r--r--   0        0        0      487 2023-07-04 19:24:43.382018 uniserde-0.3.1/uniserde/typedefs.py
+-rw-r--r--   0        0        0     8352 1970-01-01 00:00:00.000000 uniserde-0.3.1/PKG-INFO
```

### Comparing `uniserde-0.3.0/README.md` & `uniserde-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.0/pyproject.toml` & `uniserde-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uniserde"
-version = "0.3.0"
+version = "0.3.1"
 description = "Convention based, effortless serialization and deserialization"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/uniserde"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `uniserde-0.3.0/uniserde/bson_deserialize.py` & `uniserde-0.3.1/uniserde/bson_deserialize.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.0/uniserde/caching_deserializer.py` & `uniserde-0.3.1/uniserde/caching_deserializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,20 @@
     _override_method_name: str
 
     def __init_subclass__(cls) -> None:
         def make_deserializer_from_passthrough_type(
             passthrough_type: Type,
         ) -> Callable[[Self, T, Type], Any]:
             def result(self, value: T, as_type: Type[V]) -> V:
-                if not isinstance(value, as_type):
+                if not isinstance(value, as_type) and not (
+                    isinstance(value, int) and as_type is float
+                ):
                     raise SerdeError(f"Expected `{as_type}`, got `{value}`")
 
-                return value
+                return value  # type: ignore
 
             return result
 
         for typ in cls._passthrough_types:
             cls._deserializer_cache[typ] = make_deserializer_from_passthrough_type(typ)
 
     def __init__(
```

### Comparing `uniserde-0.3.0/uniserde/case_convert.py` & `uniserde-0.3.1/uniserde/case_convert.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.0/uniserde/common.py` & `uniserde-0.3.1/uniserde/common.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.0/uniserde/json_deserialize.py` & `uniserde-0.3.1/uniserde/json_deserialize.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.0/uniserde/objectid_proxy.py` & `uniserde-0.3.1/uniserde/objectid_proxy.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.0/uniserde/schema_mongodb.py` & `uniserde-0.3.1/uniserde/schema_mongodb.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.0/uniserde/serde_bson.py` & `uniserde-0.3.1/uniserde/serde_bson.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.0/uniserde/serde_class.py` & `uniserde-0.3.1/uniserde/serde_class.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.0/uniserde/serde_json.py` & `uniserde-0.3.1/uniserde/serde_json.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.0/PKG-INFO` & `uniserde-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniserde
-Version: 0.3.0
+Version: 0.3.1
 Summary: Convention based, effortless serialization and deserialization
 Home-page: https://gitlab.com/Vivern/uniserde
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

