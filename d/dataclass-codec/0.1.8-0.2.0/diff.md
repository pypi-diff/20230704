# Comparing `tmp/dataclass_codec-0.1.8.tar.gz` & `tmp/dataclass_codec-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_codec-0.1.8.tar", max compression
+gzip compressed data, was "dataclass_codec-0.2.0.tar", max compression
```

## Comparing `dataclass_codec-0.1.8.tar` & `dataclass_codec-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      101 2023-06-21 01:50:47.819434 dataclass_codec-0.1.8/README.md
--rw-r--r--   0        0        0      600 2023-07-02 21:56:10.944136 dataclass_codec-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      246 2023-06-21 01:44:15.139451 dataclass_codec-0.1.8/src/dataclass_codec/__init__.py
--rw-r--r--   0        0        0    11144 2023-07-02 21:54:59.534143 dataclass_codec-0.1.8/src/dataclass_codec/decode.py
--rw-r--r--   0        0        0     2929 2023-06-21 01:51:35.509431 dataclass_codec-0.1.8/src/dataclass_codec/encode.py
--rw-r--r--   0        0        0        0 2023-06-21 01:44:15.139451 dataclass_codec-0.1.8/src/dataclass_codec/py.typed
--rw-r--r--   0        0        0    16307 2023-07-02 21:49:06.364177 dataclass_codec-0.1.8/src/dataclass_codec/tests/test_dataclass_codec.py
--rw-r--r--   0        0        0      391 2023-07-02 21:53:28.544152 dataclass_codec-0.1.8/src/dataclass_codec/types_predicates.py
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 dataclass_codec-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      101 2023-06-21 01:55:42.515322 dataclass_codec-0.2.0/README.md
+-rw-r--r--   0        0        0      600 2023-07-04 17:52:35.754528 dataclass_codec-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-06-18 01:48:53.622553 dataclass_codec-0.2.0/src/dataclass_codec/__init__.py
+-rw-r--r--   0        0        0    11398 2023-07-04 17:51:04.614112 dataclass_codec-0.2.0/src/dataclass_codec/decode.py
+-rw-r--r--   0        0        0     2929 2023-06-21 01:55:42.515322 dataclass_codec-0.2.0/src/dataclass_codec/encode.py
+-rw-r--r--   0        0        0        0 2023-06-18 00:31:15.872983 dataclass_codec-0.2.0/src/dataclass_codec/py.typed
+-rw-r--r--   0        0        0    16510 2023-07-04 17:51:47.624314 dataclass_codec-0.2.0/src/dataclass_codec/tests/test_dataclass_codec.py
+-rw-r--r--   0        0        0      391 2023-07-04 17:50:20.533913 dataclass_codec-0.2.0/src/dataclass_codec/types_predicates.py
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 dataclass_codec-0.2.0/PKG-INFO
```

### Comparing `dataclass_codec-0.1.8/pyproject.toml` & `dataclass_codec-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-codec"
-version = "0.1.8"
+version = "0.2.0"
 description = ""
 authors = ["lucas.silva <lucas.silva@jeaholding.com.br>"]
 readme = "README.md"
 packages = [{include = "dataclass_codec", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dataclass_codec-0.1.8/src/dataclass_codec/decode.py` & `dataclass_codec-0.2.0/src/dataclass_codec/decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,17 +230,17 @@
     )
 
 
 def generic_dataclass_from_primitive_dict(
     obj: Any, _type: ANYTYPE, decode_it: DECODEIT
 ) -> Any:
     cxt = decode_context()
-    assert is_generic_dataclass_predicate(_type), "{} is not a dataclass".format(
-        _type.__name__
-    )
+    assert is_generic_dataclass_predicate(
+        _type
+    ), "{} is not a dataclass".format(_type.__name__)
 
     assert isinstance(obj, dict), "{} is {} not dict".format(
         current_path(), type(obj)
     )
 
     def make_value(k: str) -> Any:
         with current_path_scope(current_path() + "." + k):
@@ -249,29 +249,35 @@
                     return None
                 else:
                     raise ValueError(f"Missing key {k}")
 
             return decode_it(obj[k], _type.__args__[0])
 
     return _type(
-        **{k: make_value(k) for k in _type.__origin__.__dataclass_fields__.keys()}
+        **{
+            k: make_value(k)
+            for k in _type.__origin__.__dataclass_fields__.keys()
+        }
     )
 
+
 def decimal_from_str(obj: Any, _type: ANYTYPE, _decode_it: DECODEIT) -> Any:
     assert isinstance(
         obj, (str, int, float)
     ), "{} is {} not str, int or float".format(current_path(), type(obj))
     return Decimal(obj)
 
+
 def uuid_from_str(obj: Any, _type: ANYTYPE, _decode_it: DECODEIT) -> Any:
-    assert isinstance(
-        obj, str
-    ), "{} is {} not str".format(current_path(), type(obj))
+    assert isinstance(obj, str), "{} is {} not str".format(
+        current_path(), type(obj)
+    )
     return UUID(obj)
 
+
 def is_generic_list_predicate(_type: ANYTYPE) -> bool:
     return hasattr(_type, "__origin__") and _type.__origin__ is list
 
 
 def generic_list_decoder(obj: Any, _type: ANYTYPE, decode_it: DECODEIT) -> Any:
     assert is_generic_list_predicate(_type), "{} is not a list".format(
         _type.__name__
@@ -366,14 +372,22 @@
 
     type(obj)
     supertype = _type.__supertype__
 
     return _type(decode_it(obj, supertype))
 
 
+def is_any_type_predicate(_type: ANYTYPE) -> bool:
+    return _type is Any
+
+
+def any_type_decoder(obj: Any, _type: ANYTYPE, decode_it: DECODEIT) -> Any:
+    return obj
+
+
 DEFAULT_DECODERS: Dict[ANYTYPE, TYPEDECODER] = {
     **{
         t: primitive_hook(t)
         for t in (
             int,
             float,
             str,
@@ -388,14 +402,15 @@
     date: iso_date_to_date,
     time: iso_time_to_time,
     Decimal: decimal_from_str,
     UUID: uuid_from_str,
 }
 
 DEFAULT_DECODERS_BY_PREDICATE: List[Tuple[TYPEMATCHPREDICATE, TYPEDECODER]] = [
+    (is_any_type_predicate, any_type_decoder),
     (is_dataclass_predicate, dataclass_from_primitive_dict),
     (is_generic_dataclass_predicate, generic_dataclass_from_primitive_dict),
     (is_generic_list_predicate, generic_list_decoder),
     (is_generic_dict_predicate, generic_dict_decoder),
     (is_union_predicate, generic_union_decoder),
     # This must be before is_enum_predicate
     (is_new_type_predicate, generic_new_type_decoder),
```

### Comparing `dataclass_codec-0.1.8/src/dataclass_codec/encode.py` & `dataclass_codec-0.2.0/src/dataclass_codec/encode.py`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.1.8/src/dataclass_codec/tests/test_dataclass_codec.py` & `dataclass_codec-0.2.0/src/dataclass_codec/tests/test_dataclass_codec.py`

 * *Files 0% similar despite different names*

```diff
@@ -582,16 +582,23 @@
     def test_decode_raw_uuid(self) -> None:
         import uuid
 
         assert decode(
             "12345678-1234-5678-1234-567812345678", uuid.UUID
         ) == uuid.UUID("12345678-1234-5678-1234-567812345678")
 
-
     def test_generic_dataclass(self) -> None:
-        T = TypeVar("T"	)
-        
+        T = TypeVar("T")
+
         @dataclass
         class GenericDummy(Generic[T]):
             a: T
 
-        assert decode({"a": 1}, GenericDummy[int]) == GenericDummy(1)
+        assert decode({"a": 1}, GenericDummy[int]) == GenericDummy(1)
+
+    def test_any_type(self) -> None:
+        @dataclass
+        class Dummy:
+            a: Any
+
+        assert decode({"a": 1}, Dummy) == Dummy(1)
+        assert decode({"a": "hello"}, Dummy) == Dummy("hello")
```

### Comparing `dataclass_codec-0.1.8/PKG-INFO` & `dataclass_codec-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-codec
-Version: 0.1.8
+Version: 0.2.0
 Summary: 
 Author: lucas.silva
 Author-email: lucas.silva@jeaholding.com.br
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

