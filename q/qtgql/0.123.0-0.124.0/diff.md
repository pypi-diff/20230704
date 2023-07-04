# Comparing `tmp/qtgql-0.123.0.tar.gz` & `tmp/qtgql-0.124.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.123.0.tar", max compression
+gzip compressed data, was "qtgql-0.124.0.tar", max compression
```

## Comparing `qtgql-0.123.0.tar` & `qtgql-0.124.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1064 2023-07-02 14:25:50.094429 qtgql-0.123.0/LICENSE
--rw-r--r--   0        0        0     1055 2023-07-02 14:25:50.094429 qtgql-0.123.0/README.md
--rw-r--r--   0        0        0     4428 2023-07-02 14:26:10.810644 qtgql-0.123.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0     1919 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/config.py
--rw-r--r--   0        0        0        0 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/core/__init__.py
--rw-r--r--   0        0        0     1548 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/core/cppref.py
--rw-r--r--   0        0        0       41 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/core/exceptions.py
--rw-r--r--   0        0        0     3105 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/core/graphql_ref.py
--rw-r--r--   0        0        0     1179 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/core/template.py
--rw-r--r--   0        0        0     3226 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/generator.py
--rw-r--r--   0        0        0        0 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/operation/__init__.py
--rw-r--r--   0        0        0     4202 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/operation/definitions.py
--rw-r--r--   0        0        0    13608 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/operation/evaluation.py
--rw-r--r--   0        0        0      749 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/operation/template.py
--rw-r--r--   0        0        0        0 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/schema/__init__.py
--rw-r--r--   0        0        0     4164 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/schema/definitions.py
--rw-r--r--   0        0        0     8512 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/schema/evaluation.py
--rw-r--r--   0        0        0     1625 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/schema/template.py
--rw-r--r--   0        0        0      445 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0     1395 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
--rw-r--r--   0        0        0     3573 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     1849 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
--rw-r--r--   0        0        0      448 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
--rw-r--r--   0        0        0      994 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
--rw-r--r--   0        0        0     4174 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     2644 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
--rw-r--r--   0        0        0     3536 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/operation.jinja.cpp
--rw-r--r--   0        0        0     4664 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3532 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0    16979 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/types.py
--rw-r--r--   0        0        0     1151 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 qtgql-0.123.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-04 13:43:19.926438 qtgql-0.124.0/LICENSE
+-rw-r--r--   0        0        0     1055 2023-07-04 13:43:19.926438 qtgql-0.124.0/README.md
+-rw-r--r--   0        0        0     4428 2023-07-04 13:43:39.250570 qtgql-0.124.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     1939 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1548 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3091 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1179 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3226 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     3961 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    15274 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0      749 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     4164 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8512 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0      445 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1704 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     3573 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     1850 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0      448 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
+-rw-r--r--   0        0        0     1051 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     4641 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     2645 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
+-rw-r--r--   0        0        0     3884 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     4956 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3231 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    17078 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1147 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 qtgql-0.124.0/PKG-INFO
```

### Comparing `qtgql-0.123.0/LICENSE` & `qtgql-0.124.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.123.0/README.md` & `qtgql-0.124.0/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.123.0/pyproject.toml` & `qtgql-0.124.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.123.0"
+version = "0.124.0"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.123.0/qtgqlcodegen/cli.py` & `qtgql-0.124.0/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.123.0/qtgqlcodegen/config.py` & `qtgql-0.124.0/qtgqlcodegen/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import cached_property
 from pathlib import Path
 
 import graphql
-from attrs import define
+from attrs import Factory, define
 
 from qtgqlcodegen.generator import SchemaGenerator
 from qtgqlcodegen.schema.definitions import CustomScalarMap
 from qtgqlcodegen.types import CUSTOM_SCALARS
 
 
 @define(slots=False)
@@ -21,16 +21,16 @@
     - operations.graphql, queries, mutations and subscription handlers would be generated based on the operations defined there.
     """
     env_name: str = "QGqlEnv"
     """The generated types would find the environment by this name.
 
     Also the generated QML imports would fall under this namespace.
     """
-    custom_scalars: CustomScalarMap = {}
-    """mapping of custom scalars, respected by the schema evaluator."""
+    custom_scalars: CustomScalarMap = Factory(dict)
+    """Mapping of custom scalars, respected by the schema evaluator."""
     debug: bool = False
     """Templates would render some additional helpers for testing."""
 
     @cached_property
     def schema_path(self) -> Path:
         return self.graphql_dir / "schema.graphql"
```

### Comparing `qtgql-0.123.0/qtgqlcodegen/core/cppref.py` & `qtgql-0.124.0/qtgqlcodegen/core/cppref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.123.0/qtgqlcodegen/core/graphql_ref.py` & `qtgql-0.124.0/qtgqlcodegen/core/graphql_ref.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,18 +71,18 @@
 inject_typename_selection = inject_selection_factory(TYPENAME_SELECTION_NODE)
 
 
 def selection_set_search_factory(
     selection_name: str,
 ) -> Callable[[gql_lang.SelectionSetNode], bool]:
     def factory(selection_set: gql_lang.SelectionSetNode):
-        for field in selection_set.selections:
-            assert isinstance(field, gql_lang.FieldNode), f"{field} is not a field"
-            if field.name.value == selection_name:
-                return True
+        for field_or_frag in selection_set.selections:
+            if field := is_field_node(field_or_frag):
+                if field.name.value == selection_name:
+                    return True
         return False
 
     return factory
 
 
 has_id_selection = selection_set_search_factory("id")
 has_typename_selection = selection_set_search_factory("__typename")
```

### Comparing `qtgql-0.123.0/qtgqlcodegen/core/template.py` & `qtgql-0.124.0/qtgqlcodegen/core/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.123.0/qtgqlcodegen/generator.py` & `qtgql-0.124.0/qtgqlcodegen/generator.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.123.0/qtgqlcodegen/operation/definitions.py` & `qtgql-0.124.0/qtgqlcodegen/operation/definitions.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,21 +48,14 @@
 
     @cached_property
     def is_root(self) -> bool:
         return self.origin.name in self.type_info.schema_type_info.root_types_names
 
     @cached_property
     def type_name(self) -> str:
-        if self.type.is_object_type:
-            return self.type.type_name()
-
-        if model_of := self.type.is_model:
-            if model_of.is_object_type:
-                return f"qtgql::bases::ListModelABC<{self.type.type_name()}>"
-
         return self.type.member_type
 
     @cached_property
     def property_type(self) -> str:
         """
 
         :return: C++ property type that will be exposed to QML.
```

### Comparing `qtgql-0.123.0/qtgqlcodegen/operation/evaluation.py` & `qtgql-0.124.0/qtgqlcodegen/operation/evaluation.py`

 * *Files 4% similar despite different names*

```diff
@@ -222,71 +222,121 @@
 
     return QtGqlQueriedUnion(
         concrete=concrete,
         choices=choices,
     )
 
 
+def _unwrap_interface_fragments(
+    type_info: SchemaTypeInfo,
+    parent_concrete: QtGqlObjectType | QtGqlInterface,
+    selection_set: gql_lang.SelectionSetNode,
+    initial: dict[str, list[gql_lang.FieldNode]],
+    id_was_selected: bool = False,
+) -> dict[str, list[gql_lang.FieldNode]]:
+    """Fragments can be nested, i.e node{ id.
+
+        ...on SomeFrag{
+            field1
+            ...on Obj{
+                name
+            }
+        }
+    }
+    :returns: all of the inline fragments as a flat list.
+    """
+    fields_for_concrete: list[gql_lang.FieldNode] = []
+    if not has_id_selection(selection_set) and not id_was_selected:
+        id_was_selected = True
+        inject_id_selection(selection_set)
+    for field_or_frag in selection_set.selections:
+        if inline_frag := is_inline_fragment(field_or_frag):
+            type_name = inline_frag.type_condition.name.value
+            # no need to validate inner types are implementation, graphql-core does this.
+            concrete_choice = type_info.get_object_type(
+                type_name,
+            ) or type_info.get_interface(type_name)
+            assert concrete_choice
+            _unwrap_interface_fragments(
+                type_info,
+                concrete_choice,
+                inline_frag.selection_set,
+                initial,
+                id_was_selected,
+            )
+        else:
+            field_node = is_field_node(field_or_frag)
+            assert field_node
+            if field_node.name.value != "__typename":
+                fields_for_concrete.append(field_node)
+
+    initial[parent_concrete.name] = fields_for_concrete
+    return initial
+
+
 def _evaluate_interface(
     type_info: OperationTypeInfo,
     concrete: QtGqlInterface,
     selection_set: gql_lang.SelectionSetNode,
     path: str,  # current path in the query tree.
 ) -> QtGqlQueriedInterface:
     choices: list[QtGqlQueriedObjectType] = []
 
-    # first get all linear selections, these are selection that can be applied to
-    # any of the interface implementors
-    inline_fragments: list[gql_lang.InlineFragmentNode] = []
-    linear_fields: dict[str, QtGqlQueriedField] = {}
-    for field_or_frag in selection_set.selections:
-        if inline_frag := is_inline_fragment(field_or_frag):
-            inline_fragments.append(inline_frag)
-        else:
-            field_node = is_field_node(field_or_frag)
-            assert field_node
-            __f = _evaluate_field(
-                type_info=type_info,
-                concrete_field=concrete.fields_dict[field_node.name.value],
-                field_node=field_node,
-                path=path,
-                origin=concrete,
+    raw_fields_map = _unwrap_interface_fragments(
+        type_info.schema_type_info,
+        concrete,
+        selection_set,
+        {},
+    )
+    # dispatch fragmented fields where they are needed.
+    for resolve_able in concrete.implementations.values():
+        if concrete_choice := resolve_able.is_object_type:
+            fields_for_obj = []
+            # collect fields from bases.
+            for base in concrete_choice.interfaces_raw:
+                if fields_for_base := raw_fields_map.get(base.name, None):
+                    fields_for_obj.extend(fields_for_base)
+
+            # append fields of the choice itself
+            if choice_fields := raw_fields_map.get(concrete_choice.name, None):
+                fields_for_obj.extend(choice_fields)
+            ss = gql_lang.SelectionSetNode(selections=tuple(fields_for_obj))
+            choices.append(
+                # This could probably be more optimized though, currently
+                # this would suffice to reduce complexity.
+                _evaluate_object_type(
+                    type_info=type_info,
+                    concrete=concrete_choice,
+                    selection_set=ss,
+                    path=path,
+                ),
             )
-            linear_fields[__f.name] = __f
-    # evaluate type conditions
-    for inline_frag in inline_fragments:
-        type_name = inline_frag.type_condition.name.value
-        # no need to validate inner types are implementation, graphql-core does this.
-        concrete_choice = type_info.schema_type_info.get_object_type(
-            type_name,
-        ) or type_info.schema_type_info.get_interface(type_name)
-        assert concrete_choice
-        choices.append(
-            _evaluate_object_type(
-                type_info=type_info,
-                concrete=concrete_choice,
-                selection_set=inline_frag.selection_set,
-                path=path,
-            ),
-        )
 
-        # inject __type_name selection, we'll use this to deserialize correctly.
-        if not has_typename_selection(inline_frag.selection_set):
-            inject_typename_selection(inline_frag.selection_set)
+    # inject __type_name selection, we'll use this to deserialize correctly.
+    if not has_typename_selection(selection_set):
+        inject_typename_selection(selection_set)
 
     name = f"{concrete.name}__{path}"
     ret = QtGqlQueriedInterface(
         name=name,
         concrete=concrete,
         choices=choices,
-        fields_dict=linear_fields,
+        fields_dict={
+            field.name.value: _evaluate_field(
+                type_info=type_info,
+                concrete_field=concrete.fields_dict[field.name.value],
+                path=path,
+                field_node=field,
+                origin=concrete,
+            )
+            for field in raw_fields_map[concrete.name]
+        },
     )
     for choice in choices:
         choice.base_interface = ret
-        choice.fields_dict.update(linear_fields)
     type_info.narrowed_interfaces_map[name] = ret
     return ret
 
 
 def _evaluate_object_type(
     type_info: OperationTypeInfo,
     concrete: QtGqlObjectType,
@@ -297,15 +347,15 @@
     if concrete.implements_node and not has_id_selection(selection_set):
         inject_id_selection(selection_set)
 
     fields: dict[str, QtGqlQueriedField] = {}
     for selection in selection_set.selections:
         if f_node := is_field_node(selection):
             if is_type_name_selection(f_node):
-                continue  # __type_name selection is handled with special care.
+                continue  # __typename selection is handled with special care.
             concrete_field = concrete.fields_dict[f_node.name.value]
             fields[concrete_field.name] = _evaluate_field(
                 type_info=type_info,
                 concrete_field=concrete_field,
                 field_node=f_node,
                 path=path,
                 origin=concrete,
```

### Comparing `qtgql-0.123.0/qtgqlcodegen/operation/template.py` & `qtgql-0.124.0/qtgqlcodegen/operation/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.123.0/qtgqlcodegen/schema/definitions.py` & `qtgql-0.124.0/qtgqlcodegen/schema/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.123.0/qtgqlcodegen/schema/evaluation.py` & `qtgql-0.124.0/qtgqlcodegen/schema/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.123.0/qtgqlcodegen/schema/template.py` & `qtgql-0.124.0/qtgqlcodegen/schema/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.123.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp` & `qtgql-0.124.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.123.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp` & `qtgql-0.124.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 auto init_list_👉 field.name 👈 =  std::make_unique<QList<👉field.type.of_type.name👈*>>();
 for (const auto & node: 👉 instance_of_concrete 👈){
 init_list_👉 field.name 👈->append(new 👉field.type.of_type.name👈(👉operation_pointer👈, node));
 }
 👉field.private_name👈 = new qtgql::bases::ListModelABC<👉 field.type.of_type.name 👈>(this, std::move(init_list_👉 field.name 👈));
 {% elif field.type.is_queried_interface %}
 auto concrete_👉field.name👈 = 👉 instance_of_concrete 👈;
-auto 👉field.name👈_typename = concrete_👉field.name👈->TYPE_NAME();
+auto 👉field.name👈_typename = concrete_👉field.name👈->__typename();
 {%set type_cond -%}👉field.name👈_typename{% endset -%}
 {% for choice in field.type.choices -%}
 {% set do_on_meets -%}
 👉field.private_name👈 = qobject_cast<👉 field.type.name 👈*>(new 👉choice.type_name()👈(👉operation_pointer👈, std::static_pointer_cast<👉 choice.concrete.name 👈>(concrete_👉field.name👈)));
 {% endset -%}
 👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
 {% endfor %}
```

### Comparing `qtgql-0.123.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp` & `qtgql-0.124.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 {% macro proxy_type_fields(t, context) -%}
 Q_OBJECT
+Q_PROPERTY(QString  __typeName READ __typename CONSTANT)
 
 {% for f in t.fields -%}
 Q_PROPERTY(const 👉 f.property_type 👈 👉 f.name 👈 READ 👉 f.concrete.getter_name 👈 NOTIFY 👉 f.concrete.signal_name 👈);
 {% endfor %}
 signals:
 {%for f in t.fields -%}
 void 👉 f.concrete.signal_name 👈();
```

### Comparing `qtgql-0.123.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp` & `qtgql-0.124.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -68,15 +68,24 @@
 }
 {% elif proxy_field.type.is_queried_interface %}
 auto 👉f_concrete.name👈_data = data.value("👉f_concrete.name👈").toObject();
 auto 👉f_concrete.name👈_typename  = 👉f_concrete.name👈_data.value("__typename").toString();
 {%set type_cond -%}👉f_concrete.name👈_typename{% endset -%}
 {% for choice in proxy_field.type.choices %}
 {% set do_on_meets -%}
+{% if choice.implements_node %}
+if (👉current👈 && 👉current👈->get_id() == 👉f_concrete.name👈_data.value("id").toString()){
 👉choice.updater_name👈(std::static_pointer_cast<👉choice.concrete.name👈>(👉current👈), 👉f_concrete.name👈_data,  👉operation_pointer👈);
+}
+else{
+👉 setter_name 👈(👉choice.deserializer_name👈(👉proxy_field.name👈_data, 👉operation_pointer👈) 👉 setter_end 👈);
+}
+{% else %}
+👉choice.updater_name👈(std::static_pointer_cast<👉choice.concrete.name👈>(👉current👈), 👉f_concrete.name👈_data,  👉operation_pointer👈);
+{% endif %}
 {% endset -%}
 👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
 {% endfor %}
 {% else %}
 throw qtgql::exceptions::NotImplementedError({"👉proxy_field.type.__class__.__name__👈 is not supporting updates ATM"});
 {% endif %}
 }
```

### Comparing `qtgql-0.123.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp` & `qtgql-0.124.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 delete 👉field.private_name👈;
 👉field.private_name👈 = new 👉field.type.name👈(operation, concrete);
 emit 👉 field.concrete.signal_name 👈();
 {% elif field.type.is_queried_interface -%}
 auto operation = qobject_cast<👉operation.name👈*>(this->parent());
 auto concrete = 👉new_concrete👈;
 delete 👉field.private_name👈;
-auto 👉field.name👈_typename = concrete->TYPE_NAME();
+auto 👉field.name👈_typename = concrete->__typename();
 {%set type_cond -%}👉field.name👈_typename{% endset -%}
 {% for choice in field.type.choices %}
 {% set do_on_meets -%}
 👉field.private_name👈 = qobject_cast<const 👉field.type.name👈 *>(new 👉choice.name👈(operation, std::static_pointer_cast<👉choice.concrete.name👈>(concrete)));
 {% endset -%}
 👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
 {% endfor %}
```

### Comparing `qtgql-0.123.0/qtgqlcodegen/templates/operation.jinja.cpp` & `qtgql-0.124.0/qtgqlcodegen/templates/operation.jinja.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,22 @@
 
 // Interfaces
 {% for interface in context.operation.interfaces -%}
 std::shared_ptr<👉 interface.concrete.name 👈> 👉 interface.deserializer_name 👈(const QJsonObject& data, const 👉 context.operation.name 👈 * operation){
 auto type_name = data.value("__typename").toString();
 {% for choice in interface.choices -%}
 {% set do_on_meets -%}
+{% if interface.concrete.implements_node %}
+auto cached_maybe = 👉 interface.concrete.name 👈::get_node(data.value("id").toString());
+if(cached_maybe.has_value()){
+auto node = cached_maybe.value();
+👉 interface.updater_name 👈(node, data, operation);
+return std::static_pointer_cast<👉 interface.concrete.name 👈>(node);
+}
+{% endif -%}
 return std::static_pointer_cast<👉 interface.concrete.name 👈>(👉 choice.deserializer_name 👈(data, operation));
 {% endset -%}
 👉iterate_type_condition(choice,"type_name", do_on_meets, loop)👈
 {% endfor -%}
 throw qtgql::exceptions::InterfaceDeserializationError(type_name.toStdString());
 }
 {% endfor %}
```

### Comparing `qtgql-0.123.0/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.124.0/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 public:
     using QObject::QObject;
 {% for f in t.fields -%}
 [[nodiscard]] inline virtual const 👉 f.property_type 👈  👉 f.concrete.getter_name 👈() const {
 throw qtgql::exceptions::InterfaceDirectAccessError("👉t.concrete.name👈");
 }
 {% endfor %}
+public:
+[[nodiscard]] virtual const QString & __typename() const{
+    throw qtgql::exceptions::InterfaceDirectAccessError("👉t.concrete.name👈");
+}
 };
 {% endfor %}
 // ------------ Narrowed Object types ------------
 {% for t in context.operation.narrowed_types %}
 class 👉 t.name 👈: public 👉 "QObject" if not t.base_interface else t.base_interface.name 👈{
 👉 proxy_type_fields(t, context) 👈
 public:
@@ -52,31 +56,33 @@
 {%- if f.type.is_queried_object_type or f.type.is_model or f.type.is_queried_interface %}
 return m_👉f.name👈;
 {%- else -%}
 return m_inst->👉 f.concrete.getter_name 👈();
 {%- endif -%}
 };
 {% endfor -%}
-
+public:
+[[nodiscard]] const QString & __typename() const {% if t.base_interface -%}final{% endif %}{
+    return m_inst->__typename();
+}
 };
 {% endfor %}
 
 struct 👉 context.operation.generated_variables_type 👈{
 {% for var in context.operation.variables -%}
 std::optional<👉 var.type.member_type 👈> 👉 var.name 👈 = {};
 {% endfor -%}
-
     QJsonObject to_json() const{
-    QJsonObject ret;
+    QJsonObject __ret;
     {% for var in context.operation.variables -%}
     if (👉 var.name 👈.has_value()){
-    ret.insert("👉 var.name 👈",  👉 var.json_repr() 👈);
+    __ret.insert("👉 var.name 👈",  👉 var.json_repr() 👈);
     }
     {% endfor -%}
-    return ret;
+    return __ret;
     }
 };
 
 class 👉 context.operation.name 👈: public qtgql::gqlwstransport::OperationHandlerABC{
     Q_OBJECT
 Q_PROPERTY(const 👉 context.operation.root_type.name 👈 * data READ data NOTIFY dataChanged);
```

### Comparing `qtgql-0.123.0/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.124.0/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -107,25 +107,16 @@
 }
 {% else %}
 QTGQL_STATIC_MAKE_SHARED(👉 type.name 👈)
 {% endif %}
 
 👉 type.name 👈()= default;
 
-inline const QString & TYPE_NAME() final{
-    static const QString ret = "👉 type.name 👈";
-    return ret;
+public:
+inline const QString & __typename() final{
+static const QString ret = "👉 type.name 👈";
+return ret;
 };
-
-{% if type.implements_node -%}
-static std::optional<std::shared_ptr<👉 type.name 👈>> get_node(const QString & id){
-    auto node = ENV_CACHE()->get_node(id);
-    if (node.has_value()){
-        return std::static_pointer_cast<👉 type.name 👈>(node.value());
-    }
-    return {};
-}
-{% endif %}
 };
 {% endfor %}
 
 }
```

### Comparing `qtgql-0.123.0/qtgqlcodegen/types.py` & `qtgql-0.124.0/qtgqlcodegen/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,15 +387,15 @@
 
     def json_repr(self, attr_name: str | None = None) -> str:
         return f"{attr_name}.to_json()"
 
 
 @define
 class EnumValue:
-    """encapsulates enumValues from introspection, maps to an Enum member."""
+    """Encapsulates enumValues from introspection, maps to an Enum member."""
 
     name: str
     index: int
     description: str = ""
 
 
 @define(slots=False)
@@ -435,14 +435,18 @@
 class QtGqlQueriedObjectType(QtGqlQueriedTypeABC, QtGqlTypeABC):
     name: str
     concrete: QtGqlObjectType
     fields_dict: dict[str, QtGqlQueriedField] = attrs.Factory(dict)
     base_interface: QtGqlQueriedInterface | None = None  # I think that there could be only one
 
     @property
+    def implements_node(self) -> bool:
+        return self.concrete.implements_node
+
+    @property
     def is_queried_object_type(self) -> QtGqlQueriedObjectType | None:
         return self
 
     @cached_property
     def fields(self) -> tuple[QtGqlQueriedField, ...]:
         return tuple(self.fields_dict.values())
```

### Comparing `qtgql-0.123.0/qtgqlcodegen/utils.py` & `qtgql-0.124.0/qtgqlcodegen/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,20 +14,20 @@
     content: str
 
     def dump(self) -> None:
         self.path.write_text(self.content)
 
 
 class AntiForwardRef:
-    """
-    i.e:
-    Union["someString"] would return a ForwardRef, this class is a simple hack
-    to just return a type contains the name.
-    Also, this is a workaround for types that reference each-other,
-    otherwise it would cause recursion error.
+    """i.e:
+
+    Union["someString"] would return a ForwardRef, this class is a
+    simple hack to just return a type contains the name. Also, this is a
+    workaround for types that reference each-other, otherwise it would
+    cause recursion error.
     """
 
     name: str
     type_map: dict
 
     @classmethod
     def resolve(cls) -> Any:
```

### Comparing `qtgql-0.123.0/PKG-INFO` & `qtgql-0.124.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.123.0
+Version: 0.124.0
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
```

