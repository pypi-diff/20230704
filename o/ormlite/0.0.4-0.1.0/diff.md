# Comparing `tmp/ormlite-0.0.4.tar.gz` & `tmp/ormlite-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ormlite-0.0.4.tar", last modified: Mon Jul  3 16:49:05 2023, max compression
+gzip compressed data, was "ormlite-0.1.0.tar", last modified: Tue Jul  4 18:47:34 2023, max compression
```

## Comparing `ormlite-0.0.4.tar` & `ormlite-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:49:05.169872 ormlite-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-03 16:48:56.000000 ormlite-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-03 16:49:05.165872 ormlite-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-03 16:48:56.000000 ormlite-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-03 16:48:56.000000 ormlite-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:49:05.169872 ormlite-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:49:05.165872 ormlite-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:49:05.165872 ormlite-0.0.4/src/ormlite/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-03 16:48:56.000000 ormlite-0.0.4/src/ormlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-03 16:48:56.000000 ormlite-0.0.4/src/ormlite/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-03 16:48:56.000000 ormlite-0.0.4/src/ormlite/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-03 16:48:56.000000 ormlite-0.0.4/src/ormlite/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-07-03 16:48:56.000000 ormlite-0.0.4/src/ormlite/orm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-03 16:48:56.000000 ormlite-0.0.4/src/ormlite/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-03 16:48:56.000000 ormlite-0.0.4/src/ormlite/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-03 16:48:56.000000 ormlite-0.0.4/src/ormlite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:49:05.165872 ormlite-0.0.4/src/ormlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-03 16:49:05.000000 ormlite-0.0.4/src/ormlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-03 16:49:05.000000 ormlite-0.0.4/src/ormlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:49:05.000000 ormlite-0.0.4/src/ormlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-03 16:49:05.000000 ormlite-0.0.4/src/ormlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 16:49:05.000000 ormlite-0.0.4/src/ormlite.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:49:05.165872 ormlite-0.0.4/src/spec/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-03 16:48:56.000000 ormlite-0.0.4/src/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-03 16:48:56.000000 ormlite-0.0.4/src/spec/test_migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-03 16:48:56.000000 ormlite-0.0.4/src/spec/test_orm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-03 16:48:56.000000 ormlite-0.0.4/src/spec/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-03 16:48:56.000000 ormlite-0.0.4/src/spec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:47:34.328352 ormlite-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 18:47:23.000000 ormlite-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-04 18:47:34.328352 ormlite-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-04 18:47:23.000000 ormlite-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-04 18:47:23.000000 ormlite-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:47:34.328352 ormlite-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:47:34.324352 ormlite-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:47:34.328352 ormlite-0.1.0/src/ormlite/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 18:47:23.000000 ormlite-0.1.0/src/ormlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-04 18:47:23.000000 ormlite-0.1.0/src/ormlite/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-04 18:47:23.000000 ormlite-0.1.0/src/ormlite/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-04 18:47:23.000000 ormlite-0.1.0/src/ormlite/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-04 18:47:23.000000 ormlite-0.1.0/src/ormlite/orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-07-04 18:47:23.000000 ormlite-0.1.0/src/ormlite/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-04 18:47:23.000000 ormlite-0.1.0/src/ormlite/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-04 18:47:23.000000 ormlite-0.1.0/src/ormlite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:47:34.328352 ormlite-0.1.0/src/ormlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-04 18:47:34.000000 ormlite-0.1.0/src/ormlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-04 18:47:34.000000 ormlite-0.1.0/src/ormlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:47:34.000000 ormlite-0.1.0/src/ormlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-04 18:47:34.000000 ormlite-0.1.0/src/ormlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 18:47:34.000000 ormlite-0.1.0/src/ormlite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:47:34.328352 ormlite-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-04 18:47:23.000000 ormlite-0.1.0/tests/test_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-04 18:47:23.000000 ormlite-0.1.0/tests/test_orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-04 18:47:23.000000 ormlite-0.1.0/tests/test_query.py
```

### Comparing `ormlite-0.0.4/LICENSE` & `ormlite-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ormlite-0.0.4/PKG-INFO` & `ormlite-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ormlite
-Version: 0.0.4
+Version: 0.1.0
 Author-email: Charles Taylor <charlestaylor95@gmail.com>
 License: Copyright 2023 Charles Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
@@ -19,14 +19,15 @@
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [Read The Docs](https://ormlite.readthedocs.io/en/latest/)
 
+[PyPI](https://pypi.org/project/ormlite)
 <!---
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
 --->
 
 # Usage
 
 Install:
```

### Comparing `ormlite-0.0.4/README.md` & `ormlite-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [Read The Docs](https://ormlite.readthedocs.io/en/latest/)
 
+[PyPI](https://pypi.org/project/ormlite)
 <!---
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
 --->
 
 # Usage
 
 Install:
```

### Comparing `ormlite-0.0.4/pyproject.toml` & `ormlite-0.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ormlite"
-version = "0.0.4"
+version = "0.1.0"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.11"
 keywords = ["sqlite", "orm", "dataclass", "data", "query", "migration"]
 authors = [
   {name = "Charles Taylor", email = "charlestaylor95@gmail.com" }
 ]
@@ -25,9 +25,13 @@
 include = ["src/ormlite/"]
 # typeCheckingMode = "strict"
 
 reportUnusedImport = "information"
 reportUnusedVariable = "information"
 reportPrivateUsage = "error"
 # reportMissingTypeStubs = "warning"
+reportUnknownParameterType = "error"
 reportMissingParameterType = "error"
 reportSelfClsParameterName = "error"
+reportPropertyTypeMismatch = "error"
+reportIncompatibleMethodOverride = "error"
+reportUnknownLambdaType = "error"
```

### Comparing `ormlite-0.0.4/src/ormlite/adapters.py` & `ormlite-0.1.0/src/ormlite/adapters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,37 @@
+import logging
 from datetime import datetime, date
 
 from ormlite import orm
 from ormlite.orm import Adapter
 
+logger = logging.getLogger(__name__)
+
 
 def register():
     orm.register_adapter(BoolAdapter())
     orm.register_adapter(DateTimeAdapter())
     orm.register_adapter(DateAdapter())
 
 
 class BoolAdapter(Adapter[bool]):
-    sql_type = "BOOL"
+    sql_type = "BOOLEAN"
     python_type = bool
 
     def convert(self, b: bytes) -> bool:
-        if b == b"T":
+        if b == b"1":
             return True
-        elif b == b"F":
+        elif b == b"0":
             return False
         else:
-            raise Exception
+            logger.warning(f"adapting invalid bool with value of: {b}")
+            return True
 
     def adapt(self, val: bool) -> str:
-        return "T" if val else "F"
+        return "1" if val else "0"
 
 
 class DateAdapter(Adapter[date]):
     sql_type = "DATE"
     python_type = date
 
     def convert(self, b: bytes) -> date:
```

### Comparing `ormlite-0.0.4/src/ormlite/migrate.py` & `ormlite-0.1.0/src/ormlite/migrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 import dataclasses as dc
 import logging
-from typing import Any
+from typing import Any, Callable
 from collections.abc import Sequence
 
 from ormlite import orm
 from ormlite.orm import column_def, DatabaseConnection
 
 
 logger = logging.getLogger(__name__)
@@ -72,15 +72,15 @@
 
 def parse_column_names(raw_table_sql: str) -> set[str]:
     match = REGEX.match(raw_table_sql)
     if match is None:
         raise Exception(f"regex failed to parse: {raw_table_sql}")
 
     defs = match.group("defs").strip().split(",")
-    get_name = lambda row: re.split(r"\s+", row.strip())[0]
+    get_name: Callable[[str], str] = lambda row: re.split(r"\s+", row.strip())[0]
     col_names = {
         name for row in defs for name in [get_name(row)] if IDENT.fullmatch(name)
     }
     return col_names
 
 
 def index_of(fields: Sequence[dc.Field[Any]], name: str) -> int:
```

### Comparing `ormlite-0.0.4/src/ormlite/orm.py` & `ormlite-0.1.0/src/ormlite/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 import dataclasses as dc
 import sqlite3
 from collections.abc import Sequence
 from typing import (
     dataclass_transform,
     Any,
     Optional,
-    Iterable,
     TypeVar,
     ClassVar,
     Generic,
     Protocol,
 )
-from datetime import datetime, date
 
-from ormlite.errors import MissingAdapterError, InvalidForeignKeyError
+from ormlite.errors import MissingAdapterError, InvalidForeignKeyError, MultiplePrimaryKeysError
 from ormlite.utils import get_optional_type_arg
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
@@ -66,15 +64,15 @@
 
 
 @dataclass_transform()
 def model(sql_table_name: str):
     if isinstance(sql_table_name, type):
         raise TypeError("@model(sql_table_name) must be called with the sql table name")
 
-    def wrap(model: type):
+    def wrap(model: type) -> type:
         if sql_table_name in Context.TABLE_TO_MODEL:
             logger.warning(
                 f"Reregistering the sql table '{sql_table_name}' with {model}"
             )
         else:
             logger.debug(f"applying @model({sql_table_name}) to {model})")
 
@@ -86,24 +84,30 @@
 
         return model
 
     return wrap
 
 
 def validate_model(model: type):
+    has_primary = False
     for field in dc.fields(model):
         to_sql_type(field.type)
 
+        if field.metadata.get("pk"):
+            if has_primary:
+                raise MultiplePrimaryKeysError
+            else:
+                has_primary = True
 
 @dc.dataclass
 class ForeignKey:
     table: str
     key: Optional[str] = None
 
-    def to_constraint(self, field: dc.Field) -> str:
+    def to_constraint(self, field: dc.Field[Any]) -> str:
         return (
             f"FOREIGN KEY ({field.name}) "
             f"REFERENCES {self.table}({self.key or field.name})"
         )
 
 
 def field(*, pk: bool = False, fk: Optional[str] = None, **kwargs: Any):
@@ -166,15 +170,15 @@
 
     if sql_type is not None:
         return sql_type
 
     raise MissingAdapterError
 
 
-def column_def(field: dc.Field) -> str:
+def column_def(field: dc.Field[Any]) -> str:
     optional_inner_type = get_optional_type_arg(field.type)
 
     # not null is applied to all fields automatically
     # use default = None to get a nullable field
     constraint = "NOT NULL"
 
     if field.metadata.get("pk"):
```

### Comparing `ormlite-0.0.4/src/ormlite/query.py` & `ormlite-0.1.0/src/ormlite/query.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 import dataclasses as dc
 import sqlite3
-from typing import Self, Generic, TypeVar, Iterable, Optional
+from typing import (
+    Self, Generic, TypeVar, Optional, Any, Callable
+)
 from dataclasses import dataclass
 
 from ormlite import orm
 from ormlite.orm import to_sql_literal, DatabaseConnection as DbConnection
 
 logger = logging.getLogger(__name__)
 
@@ -30,108 +32,142 @@
     def __init__(self, model: type[Model]):
         self.model = model
         self.model_field_count = len(dc.fields(self.model))
         self.extra_columns = []
 
     # TODO: allow multiple joins via join dict ala ruby on rails
     # allow multiple calls to join
-    def join(self, table: str) -> Self:
+    def join(self, table: type[Any]) -> Self:
+        target_table = orm.sql_table_name(table)
         field = next(
-            field for field in dc.fields(self.model) if get_fk_table(field) == table
+            field for field in dc.fields(self.model) if get_fk_table(field) == target_table
         )
         self.join_clause = _prepare_join(
             source_table=orm.sql_table_name(self.model),
-            target_table=table,
+            target_table=target_table,
             source_key=field.name,
             target_key=field.metadata["fk"].key or field.name,
         )
         return self
 
     def extra(self, *fields: str) -> Self:
         self.extra_columns = list(fields)
         return self
 
-    def where(self, clause: str) -> Self:
-        if self.where_clause == "":
-            self.where_clause = f"WHERE {clause}"
+    def where(self, condition: Optional[str] = None, **kwargs: Any) -> Self:
+        if condition:
+            for key, value in kwargs.items():
+                condition = condition.replace(f":{key}", to_sql_literal(value))
+            conditions = [condition]
         else:
-            self.where_clause += f" AND ({clause})"
+            table_name = orm.sql_table_name(self.model)
+            conditions = []
+            for key, value in kwargs.items():
+                conditions.append(f"{table_name}.{key} = {to_sql_literal(value)}")
+
+        for condition in conditions:
+            if self.where_clause == "":
+                self.where_clause = f"WHERE ({condition})"
+            else:
+                self.where_clause += f" AND ({condition})"
 
         return self
 
     def order_by(self, clause: str) -> Self:
         self.order_by_clause = f"ORDER BY {clause}"
         return self
 
     def limit(self, limit: int) -> Self:
+        """
+        Applies a sql LIMIT.
+        Note that calling this multiple times on the same query, will override the previously set limit.
+        """
         self.limit_clause = f"LIMIT {limit}"
         return self
 
     def _execute(self, db: DbConnection) -> sqlite3.Cursor:
         extra = ""
         if self.extra_columns:
             extra = f",{','.join(self.extra_columns)}"
 
         table_name = orm.sql_table_name(self.model)
         query = f"""
-            SELECT {table_name}.*{extra}
-            FROM {table_name}
+            SELECT \"{table_name}\".*{extra}
+            FROM \"{table_name}\"
             {self.join_clause}
             {self.where_clause}
             {self.order_by_clause}
             {self.limit_clause}
         """
         logger.debug(query)
 
         return db.execute(query)
 
-    def models(self, db: DbConnection) -> Iterable[Model]:
+    def models(self, db: DbConnection) -> list[Model]:
         cursor = self._execute(db)
-        return (self._to_model(row) for row in cursor)
+        return [self._to_model(row) for row in cursor]
 
-    def rows(self, db: DbConnection) -> Iterable[Row[Model]]:
+    def dicts(self, db: DbConnection) -> list[dict[str, Any]]:
+        rows = []
         cursor = self._execute(db)
-        return (
-            Row(
-                model=self._to_model(row),
-                extra=self._to_extra(row),
-            )
-            for row in cursor
-        )
+        for raw in cursor:
+            extra = dict()
+            for desc, value in zip(cursor.description, raw):
+                key = desc[0]
+                extra[key] = value
+            rows.append(extra)
+        return rows
+
+    def rows(self, db: DbConnection) -> list[Row[Model]]:
+        rows = []
+        cursor = self._execute(db)
+        model_fields = set(field.name for field in dc.fields(self.model))
+        for raw in cursor:
+            extra = dict()
+            model_dict = dict()
+            for desc, value in zip(cursor.description, raw):
+                key = desc[0]
+                if key in model_fields:
+                    model_dict[key] = value
+                else:
+                    extra[key] = value
+            rows.append(Row(model=self.model(**model_dict), extra=extra))
+        return rows
 
-    def _to_model(self, row: tuple):
+    def _to_model(self, row: tuple[Any, ...]) -> Model:
         return self.model(*row[: self.model_field_count])
 
-    def _to_extra(self, row: tuple):
-        extra = {}
-        rest = row[self.model_field_count :]
-        for name, value in zip(self.extra_columns, rest):
-            extra[name] = value
-        return extra
 
 
 def select(model: type[Model]) -> SelectQuery[Model]:
+    """
+    Begin a select query.
+
+    :param model: Model class; this determines which model is when binding the sql rows into python objects
+    """
     return SelectQuery(model)
 
 
 def upsert(
     db: DbConnection, records: list[Model], *, update: list[str]
 ):  # pyright: ignore
-    """Insert records, on conflict, update fields but only specific ones
+    """
+    Insert records, on conflict, update fields but only specific ones
 
+    :param db: A sqlite database connection
     :param records: Records to insert or update
-    :type records: list[Model]
+    :param update: List of column names to update in case of conflict
     """
     # :param update: List of fields to update in the case of a conflict
     if len(records) == 0:
         return
     model = type(records[0])
     table = orm.sql_table_name(model)
     columns = [field.name for field in dc.fields(model)]
-    to_sql = lambda row: to_sql_literal([getattr(row, col) for col in columns])
+    to_sql: Callable[[Model], str] = lambda row: to_sql_literal([getattr(row, col) for col in columns])
 
     on_conflict_clause = ""
     if len(update) > 0:
         on_conflict_clause = f"""
             ON CONFLICT DO UPDATE
             SET {','.join(f'{col}=excluded.{col}' for col in update)}
         """
@@ -141,15 +177,15 @@
         INSERT INTO {table}({','.join(columns)})
         VALUES {','.join(to_sql(row) for row in records)}
         {on_conflict_clause}
         """
     )
 
 
-def get_fk_table(field: dc.Field) -> Optional[str]:
+def get_fk_table(field: dc.Field[Any]) -> Optional[str]:
     fk = field.metadata.get("fk")
     if not fk:
         return None
     return fk.table
 
 
 def _prepare_join(
```

### Comparing `ormlite-0.0.4/src/ormlite/utils.py` & `ormlite-0.1.0/src/ormlite/utils.py`

 * *Files identical despite different names*

### Comparing `ormlite-0.0.4/src/ormlite.egg-info/PKG-INFO` & `ormlite-0.1.0/src/ormlite.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ormlite
-Version: 0.0.4
+Version: 0.1.0
 Author-email: Charles Taylor <charlestaylor95@gmail.com>
 License: Copyright 2023 Charles Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
@@ -19,14 +19,15 @@
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [Read The Docs](https://ormlite.readthedocs.io/en/latest/)
 
+[PyPI](https://pypi.org/project/ormlite)
 <!---
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
 --->
 
 # Usage
 
 Install:
```

### Comparing `ormlite-0.0.4/src/spec/test_migrate.py` & `ormlite-0.1.0/tests/test_migrate.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     # Act
     migrate(db)
 
     # Assert
     assert fetch_table_defs(db) == [
         (
             "persons",
-            'CREATE TABLE "persons" (age INTEGER NOT NULL, name TEXT NOT NULL, address TEXT, phone INTEGER, funny BOOL NOT NULL, height REAL NOT NULL)',
+            'CREATE TABLE "persons" (age INTEGER NOT NULL, name TEXT NOT NULL, address TEXT, phone INTEGER, funny BOOLEAN NOT NULL, height REAL NOT NULL)',
         )
     ]
 
     # Arrange: delete models
     unregister_all_models()
 
     # Act
```

### Comparing `ormlite-0.0.4/src/spec/test_orm.py` & `ormlite-0.1.0/tests/test_orm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import pytest
 import dataclasses as dc
 import sqlite3
 from datetime import datetime, date
 from typing import Union, Optional
 
 from ormlite import model, field, migrate
-from ormlite.errors import MissingAdapterError, InvalidForeignKeyError
+from ormlite.errors import MissingAdapterError, InvalidForeignKeyError, MultiplePrimaryKeysError
 from ormlite.orm import ForeignKey, to_sql_literal, to_sql_type
 from .utils import unregister_all_models
 
 
 def test_bare_model_decorator_is_not_supported():
     with pytest.raises(TypeError):
-
         @model
         class Foo:
             pass
 
 
 def test_field_optional_union_supported():
     @model("union_operator")
@@ -45,14 +44,23 @@
     with pytest.raises(MissingAdapterError):
 
         @model("triple_union")
         class Foo:
             bar: Union[str, int, float]
 
 
+def test_multiple_primary_keys():
+    with pytest.raises(MultiplePrimaryKeysError):
+        @model("items")
+        class Item:
+            id_1: int = field(pk=True)
+            id_2: str = field(pk=True)
+
+
+
 def test_foreign_key_punning():
     @model("foos")
     class Foo:
         fk: str = field(fk="bars")
 
     @model("bars")
     class Bar:
```

