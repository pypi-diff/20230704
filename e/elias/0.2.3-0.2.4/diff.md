# Comparing `tmp/elias-0.2.3.tar.gz` & `tmp/elias-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Projects/elias/dist/.tmp-bvkk1f3m/elias-0.2.3.tar", last modified: Wed Jun 21 15:10:03 2023, max compression
+gzip compressed data, was "/mnt/d/Projects/elias/dist/.tmp-s9pdpkdk/elias-0.2.4.tar", last modified: Tue Jul  4 15:25:46 2023, max compression
```

## Comparing `elias-0.2.3.tar` & `elias-0.2.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 15:10:03.916242 elias-0.2.3/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.3/LICENSE
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-06-21 15:10:03.919085 elias-0.2.3/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1736 2022-04-27 09:37:39.000000 elias-0.2.3/README.md
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      110 2022-04-27 09:37:39.000000 elias-0.2.3/pyproject.toml
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      707 2023-06-21 15:10:03.932315 elias-0.2.3/setup.cfg
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       98 2022-04-27 09:37:39.000000 elias-0.2.3/setup.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 15:10:02.285404 elias-0.2.3/src/
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 15:10:02.472916 elias-0.2.3/src/elias/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    23125 2023-06-21 14:55:32.000000 elias-0.2.3/src/elias/config.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 15:10:02.894836 elias-0.2.3/src/elias/data/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/data/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8439 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/data/combined.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4507 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/data/loader.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4987 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/data/sampling.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1047 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/data/stop_criterion.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 15:10:03.160211 elias-0.2.3/src/elias/folder/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      156 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/folder/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1355 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/folder/analysis.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8126 2022-05-13 11:41:20.000000 elias-0.2.3/src/elias/folder/data.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13271 2022-12-23 10:38:59.000000 elias-0.2.3/src/elias/folder/folder.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1491 2022-12-23 10:15:28.000000 elias-0.2.3/src/elias/folder/model.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4983 2023-05-29 14:26:02.000000 elias-0.2.3/src/elias/folder/run.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 15:10:03.474347 elias-0.2.3/src/elias/manager/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      294 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/manager/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2705 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/manager/analysis.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1594 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/manager/artifact.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    12045 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/manager/buffered.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13104 2022-10-23 15:43:10.000000 elias-0.2.3/src/elias/manager/data.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22291 2022-12-23 10:55:00.000000 elias-0.2.3/src/elias/manager/model.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2918 2023-05-29 14:22:02.000000 elias-0.2.3/src/elias/manager/run.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 15:10:03.863406 elias-0.2.3/src/elias/util/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      361 2022-06-24 14:37:22.000000 elias-0.2.3/src/elias/util/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6870 2023-04-28 12:57:24.000000 elias-0.2.3/src/elias/util/fs.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     7919 2022-06-24 13:43:08.000000 elias-0.2.3/src/elias/util/io.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      333 2023-06-21 14:23:03.000000 elias-0.2.3/src/elias/util/random.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4690 2023-03-21 10:20:42.000000 elias-0.2.3/src/elias/util/range.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1248 2022-10-24 10:11:39.000000 elias-0.2.3/src/elias/util/timing.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      390 2023-05-26 09:28:39.000000 elias-0.2.3/src/elias/util/typing.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5512 2022-05-11 08:27:09.000000 elias-0.2.3/src/elias/util/version.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 15:10:02.662744 elias-0.2.3/src/elias.egg-info/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-06-21 15:10:01.000000 elias-0.2.3/src/elias.egg-info/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      948 2023-06-21 15:10:02.000000 elias-0.2.3/src/elias.egg-info/SOURCES.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-06-21 15:10:01.000000 elias-0.2.3/src/elias.egg-info/dependency_links.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      100 2023-06-21 15:10:01.000000 elias-0.2.3/src/elias.egg-info/requires.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        6 2023-06-21 15:10:01.000000 elias-0.2.3/src/elias.egg-info/top_level.txt
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:25:46.606339 elias-0.2.4/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.4/LICENSE
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-07-04 15:25:46.606339 elias-0.2.4/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1736 2022-04-27 09:37:39.000000 elias-0.2.4/README.md
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      110 2022-04-27 09:37:39.000000 elias-0.2.4/pyproject.toml
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      707 2023-07-04 15:25:46.616240 elias-0.2.4/setup.cfg
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       98 2022-04-27 09:37:39.000000 elias-0.2.4/setup.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:25:44.904023 elias-0.2.4/src/
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:25:45.100572 elias-0.2.4/src/elias/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.4/src/elias/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    24124 2023-07-04 15:24:59.000000 elias-0.2.4/src/elias/config.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:25:45.519401 elias-0.2.4/src/elias/data/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.4/src/elias/data/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8439 2022-04-27 09:37:39.000000 elias-0.2.4/src/elias/data/combined.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4507 2022-04-27 09:37:39.000000 elias-0.2.4/src/elias/data/loader.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4987 2022-04-27 09:37:39.000000 elias-0.2.4/src/elias/data/sampling.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1047 2022-04-27 09:37:39.000000 elias-0.2.4/src/elias/data/stop_criterion.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:25:45.820819 elias-0.2.4/src/elias/folder/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      156 2022-04-27 09:37:39.000000 elias-0.2.4/src/elias/folder/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1355 2022-04-27 09:37:39.000000 elias-0.2.4/src/elias/folder/analysis.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8126 2022-05-13 11:41:20.000000 elias-0.2.4/src/elias/folder/data.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13271 2022-12-23 10:38:59.000000 elias-0.2.4/src/elias/folder/folder.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1491 2022-12-23 10:15:28.000000 elias-0.2.4/src/elias/folder/model.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4983 2023-05-29 14:26:02.000000 elias-0.2.4/src/elias/folder/run.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:25:46.180691 elias-0.2.4/src/elias/manager/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      294 2022-04-27 09:37:39.000000 elias-0.2.4/src/elias/manager/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2705 2022-04-27 09:37:39.000000 elias-0.2.4/src/elias/manager/analysis.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1594 2022-04-27 09:37:39.000000 elias-0.2.4/src/elias/manager/artifact.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    12045 2022-04-27 09:37:39.000000 elias-0.2.4/src/elias/manager/buffered.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13104 2022-10-23 15:43:10.000000 elias-0.2.4/src/elias/manager/data.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22291 2022-12-23 10:55:00.000000 elias-0.2.4/src/elias/manager/model.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2918 2023-05-29 14:22:02.000000 elias-0.2.4/src/elias/manager/run.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:25:46.563223 elias-0.2.4/src/elias/util/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      361 2022-06-24 14:37:22.000000 elias-0.2.4/src/elias/util/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6870 2023-04-28 12:57:24.000000 elias-0.2.4/src/elias/util/fs.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     7919 2022-06-24 13:43:08.000000 elias-0.2.4/src/elias/util/io.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      333 2023-06-21 14:23:03.000000 elias-0.2.4/src/elias/util/random.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4690 2023-03-21 10:20:42.000000 elias-0.2.4/src/elias/util/range.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1248 2022-10-24 10:11:39.000000 elias-0.2.4/src/elias/util/timing.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1218 2023-07-04 15:24:59.000000 elias-0.2.4/src/elias/util/typing.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5512 2022-05-11 08:27:09.000000 elias-0.2.4/src/elias/util/version.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:25:45.282939 elias-0.2.4/src/elias.egg-info/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-07-04 15:25:44.000000 elias-0.2.4/src/elias.egg-info/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      948 2023-07-04 15:25:44.000000 elias-0.2.4/src/elias.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-07-04 15:25:44.000000 elias-0.2.4/src/elias.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      100 2023-07-04 15:25:44.000000 elias-0.2.4/src/elias.egg-info/requires.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        6 2023-07-04 15:25:44.000000 elias-0.2.4/src/elias.egg-info/top_level.txt
```

### Comparing `elias-0.2.3/PKG-INFO` & `elias-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elias
-Version: 0.2.3
+Version: 0.2.4
 Summary: ELIAS experiment library for facilitating machine learning projects
 Home-page: https://github.com/tobias-kirschstein/elias
 Author: Tobias Kirschstein
 Author-email: tobias.kirschstein@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `elias-0.2.3/README.md` & `elias-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/setup.cfg` & `elias-0.2.4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = elias
-version = 0.2.3
+version = 0.2.4
 author = Tobias Kirschstein
 author_email = tobias.kirschstein@gmail.com
 description = ELIAS experiment library for facilitating machine learning projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tobias-kirschstein/elias
 project_urls = 
@@ -19,15 +19,15 @@
 python_requires = >=3.6
 install_requires = 
 	dacite >= 1.6.0
 	pyyaml>=5.4.1
 	numpy>=1.20.2
 	testfixtures>=6.18.0
 	matplotlib>=3.4.2
-	silberstral>=0.2.1
+	silberstral>=0.2.3
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `elias-0.2.3/src/elias/config.py` & `elias-0.2.4/src/elias/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from __future__ import annotations
 
 import inspect
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, asdict, fields, field
 from enum import Enum, EnumMeta, auto
+from importlib import import_module
 from pydoc import locate
 from typing import List, Tuple, Any, Type, get_type_hints, Generic, TypeVar, Dict, Iterator, Callable, Optional
 
 import dacite
 import numpy as np
 from dacite import from_dict
 from dacite.dataclasses import get_fields
 from silberstral import gather_types, is_type_var_instantiated, reveal_type_var
 
 # TODO: Implement Dict or_else() method
 
 # =========================================================================
 # Better Enum handling for persistable config objects
 # =========================================================================
-
+from elias.util.typing import class_to_module_path, module_path_to_class
 
 _T_Enum = TypeVar('_T_Enum', bound=Enum)
 
 
 class NamedEnumMeta(EnumMeta):
     """
     Enum Meta to enable instantiating enums with their name as well.
@@ -116,14 +117,19 @@
                 # If a Config defines a member of type Dict it won't be unrolled by the dataclass asdict() method
                 # Hence, unroll it manually here. Enums are fine for both keys and values, but they have to be
                 # serialized
                 value = {
                     k.value if isinstance(k, Enum) else k:
                         v.value if isinstance(v, Enum) else v
                     for k, v in value.items()}
+            elif inspect.isclass(value) and key in config_fields and config_fields[key].type == Type:
+                # Handling for fields with type 'Type':
+                # represent the Type as a module import string, e.g., np.ndarray
+                value = class_to_module_path(value)
+
             # TODO: due to dacite we can only unpack numpy items at the outer level.
             #   dacite does iterate through nested configs of course, but here it does not give us access to the fields
             #   of the nested config...
             elif key in config_fields \
                     and (config_fields[key].type == float and (
                     isinstance(value, np.float32) or isinstance(value, np.float64))
                          or (config_fields[key].type == int and (
@@ -321,14 +327,15 @@
                 lambda abstract_dataclass_values, data_sub_class_type=data_sub_class_type:
                 instantiate_adc_with_sub_class(abstract_dataclass_values, data_sub_class_type)
             for abstract_dataclass, data_sub_class_type
             in zip(abstract_dataclasses, data_sub_class_types)}
 
         # Numpy arrays are serialized as lists. Cast them back to np array here
         all_type_hooks[np.ndarray] = lambda array_values: np.asarray(array_values)
+        all_type_hooks[Type] = module_path_to_class
 
         if type_hooks is not None:
             # Add use-defined type hooks
             all_type_hooks.update(type_hooks)
 
         # Register type hooks to replace every single AbstractDataClass with the respective subclass hinted by the
         # 'type' attribute
@@ -344,15 +351,28 @@
         #     # For some reason, __init__ isn't called anymore if __new__ is overridden. So manually call it here
         #     obj.__init__(*args, **kwargs)
         #     return obj
         #
         # backward_cls.__new__ = backward_compatibility_new
         # return from_dict(backward_cls, json_config, config=dacite_config)
         cls._backward_compatibility(json_config)
-        return from_dict(cls, json_config, config=dacite_config)
+        try:
+            config = from_dict(cls, json_config, config=dacite_config)
+        except IndexError as e:
+            type_hints = get_type_hints(cls)
+            if Type in type_hints.values():
+                # In case a field has type "Type" dacite unfortunately throws an unecessary error
+                # IndexError: tuple index out of range
+                # happening in types.py:129
+                dacite_config.check_types = False
+                config = from_dict(cls, json_config, config=dacite_config)
+            else:
+                raise e
+
+        return config
 
     @classmethod
     def from_dict(cls, values: dict):
         """
         Attempts to construct this Config by filling in the appropriate values from the specified :attr:`values`.
         Any excess items in the passed dictionary are ignored allowing to instantiate the Config dataclass with
         a bigger dictionary without having to hand-select the matching keys.
```

### Comparing `elias-0.2.3/src/elias/data/combined.py` & `elias-0.2.4/src/elias/data/combined.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/data/loader.py` & `elias-0.2.4/src/elias/data/loader.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/data/sampling.py` & `elias-0.2.4/src/elias/data/sampling.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/data/stop_criterion.py` & `elias-0.2.4/src/elias/data/stop_criterion.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/folder/analysis.py` & `elias-0.2.4/src/elias/folder/analysis.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/folder/data.py` & `elias-0.2.4/src/elias/folder/data.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/folder/folder.py` & `elias-0.2.4/src/elias/folder/folder.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/folder/model.py` & `elias-0.2.4/src/elias/folder/model.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/folder/run.py` & `elias-0.2.4/src/elias/folder/run.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/manager/analysis.py` & `elias-0.2.4/src/elias/manager/analysis.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/manager/artifact.py` & `elias-0.2.4/src/elias/manager/artifact.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/manager/buffered.py` & `elias-0.2.4/src/elias/manager/buffered.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/manager/data.py` & `elias-0.2.4/src/elias/manager/data.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/manager/model.py` & `elias-0.2.4/src/elias/manager/model.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/manager/run.py` & `elias-0.2.4/src/elias/manager/run.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/util/fs.py` & `elias-0.2.4/src/elias/util/fs.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/util/io.py` & `elias-0.2.4/src/elias/util/io.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/util/range.py` & `elias-0.2.4/src/elias/util/range.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/util/timing.py` & `elias-0.2.4/src/elias/util/timing.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias/util/version.py` & `elias-0.2.4/src/elias/util/version.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.3/src/elias.egg-info/PKG-INFO` & `elias-0.2.4/src/elias.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elias
-Version: 0.2.3
+Version: 0.2.4
 Summary: ELIAS experiment library for facilitating machine learning projects
 Home-page: https://github.com/tobias-kirschstein/elias
 Author: Tobias Kirschstein
 Author-email: tobias.kirschstein@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `elias-0.2.3/src/elias.egg-info/SOURCES.txt` & `elias-0.2.4/src/elias.egg-info/SOURCES.txt`

 * *Files identical despite different names*

