# Comparing `tmp/rdfdf-0.1.4.tar.gz` & `tmp/rdfdf-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfdf-0.1.4.tar", max compression
+gzip compressed data, was "rdfdf-0.1.5.tar", max compression
```

## Comparing `rdfdf-0.1.4.tar` & `rdfdf-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-05-08 07:12:58.000000 rdfdf-0.1.4/LICENSE
--rw-r--r--   0        0        0     8588 2023-05-24 07:20:23.215813 rdfdf-0.1.4/README.md
--rw-r--r--   0        0        0      459 2023-06-29 06:44:12.207413 rdfdf-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 10:17:54.081795 rdfdf-0.1.4/rdfdf/__init__.py
--rw-r--r--   0        0        0      918 2023-05-15 09:40:40.000000 rdfdf-0.1.4/rdfdf/examples/example_1.py
--rw-r--r--   0        0        0     1154 2023-05-15 09:40:40.000000 rdfdf-0.1.4/rdfdf/examples/example_2.py
--rw-r--r--   0        0        0     1517 2023-05-15 09:40:40.000000 rdfdf-0.1.4/rdfdf/examples/example_3.py
--rw-r--r--   0        0        0     1373 2023-05-15 09:40:40.000000 rdfdf-0.1.4/rdfdf/examples/example_4.py
--rw-r--r--   0        0        0        0 2023-05-23 08:11:06.000000 rdfdf-0.1.4/rdfdf/helpers/__init__.py
--rw-r--r--   0        0        0     1323 2023-06-20 14:36:07.751495 rdfdf-0.1.4/rdfdf/helpers/importers.py
--rw-r--r--   0        0        0      969 2023-05-22 07:07:02.000000 rdfdf-0.1.4/rdfdf/helpers/rdfdf_utils.py
--rw-r--r--   0        0        0     4087 2023-06-29 06:34:43.690379 rdfdf-0.1.4/rdfdf/rdfdf.py
--rw-r--r--   0        0        0     9145 1970-01-01 00:00:00.000000 rdfdf-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-08 07:12:58.000000 rdfdf-0.1.5/LICENSE
+-rw-r--r--   0        0        0     8674 2023-06-29 06:45:26.524130 rdfdf-0.1.5/README.md
+-rw-r--r--   0        0        0      459 2023-07-04 12:55:48.452775 rdfdf-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 10:17:54.081795 rdfdf-0.1.5/rdfdf/__init__.py
+-rw-r--r--   0        0        0      918 2023-05-15 09:40:40.000000 rdfdf-0.1.5/rdfdf/examples/example_1.py
+-rw-r--r--   0        0        0     1154 2023-05-15 09:40:40.000000 rdfdf-0.1.5/rdfdf/examples/example_2.py
+-rw-r--r--   0        0        0     1517 2023-05-15 09:40:40.000000 rdfdf-0.1.5/rdfdf/examples/example_3.py
+-rw-r--r--   0        0        0     1373 2023-05-15 09:40:40.000000 rdfdf-0.1.5/rdfdf/examples/example_4.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:11:06.000000 rdfdf-0.1.5/rdfdf/helpers/__init__.py
+-rw-r--r--   0        0        0     1323 2023-06-20 14:36:07.751495 rdfdf-0.1.5/rdfdf/helpers/importers.py
+-rw-r--r--   0        0        0      969 2023-05-22 07:07:02.000000 rdfdf-0.1.5/rdfdf/helpers/rdfdf_utils.py
+-rw-r--r--   0        0        0     4234 2023-07-04 12:55:12.926009 rdfdf-0.1.5/rdfdf/rdfdf.py
+-rw-r--r--   0        0        0     9231 1970-01-01 00:00:00.000000 rdfdf-0.1.5/PKG-INFO
```

### Comparing `rdfdf-0.1.4/LICENSE` & `rdfdf-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.4/README.md` & `rdfdf-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 # rdfdf
 ![pipeline status](https://gitlab.com/lupl/rdfdf/badges/dev/pipeline.svg)
+[![PyPI version](https://badge.fury.io/py/rdfdf.svg)](https://badge.fury.io/py/rdfdf)
 
 rdfdf - Functionality for rule-based `pandas.DataFrame` - `rdflib.Graph` conversion.
 
 For representation of tabular data in RDF see Allemang, Hendler: Semantic Web for the Working Ontologist. 2011, 40ff.
 
 > This project is in an early stage of development and should be used with caution.
```

### Comparing `rdfdf-0.1.4/rdfdf/examples/example_1.py` & `rdfdf-0.1.5/rdfdf/examples/example_1.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.4/rdfdf/examples/example_2.py` & `rdfdf-0.1.5/rdfdf/examples/example_2.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.4/rdfdf/examples/example_3.py` & `rdfdf-0.1.5/rdfdf/examples/example_3.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.4/rdfdf/examples/example_4.py` & `rdfdf-0.1.5/rdfdf/examples/example_4.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.4/rdfdf/helpers/importers.py` & `rdfdf-0.1.5/rdfdf/helpers/importers.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.4/rdfdf/helpers/rdfdf_utils.py` & `rdfdf-0.1.5/rdfdf/helpers/rdfdf_utils.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.4/rdfdf/rdfdf.py` & `rdfdf-0.1.5/rdfdf/rdfdf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from collections.abc import Callable, Mapping, Iterable
 from typing import Generator
 
 import pandas as pd
 from rdflib import Graph, Literal, URIRef, Namespace
 
-from rdfdf.helpers.rdfdf_utils import anaphoric
-
 _TripleObject = URIRef | Literal
 _FieldRules = Mapping[str, tuple[URIRef, Callable[[str], _TripleObject]]]
 _TripleType = tuple[URIRef, URIRef, _TripleObject]
 
 
 class DFGraphConverter:
     """Rule-based pandas.DataFrame to rdflib.Graph converter.
@@ -63,22 +61,28 @@
                 if self._subject_rule
                 else row[self._subject_column]
             )
 
             for field, rule in self._column_rules.items():
                 _object = row[field]
 
+                ## old
                 # make bindings meaningful in rule callables
-                rule = anaphoric(
+                # rule = anaphoric(
+                #     __subject__=_subject,
+                #     __object__=_object,
+                #     __store__=self.store
+                # )(rule)
+
+                ## new
+                field_rule_result = rule(
                     __subject__=_subject,
                     __object__=_object,
                     __store__=self.store
-                )(rule)
-
-                field_rule_result = rule()
+                )
 
                 # yield only rdflib.Graph instances
                 if isinstance(field_rule_result, Graph):
                     yield field_rule_result
                 continue
 
     def _merge_to_graph_component(self,
```

### Comparing `rdfdf-0.1.4/PKG-INFO` & `rdfdf-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfdf
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 License: GPL3
 Author: Lukas Plank
 Author-email: lupl@tuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: rdflib (>=6.3.2,<7.0.0)
 Description-Content-Type: text/markdown
 
 
 # rdfdf
 ![pipeline status](https://gitlab.com/lupl/rdfdf/badges/dev/pipeline.svg)
+[![PyPI version](https://badge.fury.io/py/rdfdf.svg)](https://badge.fury.io/py/rdfdf)
 
 rdfdf - Functionality for rule-based `pandas.DataFrame` - `rdflib.Graph` conversion.
 
 For representation of tabular data in RDF see Allemang, Hendler: Semantic Web for the Working Ontologist. 2011, 40ff.
 
 > This project is in an early stage of development and should be used with caution.
```

