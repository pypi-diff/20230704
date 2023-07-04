# Comparing `tmp/configzen-0.5.4.tar.gz` & `tmp/configzen-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.5.4.tar", max compression
+gzip compressed data, was "configzen-0.5.6.tar", max compression
```

## Comparing `configzen-0.5.4.tar` & `configzen-0.5.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      536 2023-06-29 17:13:35.607166 configzen-0.5.4/configzen/__init__.py
--rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.5.4/configzen/__main__.py
--rw-r--r--   0        0        0     1681 2023-07-03 13:55:18.269988 configzen-0.5.4/configzen/_isolation.py
--rw-r--r--   0        0        0     3375 2023-07-01 12:22:23.319430 configzen-0.5.4/configzen/_setup.py
--rw-r--r--   0        0        0    77601 2023-07-03 19:32:23.279282 configzen-0.5.4/configzen/config.py
--rw-r--r--   0        0        0     5232 2023-07-03 13:00:51.582780 configzen-0.5.4/configzen/decorators.py
--rw-r--r--   0        0        0     4434 2023-07-03 13:55:18.493989 configzen-0.5.4/configzen/errors.py
--rw-r--r--   0        0        0      531 2023-06-27 21:14:31.456634 configzen-0.5.4/configzen/field.py
--rw-r--r--   0        0        0     6736 2023-07-03 13:00:51.893832 configzen-0.5.4/configzen/interpolation.py
--rw-r--r--   0        0        0    26250 2023-07-03 13:16:45.908317 configzen-0.5.4/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.5.4/configzen/py.typed
--rw-r--r--   0        0        0     4704 2023-07-03 13:21:43.983660 configzen-0.5.4/configzen/route.py
--rw-r--r--   0        0        0     1197 2023-07-03 12:44:27.155689 configzen-0.5.4/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.5.4/LICENSE
--rw-r--r--   0        0        0     1474 2023-07-03 20:57:37.732630 configzen-0.5.4/pyproject.toml
--rw-r--r--   0        0        0    14350 2023-06-29 18:06:31.120725 configzen-0.5.4/README.md
--rw-r--r--   0        0        0    14870 1970-01-01 00:00:00.000000 configzen-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      536 2023-06-29 17:13:35.607166 configzen-0.5.6/configzen/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.5.6/configzen/__main__.py
+-rw-r--r--   0        0        0     1681 2023-07-03 13:55:18.269988 configzen-0.5.6/configzen/_isolation.py
+-rw-r--r--   0        0        0     3375 2023-07-01 12:22:23.319430 configzen-0.5.6/configzen/_setup.py
+-rw-r--r--   0        0        0    78116 2023-07-04 17:12:24.284924 configzen-0.5.6/configzen/config.py
+-rw-r--r--   0        0        0     5206 2023-07-04 17:07:03.452372 configzen-0.5.6/configzen/decorators.py
+-rw-r--r--   0        0        0     4434 2023-07-03 13:55:18.493989 configzen-0.5.6/configzen/errors.py
+-rw-r--r--   0        0        0      491 2023-07-04 19:06:00.928709 configzen-0.5.6/configzen/field.py
+-rw-r--r--   0        0        0     6740 2023-07-04 09:58:16.042313 configzen-0.5.6/configzen/interpolation.py
+-rw-r--r--   0        0        0    26250 2023-07-03 13:16:45.908317 configzen-0.5.6/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.5.6/configzen/py.typed
+-rw-r--r--   0        0        0     4704 2023-07-03 13:21:43.983660 configzen-0.5.6/configzen/route.py
+-rw-r--r--   0        0        0     1197 2023-07-03 12:44:27.155689 configzen-0.5.6/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.5.6/LICENSE
+-rw-r--r--   0        0        0     1474 2023-07-04 19:06:29.565837 configzen-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0    14350 2023-06-29 18:06:31.120725 configzen-0.5.6/README.md
+-rw-r--r--   0        0        0    14870 1970-01-01 00:00:00.000000 configzen-0.5.6/PKG-INFO
```

### Comparing `configzen-0.5.4/configzen/__init__.py` & `configzen-0.5.6/configzen/__init__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.5.4/configzen/__main__.py` & `configzen-0.5.6/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.5.4/configzen/_isolation.py` & `configzen-0.5.6/configzen/_isolation.py`

 * *Files identical despite different names*

### Comparing `configzen-0.5.4/configzen/_setup.py` & `configzen-0.5.6/configzen/_setup.py`

 * *Files identical despite different names*

### Comparing `configzen-0.5.4/configzen/config.py` & `configzen-0.5.6/configzen/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,22 +98,24 @@
 from configzen._isolation import isolate_run, isolate_await, isolation_runner
 from configzen.errors import (
     ConfigAccessError,
     ResourceLookupError,
     UnavailableParserError,
     UnspecifiedParserError,
     InterpolationLookupError,
+    InterpolationError,
 )
 from configzen.interpolation import (
-    INTERPOLATION_NAMESPACE_TOKEN,
+    NAMESPACE_TOKEN,
     INTERPOLATOR,
     BaseInterpolator,
     include_const,
     interpolate,
     include,
+    AT_TOKEN,
 )
 from configzen.processor import EXPORT, DirectiveContext, Processor
 from configzen.route import ConfigRoute
 from configzen.typedefs import (
     AsyncConfigIO,
     ConfigIO,
     ConfigModelT,
@@ -451,14 +453,15 @@
         "ion",
         "bson",
         "cbor",
         "cbor2",
         "msgpack",
         "pickle",
     }
+    SUPPORTED_PARSERS: list[str] = anyconfig.list_types()
 
     def __init__(
         self,
         resource: RawResourceT,
         parser_name: str | None = None,
         processor_class: type[Processor[ConfigModelT]] | None = None,
         *,
@@ -565,15 +568,15 @@
             value = value.casefold()
         self._parser_name = value
 
     def _guess_parser_name(self) -> str | None:
         parser_name = None
         if isinstance(self.resource, pathlib.Path):
             suffix = self.resource.suffix[1:].casefold()
-            supported_parsers = anyconfig.list_types()
+            supported_parsers = self.SUPPORTED_PARSERS
             if not suffix:
                 recognized_file_extensions = supported_parsers + [
                     alias + "(-> " + actual_parser_name + ")"
                     for alias, actual_parser_name in self.EXTRA_FILE_EXTENSIONS.items()
                     if actual_parser_name in supported_parsers
                 ]
                 msg = (
@@ -1709,16 +1712,16 @@
         try:
             interpolated = interpolate(
                 post_hook_value,
                 cls,
                 values.copy(),
                 field.outer_type_,
             )
-        except InterpolationLookupError as err:
-            err.message += f" (issued by {cls.__qualname__}.{field.alias})"
+        except InterpolationError as err:
+            err.message += f" (encountered in {cls.__qualname__}.{field.alias})"
             raise
 
         new_value = field_hook(field.outer_type_, interpolated)
         if old_value != new_value:
             interpolation_tracker[field.alias] = (old_value, copy.copy(new_value))
         post_hook_value = new_value
     return post_hook_value
@@ -2377,34 +2380,46 @@
             namespaces.setdefault(None, {}).update(
                 context.toplevel_interpolation_namespace
             )
         for identifier in identifiers:
             (
                 namespace_identifier,
                 specifies_namespace,
-                raw_identifier,
-            ) = identifier.rpartition(INTERPOLATION_NAMESPACE_TOKEN)
+                raw_route,
+            ) = identifier.rpartition(NAMESPACE_TOKEN)
             namespace = namespaces.get(None, {})
             if specifies_namespace:
                 try:
                     namespace |= namespaces[namespace_identifier]
                 except KeyError:
                     raise InterpolationLookupError(namespace_identifier) from None
             else:
                 namespace |= closest_namespace
 
+            owner, has_at, raw_route = raw_route.rpartition(AT_TOKEN)
+
+            lookup_identifier = owner if has_at else raw_route
             try:
-                value = at(namespace, raw_identifier)
+                value = at(namespace, lookup_identifier)
             except ResourceLookupError:
                 if not specifies_namespace:
                     raise
-                value = at(closest_namespace, raw_identifier)
+                value = at(closest_namespace, lookup_identifier)
+
+            if has_at:
+                owner = value
+                if not isinstance(owner, ConfigModel):
+                    raise InterpolationError(
+                        f"Cannot @-interpolate with {type(owner).__name__!r} objects"
+                    )
+                value = owner.at(raw_route)
+
             interpolation_context[identifier] = value
-            if raw_identifier not in closest_namespace:
-                interpolation_context[raw_identifier] = value
+            if raw_route not in closest_namespace:
+                interpolation_context[raw_route] = value
 
         return interpolation_context
 
     @classmethod
     def __field_setup__(cls, value: dict[str, Any], field: ModelField) -> Any:
         """
         Called when this configuration model is being initialized as a field
```

### Comparing `configzen-0.5.4/configzen/decorators.py` & `configzen-0.5.6/configzen/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         return functools.partial(with_export_hook, func)
 
     export_hook.register(cls, func)
 
     if not hasattr(cls, "__get_validators__"):
 
         def validator_gen() -> Iterator[Callable[[Any], Any]]:
-            hook_func = field_hook.dispatch(cls)  # type: ignore[arg-type]
+            hook_func = field_hook.dispatch(cls)
             yield lambda value: hook_func(cls, value)
 
         with contextlib.suppress(TypeError):
             cls.__get_validators__ = validator_gen  # type: ignore[attr-defined]
 
     return cls
```

### Comparing `configzen-0.5.4/configzen/errors.py` & `configzen-0.5.6/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.5.4/configzen/interpolation.py` & `configzen-0.5.6/configzen/interpolation.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 
 __all__ = (
     "interpolate",
     "include",
 )
 
 INTERPOLATOR: str = "__interpolator__"
-INTERPOLATION_NAMESPACE_TOKEN: str = "::"
+NAMESPACE_TOKEN: str = "::"
+AT_TOKEN: str = "@"
 
 
 class ConfigInterpolationTemplate(string.Template):
-    idpattern = rf"([_a-z]*({INTERPOLATION_NAMESPACE_TOKEN})?[_a-z][\\\.\[\]_a-z0-9]*)"
+    idpattern = rf"([_a-z]*({NAMESPACE_TOKEN}|{AT_TOKEN})?[_a-z][\\\.\[\]_a-z0-9]*)"
     flags = re.IGNORECASE
 
     if sys.version_info < (3, 11):
 
         def get_identifiers(self) -> list[str]:
             ids = []
             for mo in self.pattern.finditer(self.template):
```

### Comparing `configzen-0.5.4/configzen/processor.py` & `configzen-0.5.6/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.5.4/configzen/route.py` & `configzen-0.5.6/configzen/route.py`

 * *Files identical despite different names*

### Comparing `configzen-0.5.4/configzen/typedefs.py` & `configzen-0.5.6/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.5.4/LICENSE` & `configzen-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.5.4/pyproject.toml` & `configzen-0.5.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.5.4"
+version = "0.5.6"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.5.4/README.md` & `configzen-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.5.4/PKG-INFO` & `configzen-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.5.4
+Version: 0.5.6
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

