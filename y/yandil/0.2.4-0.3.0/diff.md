# Comparing `tmp/yandil-0.2.4.tar.gz` & `tmp/yandil-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yandil-0.2.4.tar", max compression
+gzip compressed data, was "yandil-0.3.0.tar", max compression
```

## Comparing `yandil-0.2.4.tar` & `yandil-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1498 2023-06-30 17:01:10.398100 yandil-0.2.4/LICENSE
--rw-r--r--   0        0        0    11594 2023-06-30 17:01:10.398100 yandil-0.2.4/README.md
--rw-r--r--   0        0        0      988 2023-06-30 17:02:06.610940 yandil-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/__init__.py
--rw-r--r--   0        0        0      148 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/argument.py
--rw-r--r--   0        0        0        0 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/configuration/__init__.py
--rw-r--r--   0        0        0      800 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/configuration/configuration_container.py
--rw-r--r--   0        0        0      507 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/configuration/environment.py
--rw-r--r--   0        0        0    10681 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/container.py
--rw-r--r--   0        0        0        0 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/declarative/__init__.py
--rw-r--r--   0        0        0      516 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/declarative/decorators.py
--rw-r--r--   0        0        0      799 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/dependency.py
--rw-r--r--   0        0        0     1505 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/dependency_filler.py
--rw-r--r--   0        0        0        0 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/discovery/__init__.py
--rw-r--r--   0        0        0     3664 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/discovery/class_discovery.py
--rw-r--r--   0        0        0      883 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/discovery/module_discovery.py
--rw-r--r--   0        0        0        0 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/errors/__init__.py
--rw-r--r--   0        0        0      246 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/errors/abstract_class_not_allowed_error.py
--rw-r--r--   0        0        0      467 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/errors/configuration_value_type_mismatch_error.py
--rw-r--r--   0        0        0      239 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/errors/dependency_not_found_error.py
--rw-r--r--   0        0        0      257 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/errors/missing_configuration_value_error.py
--rw-r--r--   0        0        0      127 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/errors/missing_type_hint_item_type_error.py
--rw-r--r--   0        0        0      301 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/errors/primary_dependency_already_defined_error.py
--rw-r--r--   0        0        0      243 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/errors/primary_dependency_not_found_error.py
--rw-r--r--   0        0        0        0 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/loaders/__init__.py
--rw-r--r--   0        0        0     1188 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/loaders/declarative_dependency_loader.py
--rw-r--r--   0        0        0     4954 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/loaders/self_discover_dependency_loader.py
--rw-r--r--   0        0        0     1238 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/typing_tools.py
--rw-r--r--   0        0        0    12144 1970-01-01 00:00:00.000000 yandil-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1498 2023-07-04 16:42:16.635036 yandil-0.3.0/LICENSE
+-rw-r--r--   0        0        0    11594 2023-07-04 16:42:16.635036 yandil-0.3.0/README.md
+-rw-r--r--   0        0        0      988 2023-07-04 16:43:12.363825 yandil-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/__init__.py
+-rw-r--r--   0        0        0      148 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/argument.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/configuration/__init__.py
+-rw-r--r--   0        0        0      800 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/configuration/configuration_container.py
+-rw-r--r--   0        0        0      507 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/configuration/environment.py
+-rw-r--r--   0        0        0    10964 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/container.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/declarative/__init__.py
+-rw-r--r--   0        0        0      516 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/declarative/decorators.py
+-rw-r--r--   0        0        0      799 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/dependency.py
+-rw-r--r--   0        0        0     1505 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/dependency_filler.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/discovery/__init__.py
+-rw-r--r--   0        0        0     3653 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/discovery/class_discovery.py
+-rw-r--r--   0        0        0      883 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/discovery/module_discovery.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/errors/__init__.py
+-rw-r--r--   0        0        0      246 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/errors/abstract_class_not_allowed_error.py
+-rw-r--r--   0        0        0      467 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/errors/configuration_value_type_mismatch_error.py
+-rw-r--r--   0        0        0      239 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/errors/dependency_not_found_error.py
+-rw-r--r--   0        0        0      279 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/errors/instance_and_class_does_not_match_error.py
+-rw-r--r--   0        0        0      257 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/errors/missing_configuration_value_error.py
+-rw-r--r--   0        0        0      127 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/errors/missing_type_hint_item_type_error.py
+-rw-r--r--   0        0        0      301 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/errors/primary_dependency_already_defined_error.py
+-rw-r--r--   0        0        0      243 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/errors/primary_dependency_not_found_error.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/loaders/__init__.py
+-rw-r--r--   0        0        0     1188 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/loaders/declarative_dependency_loader.py
+-rw-r--r--   0        0        0     4954 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/loaders/self_discover_dependency_loader.py
+-rw-r--r--   0        0        0     1238 2023-07-04 16:42:16.635036 yandil-0.3.0/src/yandil/typing_tools.py
+-rw-r--r--   0        0        0    12144 1970-01-01 00:00:00.000000 yandil-0.3.0/PKG-INFO
```

### Comparing `yandil-0.2.4/LICENSE` & `yandil-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yandil-0.2.4/README.md` & `yandil-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `yandil-0.2.4/pyproject.toml` & `yandil-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yandil"
-version = "0.2.4"
+version = "0.3.0"
 description = "Yet ANother Dependency Injection Library"
 readme = "README.md"
 authors = ["DeejayRevok <seryi_one@hotmail.com>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/DeejayRevok/yandil"
 homepage = "https://github.com/DeejayRevok/yandil"
 keywords = ["dependency injection", "di"]
@@ -34,15 +34,15 @@
 [tool.isort]
 profile = "black"
 py_version=310
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.2.4"
+version = "0.3.0"
 tag_format = "$version"
 version_files = [
   "pyproject.toml:version"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `yandil-0.2.4/src/yandil/configuration/configuration_container.py` & `yandil-0.3.0/src/yandil/configuration/configuration_container.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.4/src/yandil/container.py` & `yandil-0.3.0/src/yandil/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,26 +26,27 @@
 
 from yandil.argument import Argument
 from yandil.configuration.configuration_container import ConfigurationContainer, default_configuration_container
 from yandil.dependency import Dependency
 from yandil.errors.abstract_class_not_allowed_error import AbstractClassNotAllowedError
 from yandil.errors.configuration_value_type_mismatch_error import ConfigurationValueTypeMismatchError
 from yandil.errors.dependency_not_found_error import DependencyNotFoundError
+from yandil.errors.instance_and_class_does_not_match_error import InstanceAndClassDoesNotMatchError
 from yandil.errors.missing_configuration_value_error import MissingConfigurationValueError
 from yandil.errors.missing_type_hint_item_type_error import MissingTypeHintItemTypeError
 from yandil.errors.primary_dependency_already_defined_error import PrimaryDependencyAlreadyDefinedError
 from yandil.errors.primary_dependency_not_found_error import PrimaryDependencyNotFoundError
 from yandil.typing_tools import is_type_hint_iterable, str_to_builtin_type, type_hint_iterable_builder_factory
 
 DT = TypeVar("DT")
 
 
 class Container:
-    __EXCLUDED_BASES: Final[Set[str]] = {object}
-    __ABSTRACT_BASES: Final[Set[str]] = {Protocol, Generic, ABC}
+    __EXCLUDED_BASES: Final[Set[str]] = {object, Generic}
+    __ABSTRACT_BASES: Final[Set[str]] = {Protocol, ABC}
     __BUILTIN_TYPES: Final[Set[str]] = {int, float, str, bool, bytes, bytearray}
 
     def __init__(self, configuration_container: ConfigurationContainer):
         self.__dependency_map: Dict[Type, Dependency] = {}
         self.__bases_map: Dict[Type | GenericAlias, List[Type]] = defaultdict(list)
         self.__configuration_container = configuration_container
 
@@ -57,32 +58,34 @@
             return
 
         dependency = Dependency(cls, is_primary=is_primary)
 
         self.__update_bases_map(cls, is_primary)
         self.__dependency_map[cls] = dependency
 
+    def __is_abstract_class(self, cls: Type) -> bool:
+        for base in cls.__bases__:
+            if base in self.__ABSTRACT_BASES:
+                return True
+        return False
+
     def __setitem__(self, cls: Type[DT], value: DT) -> None:
-        if self.__is_abstract_class(cls):
-            cls = value.__class__
-            is_primary = True
-            dependency = Dependency(cls, value=value, is_resolved=True, is_primary=True)
-        else:
+        if cls == value.__class__:
             is_primary = None
             dependency = Dependency(cls, value=value, is_resolved=True)
+        elif isinstance(value, cls):
+            is_primary = self.__get_primary_dependency_from_base_children(self.__bases_map.get(cls, [])) is None
+            cls = value.__class__
+            dependency = Dependency(cls, value=value, is_resolved=True, is_primary=is_primary)
+        else:
+            raise InstanceAndClassDoesNotMatchError(value, cls)
 
         self.__update_bases_map(cls, is_primary)
         self.__dependency_map[cls] = dependency
 
-    def __is_abstract_class(self, cls: Type) -> bool:
-        for base in cls.__bases__:
-            if base in self.__ABSTRACT_BASES:
-                return True
-        return False
-
     def __update_bases_map(
         self,
         cls: Type,
         children_is_primary: Optional[bool],
         reference_class: Optional[Type] = None,
         reference_class_args: Optional[Tuple[Any]] = None,
     ) -> None:
```

### Comparing `yandil-0.2.4/src/yandil/declarative/decorators.py` & `yandil-0.3.0/src/yandil/declarative/decorators.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.4/src/yandil/dependency.py` & `yandil-0.3.0/src/yandil/dependency.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.4/src/yandil/dependency_filler.py` & `yandil-0.3.0/src/yandil/dependency_filler.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.4/src/yandil/discovery/class_discovery.py` & `yandil-0.3.0/src/yandil/discovery/class_discovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     for node in module_ast.body:
         if isinstance(node, ClassDef):
             yield node
 
 
 def exclude_abstract_classes(class_nodes: Iterable[ClassDef]) -> Iterable[ClassDef]:
-    abstract_bases = {"Protocol", "Generic", "ABC"}
+    abstract_bases = {"Protocol", "ABC"}
 
     def __is_abstract_class_node(node: ClassDef) -> bool:
         for base in node.bases:
             if isinstance(base, Name) and base.id in abstract_bases:
                 return True
 
             if isinstance(base, Subscript) and isinstance(base.value, Name) and base.value.id in abstract_bases:
```

### Comparing `yandil-0.2.4/src/yandil/discovery/module_discovery.py` & `yandil-0.3.0/src/yandil/discovery/module_discovery.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.4/src/yandil/loaders/declarative_dependency_loader.py` & `yandil-0.3.0/src/yandil/loaders/declarative_dependency_loader.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.4/src/yandil/loaders/self_discover_dependency_loader.py` & `yandil-0.3.0/src/yandil/loaders/self_discover_dependency_loader.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.4/src/yandil/typing_tools.py` & `yandil-0.3.0/src/yandil/typing_tools.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.4/PKG-INFO` & `yandil-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandil
-Version: 0.2.4
+Version: 0.3.0
 Summary: Yet ANother Dependency Injection Library
 Home-page: https://github.com/DeejayRevok/yandil
 License: BSD-3-Clause
 Keywords: dependency injection,di
 Author: DeejayRevok
 Author-email: seryi_one@hotmail.com
 Requires-Python: >=3.10.0,<3.11.0
```

