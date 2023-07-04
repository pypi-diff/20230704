# Comparing `tmp/silberstral-0.2.2.tar.gz` & `tmp/silberstral-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Projects/silberstral/dist/.tmp-e0bq4kvn/silberstral-0.2.2.tar", last modified: Fri Feb 24 12:52:31 2023, max compression
+gzip compressed data, was "/mnt/d/Projects/silberstral/dist/.tmp-kc1_u3aq/silberstral-0.2.3.tar", last modified: Tue Jul  4 15:17:40 2023, max compression
```

## Comparing `silberstral-0.2.2.tar` & `silberstral-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-24 12:52:31.000000 silberstral-0.2.2/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1094 2022-04-27 09:37:20.000000 silberstral-0.2.2/LICENSE.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3588 2023-02-24 12:52:31.000000 silberstral-0.2.2/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2871 2022-04-27 09:37:20.000000 silberstral-0.2.2/README.md
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      108 2022-04-27 09:37:20.000000 silberstral-0.2.2/pyproject.toml
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      999 2023-02-24 12:52:31.000000 silberstral-0.2.2/setup.cfg
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       96 2022-04-27 09:37:20.000000 silberstral-0.2.2/setup.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-24 12:52:30.000000 silberstral-0.2.2/src/
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-24 12:52:30.000000 silberstral-0.2.2/src/silberstral/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      137 2022-04-27 09:37:20.000000 silberstral-0.2.2/src/silberstral/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    18319 2023-02-23 09:52:05.000000 silberstral-0.2.2/src/silberstral/silberstral.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-24 12:52:30.000000 silberstral-0.2.2/src/silberstral.egg-info/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3588 2023-02-24 12:52:30.000000 silberstral-0.2.2/src/silberstral.egg-info/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      333 2023-02-24 12:52:30.000000 silberstral-0.2.2/src/silberstral.egg-info/SOURCES.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-02-24 12:52:30.000000 silberstral-0.2.2/src/silberstral.egg-info/dependency_links.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       22 2023-02-24 12:52:30.000000 silberstral-0.2.2/src/silberstral.egg-info/requires.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       12 2023-02-24 12:52:30.000000 silberstral-0.2.2/src/silberstral.egg-info/top_level.txt
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-24 12:52:31.000000 silberstral-0.2.2/test/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    15596 2023-01-13 13:55:26.000000 silberstral-0.2.2/test/test_silberstral.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:17:40.516766 silberstral-0.2.3/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1094 2022-04-27 09:37:20.000000 silberstral-0.2.3/LICENSE.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3588 2023-07-04 15:17:40.526760 silberstral-0.2.3/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2871 2022-04-27 09:37:20.000000 silberstral-0.2.3/README.md
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      108 2022-04-27 09:37:20.000000 silberstral-0.2.3/pyproject.toml
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      999 2023-07-04 15:17:40.531534 silberstral-0.2.3/setup.cfg
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       96 2022-04-27 09:37:20.000000 silberstral-0.2.3/setup.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:17:40.132516 silberstral-0.2.3/src/
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:17:40.291452 silberstral-0.2.3/src/silberstral/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      137 2022-04-27 09:37:20.000000 silberstral-0.2.3/src/silberstral/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    19092 2023-07-04 15:11:08.000000 silberstral-0.2.3/src/silberstral/silberstral.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:17:40.467785 silberstral-0.2.3/src/silberstral.egg-info/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3588 2023-07-04 15:17:39.000000 silberstral-0.2.3/src/silberstral.egg-info/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      333 2023-07-04 15:17:40.000000 silberstral-0.2.3/src/silberstral.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-07-04 15:17:39.000000 silberstral-0.2.3/src/silberstral.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       22 2023-07-04 15:17:39.000000 silberstral-0.2.3/src/silberstral.egg-info/requires.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       12 2023-07-04 15:17:39.000000 silberstral-0.2.3/src/silberstral.egg-info/top_level.txt
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:17:40.498507 silberstral-0.2.3/test/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    15813 2023-07-04 15:16:18.000000 silberstral-0.2.3/test/test_silberstral.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `silberstral-0.2.2/LICENSE.txt` & `silberstral-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `silberstral-0.2.2/PKG-INFO` & `silberstral-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silberstral
-Version: 0.2.2
+Version: 0.2.3
 Summary: Reveals the true shape of type vars
 Home-page: https://github.com/tobias-kirschstein/silberstral
 Author: Tobias Kirschstein
 Author-email: tobias.kirschstein@gmail.com
 License: MIT
 Keywords: typing,type var,instantiation,generics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `silberstral-0.2.2/README.md` & `silberstral-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `silberstral-0.2.2/setup.cfg` & `silberstral-0.2.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = silberstral
-version = 0.2.2
+version = 0.2.3
 author = Tobias Kirschstein
 author_email = tobias.kirschstein@gmail.com
 description = Reveals the true shape of type vars
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 url = https://github.com/tobias-kirschstein/silberstral
```

### Comparing `silberstral-0.2.2/src/silberstral/silberstral.py` & `silberstral-0.2.3/src/silberstral/silberstral.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,30 +225,42 @@
 
     # Ensure that types is iterable
     # TODO: is_generic_collection(types) fails with "unhashable type: 'list'" for dacite > 1.7.0
     if is_generic_collection(types) or is_generic(types) or isclass(types):
         types = [types]
 
     all_types = set()
+    _gather_types_recursive(types, all_types, parent_type=parent_type)
+    return all_types
+
+
+def _gather_types_recursive(types: Union[Iterable[Type], Type],
+                            collected_types: Set[Type],
+                            parent_type: Optional[Type] = None,
+                            ):
     for t in types:
         # t = t if inspect.isclass(t) else type(t)  # Ensure that passed value is a class
         # TODO: wrt parent_type: maybe we don't want to allow GenericAliases in dataclasses?
         if is_generic_collection(t) or is_union(t):
-            all_types.update(gather_types(extract_generic(t), parent_type))
+            extracted_types = set(extract_generic(t))
+            extracted_types.difference_update(collected_types)
+            _gather_types_recursive(extracted_types, collected_types, parent_type=parent_type)
         elif is_dataclass(t):
             # TODO: Could get some infinite recursion here. Maybe track visited types?
             field_types = get_type_hints(t).values()
-            all_types.update(gather_types(field_types, t))
-            all_types.add(t)
+            field_types = set(field_types)
+            field_types.difference_update(collected_types)
+            collected_types.add(t)  # For dataclasses, also add the type of the dataclass, not only the containing types
+            # Important that t is first added to collected_types. Otherwise, we might get infinite recursion
+            _gather_types_recursive(field_types, collected_types, parent_type=t)
         elif isinstance(t, TypeVar):
             t = reveal_type_var(parent_type, t)
-            all_types.add(t)
+            collected_types.add(t)
         else:
-            all_types.add(t)
-    return all_types
+            collected_types.add(t)
 
 
 def save_instantiate(cls_generic: _GenericAlias, *args, **kwargs) -> object:
     """
     Handles the rare use-case that one wants to instantiate a generic class without subclassing.
     In this case, Python's default way of instantiating generic classes prohibits the use of `reveal_type_var()` in
     the constructor.
```

### Comparing `silberstral-0.2.2/src/silberstral.egg-info/PKG-INFO` & `silberstral-0.2.3/src/silberstral.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silberstral
-Version: 0.2.2
+Version: 0.2.3
 Summary: Reveals the true shape of type vars
 Home-page: https://github.com/tobias-kirschstein/silberstral
 Author: Tobias Kirschstein
 Author-email: tobias.kirschstein@gmail.com
 License: MIT
 Keywords: typing,type var,instantiation,generics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `silberstral-0.2.2/test/test_silberstral.py` & `silberstral-0.2.3/test/test_silberstral.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 from dataclasses import dataclass
 from typing import TypeVar, Generic, Iterable, Iterator, T_co, Container, Collection, List, Deque, Set, Dict, Generator, \
-    T, KT, VT, T_contra, V_co, Union
+    T, KT, VT, T_contra, V_co, Union, Optional
 from unittest import TestCase
 
 from silberstral import reveal_type_var, get_origin, gather_types, reveal_type_vars, save_instantiate
 from silberstral.silberstral import create_linked_type_var
 
 _T1 = TypeVar('_T1')
 _T2 = TypeVar('_T2')
@@ -275,14 +275,20 @@
 
 @dataclass
 class DataclassWithUnionIntFloatAndString:
     a: Union[int, float]
     b: str
 
 
+@dataclass
+class RecursiveDataclass:
+    a: str
+    nested: Optional['RecursiveDataclass'] = None
+
+
 # =========================================================================
 # Actual Tests
 # =========================================================================
 
 class GenericTest(TestCase):
 
     def test_reveal_type_var(self):
@@ -403,11 +409,13 @@
 
         # Currently, type vars instantiated through subclassing will NOT be listed
         self.assertEqual(gather_types(TypeVar2Super11Level2), {TypeVar2Super11Level2})
 
         self.assertEqual(gather_types(DataclassWithUnionIntFloatAndString),
                          {DataclassWithUnionIntFloatAndString, int, float, str})
 
+        self.assertEqual(gather_types(RecursiveDataclass), {str, RecursiveDataclass, type(None)})
+
     def test_override_type_var_middle_class(self):
         obj: MiddleClass1TypeVarBConstructor = save_instantiate(MiddleClass1TypeVarBConstructor[Value1])
         self.assertEqual(obj.cls_T1, Value1)
         self.assertEqual(obj.cls_T2, Value1)
```

