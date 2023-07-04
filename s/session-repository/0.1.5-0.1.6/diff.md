# Comparing `tmp/session-repository-0.1.5.tar.gz` & `tmp/session-repository-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.1.5.tar", last modified: Fri Jun 30 09:45:16 2023, max compression
+gzip compressed data, was "session-repository-0.1.6.tar", last modified: Tue Jul  4 11:22:14 2023, max compression
```

## Comparing `session-repository-0.1.5.tar` & `session-repository-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 09:45:16.805306 session-repository-0.1.5/
--rw-rw-rw-   0        0        0      599 2023-06-30 09:45:16.803537 session-repository-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 09:45:16.774274 session-repository-0.1.5/session_repository/
--rw-rw-rw-   0        0        0     7457 2023-06-30 09:44:47.000000 session-repository-0.1.5/session_repository/core.py
--rw-rw-rw-   0        0        0      487 2023-06-29 16:01:04.000000 session-repository-0.1.5/session_repository/enum.py
--rw-rw-rw-   0        0        0     7274 2023-06-30 07:14:32.000000 session-repository-0.1.5/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 09:45:16.796194 session-repository-0.1.5/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-06-30 09:45:16.000000 session-repository-0.1.5/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-30 09:45:16.000000 session-repository-0.1.5/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 09:45:16.000000 session-repository-0.1.5/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-30 09:45:16.000000 session-repository-0.1.5/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-30 09:45:16.000000 session-repository-0.1.5/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 09:45:16.806439 session-repository-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-06-30 09:44:59.000000 session-repository-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 11:22:14.013910 session-repository-0.1.6/
+-rw-rw-rw-   0        0        0      599 2023-07-04 11:22:14.011911 session-repository-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-04 11:22:13.977531 session-repository-0.1.6/session_repository/
+-rw-rw-rw-   0        0        0     8446 2023-07-04 11:21:39.000000 session-repository-0.1.6/session_repository/core.py
+-rw-rw-rw-   0        0        0      487 2023-06-29 16:01:04.000000 session-repository-0.1.6/session_repository/enum.py
+-rw-rw-rw-   0        0        0     7274 2023-06-30 07:14:32.000000 session-repository-0.1.6/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 11:22:14.006794 session-repository-0.1.6/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-07-04 11:22:13.000000 session-repository-0.1.6/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-04 11:22:13.000000 session-repository-0.1.6/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 11:22:13.000000 session-repository-0.1.6/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-04 11:22:13.000000 session-repository-0.1.6/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-04 11:22:13.000000 session-repository-0.1.6/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 11:22:14.014910 session-repository-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-07-04 11:21:46.000000 session-repository-0.1.6/setup.py
```

### Comparing `session-repository-0.1.5/PKG-INFO` & `session-repository-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.1.5
+Version: 0.1.6
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.5.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.6.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.1.5/session_repository/core.py` & `session-repository-0.1.6/session_repository/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,255 +1,210 @@
 # MODULES
-from contextlib import AbstractContextManager
-from logging import Logger
+import json
 from typing import (
     Any,
-    Callable,
     Dict,
+    Iterable,
     List,
-    Optional,
     Tuple,
-    Type,
-    TypeVar,
     Union,
 )
 
-# PYDANTIC
-from pydantic import BaseModel
-
 # SQLALCHEMY
-from sqlalchemy.orm import Session, InstrumentedAttribute
-
-# UTILS
-from session_repository.utils import (
-    _FilterType,
-    apply_no_load,
-    apply_filters,
-    apply_order_by,
-    apply_limit,
-    apply_pagination,
+from sqlalchemy import and_, asc, desc, tuple_
+from sqlalchemy.orm import (
+    Query,
+    InstrumentedAttribute,
+    noload,
 )
+from sqlalchemy.sql.elements import Null
 
+# Enum
+from session_repository.enum import Operators
 
-T = TypeVar("T", bound=BaseModel)
+_FilterType = Dict[Union[InstrumentedAttribute, Tuple[InstrumentedAttribute]], Any]
 
 
-class SessionRepository:
-    def __init__(
-        self,
-        session_factory: Callable[..., AbstractContextManager[Session]],
-        logger: Logger,
-        literal_binds: bool = True,
-    ) -> None:
-        self._session_factory = session_factory
-        self._logger = logger
-        self._literal_binds = literal_binds
-
-    def _select(
-        self,
-        model,
-        model_returned: Optional[Type[T]] = None,
-        filters: Optional[_FilterType] = None,
-        disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
-        current_session: Optional[Session] = None,
-    ) -> Optional[T]:
-        def _select_from_session(session: Session):
-            query = session.query(model)
-            query = apply_no_load(query=query, relationship_dict=disabled_relationships)
-            query = apply_filters(query=query, filter_dict=filters)
-            results = query.first()
-
-            if self._logger is not None:
-                query_compiled = query.statement.compile(
-                    compile_kwargs={"literal_binds": self._literal_binds}
-                )
-                self._logger.info(query_compiled.string)
-
-            if results is None:
-                return
-
-            mapped_results = (
-                model_returned.from_orm(results)
-                if model_returned is not None
-                else results
-            )
+def apply_no_load(
+    query: Query,
+    relationship_dict: Dict[InstrumentedAttribute, Any],
+    parents: List[InstrumentedAttribute] = None,
+):
+    if relationship_dict is None:
+        return query
 
-            return mapped_results
+    for relationship, sub_relationships in relationship_dict.items():
+        if relationship is None or not isinstance(relationship, InstrumentedAttribute):
+            continue
 
-        if current_session is not None:
-            results = _select_from_session(session=current_session)
+        sub_items = [relationship] if parents is None else [*parents, relationship]
+        if sub_relationships is None:
+            query = query.options(noload(*sub_items))
         else:
-            with self._session_factory() as session:
-                results = _select_from_session(session=session)
-
-        return results
-
-    def _select_all(
-        self,
-        model,
-        model_returned: Optional[Type[T]] = None,
-        filters: Optional[_FilterType] = None,
-        disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
-        page: Optional[int] = None,
-        per_page: Optional[int] = None,
-        order_by: Optional[Union[List[str], str]] = None,
-        direction: Optional[str] = None,
-        limit: int = None,
-        current_session: Optional[Session] = None,
-    ) -> Union[Tuple[List[T], str], List[T]]:
-        def _select_from_session(session: Session):
-            query = session.query(model)
             query = apply_no_load(
-                query=query,
-                relationship_dict=disabled_relationships,
-            )
-            query = apply_filters(
-                query=query,
-                filter_dict=filters,
-            )
-            query = apply_order_by(
-                query=query,
-                model=model,
-                order_by=order_by,
-                direction=direction,
-            )
-            query = apply_limit(
-                query=query,
-                limit=limit,
-            )
-            query, pagination = apply_pagination(
-                query=query,
-                page=page,
-                per_page=per_page,
-            )
-
-            results = query.all()
-
-            if self._logger is not None:
-                query_compiled = query.statement.compile(
-                    compile_kwargs={"literal_binds": self._literal_binds}
-                )
-                self._logger.info(query_compiled.string)
-
-            if results is None:
-                return
-
-            mapped_results = (
-                [model_returned.from_orm(res) for res in results]
-                if model_returned is not None
-                else results
-            )
-
-            if pagination is None:
-                return mapped_results
-
-            return mapped_results, pagination
-
-        if current_session is not None:
-            results = _select_from_session(session=current_session)
-        else:
-            with self._session_factory() as session:
-                results = _select_from_session(session=session)
-
-        return results
-
-    def _update(
-        self,
-        model,
-        values: Dict,
-        filters: Optional[_FilterType] = None,
-        flush: bool = False,
-        commit: bool = False,
-        current_session: Optional[Session] = None,
-    ):
-        def _update_from_session(session: Session):
-            rows = self._select_all(
-                model=model,
-                filters=filters,
-                current_session=session,
-            )
-
-            if len(rows) == 0:
-                return rows
+                query,
+                relationship_dict=sub_relationships,
+                parents=sub_items,
+            )
+
+    return query
+
+
+def apply_filters(query: Query, filter_dict: _FilterType):
+    filters = get_filters(filters=filter_dict)
+
+    return query if len(filters) == 0 else query.filter(and_(*filters))
+
+
+def apply_order_by(query: Query, model, order_by: list[str] | str, direction: str):
+    if order_by is None:
+        return query
+
+    if isinstance(order_by, str):
+        order_by = [order_by]
+
+    if direction == "desc":
+        return query.order_by(*[desc(getattr(model, column)) for column in order_by])
+
+    if direction == "asc":
+        return query.order_by(*[asc(getattr(model, column)) for column in order_by])
+
+    return query
+
+
+def build_order_by(model, order_by: dict):
+    if isinstance(order_by, dict):
+        order_by_list = []
+        for key, value in order_by.items():
+            if isinstance(value, dict):
+                relationship = getattr(model, key)
+                order_by_relationship = build_order_by(value, relationship)
+                order_by_list.extend(order_by_relationship)
+            else:
+                column = getattr(model, key)
+                if value == "ASC":
+                    order_by_list.append(asc(column))
+                elif value == "DESC":
+                    order_by_list.append(desc(column))
+        return order_by_list
+    else:
+        raise ValueError("Invalid nomenclature format.")
+
+
+def apply_pagination(query: Query, page: int, per_page: int):
+    pagination = None
+    if page is not None and per_page is not None:
+        total_results = query.count()
+        total_pages = (total_results + per_page - 1) // per_page
+
+        pagination = {
+            "total": total_results,
+            "page": page,
+            "per_page": per_page,
+            "total_pages": total_pages,
+        }
+
+        pagination = json.dumps(pagination)
+
+        query = query.offset((page - 1) * per_page).limit(per_page)
+
+    return query, pagination
+
+
+def apply_limit(query: Query, limit: int):
+    return query.limit(limit) if limit is not None else query
+
+
+def get_conditions_from_dict(values: _FilterType):
+    conditions = []
+    for key, value in values.items():
+        if type(value) == set:
+            value = list(value)
+        elif type(value) == dict:
+            for k, v in value.items():
+                if v is None:
+                    continue
+
+                match k:
+                    case Operators.EQUAL:
+                        conditions.append(key == v)
+                    case Operators.DIFFERENT:
+                        conditions.append(key != v)
+                    case Operators.LIKE:
+                        if not isinstance(v, Null):
+                            conditions.append(key.like(v))
+                        else:
+                            conditions.append(key == v)
+                    case Operators.NOT_LIKE:
+                        if not isinstance(v, Null):
+                            conditions.append(~key.like(v))
+                        else:
+                            conditions.append(key != v)
+                    case Operators.ILIKE:
+                        if not isinstance(v, Null):
+                            conditions.append(key.ilike(v))
+                        else:
+                            conditions.append(key == v)
+                    case Operators.NOT_ILIKE:
+                        if not isinstance(v, Null):
+                            conditions.append(~key.ilike(v))
+                        else:
+                            conditions.append(key != v)
+                    case Operators.BETWEEN:
+                        if len(v) != 2:
+                            continue
+                        if v[0] is not None:
+                            conditions.append(key > v[0])
+                        if v[1] is not None:
+                            conditions.append(key < v[1])
+                    case Operators.BETWEEN_OR_EQUAL:
+                        if len(v) != 2:
+                            continue
+                        if v[0] is not None:
+                            conditions.append(key >= v[0])
+                        if v[1] is not None:
+                            conditions.append(key <= v[1])
+                    case Operators.SUPERIOR:
+                        conditions.append(key > v)
+                    case Operators.INFERIOR:
+                        conditions.append(key < v)
+                    case Operators.SUPERIOR_OR_EQUAL:
+                        conditions.append(key >= v)
+                    case Operators.INFERIOR_OR_EQUAL:
+                        conditions.append(key <= v)
+                    case Operators.IN:
+                        v = v if isinstance(v, Iterable) else [v]
+                        if isinstance(key, tuple):
+                            conditions.append(tuple_(*key).in_(v))
+                        else:
+                            conditions.append(key.in_(v))
+                    case Operators.NOT_IN:
+                        v = v if isinstance(v, Iterable) else [v]
+                        conditions.append(key.notin_(v))
+                    case Operators.HAS:
+                        v = get_filters(v)
+                        for condition in v:
+                            conditions.append(key.has(condition))
+                    case Operators.ANY:
+                        v = get_filters(v)
+                        conditions.append(key.any(and_(*v)))
+
+    return conditions
+
+
+def get_filters(filters: _FilterType):
+    if filters is None:
+        return []
+    if not isinstance(filters, dict):
+        raise TypeError("<filters> must be type of <dict>")
+
+    filters = [{x: y} for x, y in filters.items()]
+
+    conditions = []
+    for filter_c in filters:
+        if not type(filter_c) == dict:
+            continue
 
-            for row in rows:
-                for key, value in values.items():
-                    setattr(row, key, value)
-
-            if flush:
-                session.flush()
-            if commit:
-                session.commit()
-
-            [session.refresh(row) for row in rows]
-
-            return rows
-
-        if current_session is not None:
-            results = _update_from_session(session=current_session)
-        else:
-            with self._session_factory() as session:
-                results = _update_from_session(session=session)
-
-        return results
-
-    def _add(
-        self,
-        data,
-        flush: bool = False,
-        commit: bool = False,
-        current_session: Optional[Session] = None,
-    ):
-        def _add_from_session(session: Session):
-            session.add_all(data) if isinstance(data, list) else session.add(data)
-            if flush:
-                session.flush()
-            if commit:
-                session.commit()
-
-            session.refresh(data)
-
-            return data
-
-        if current_session is not None:
-            results = _add_from_session(session=current_session)
-        else:
-            with self._session_factory() as session:
-                results = _add_from_session(session=session)
-
-        return results
-
-    def _delete(
-        self,
-        model,
-        filters: Optional[_FilterType] = None,
-        flush: bool = True,
-        commit: bool = False,
-        current_session: Optional[Session] = None,
-    ) -> bool:
-        def _delete_from_session(session: Session):
-            rows: List[BaseModel] = self._select_all(
-                model=model,
-                filters=filters,
-                current_session=session,
-            )
-
-            if len(rows) == 0:
-                return False
-
-            for row in rows:
-                session.delete(row)
-
-            if flush:
-                session.flush()
-            if commit:
-                session.commit()
-
-            return True
-
-        if current_session is not None:
-            results = _delete_from_session(session=current_session)
-        else:
-            with self._session_factory() as session:
-                results = _delete_from_session(session=session)
+        conditions_from_dict = get_conditions_from_dict(filter_c)
+        conditions.extend(conditions_from_dict)
 
-        return results
+    return conditions
```

### Comparing `session-repository-0.1.5/session_repository.egg-info/PKG-INFO` & `session-repository-0.1.6/session_repository.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.1.5
+Version: 0.1.6
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.5.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.6.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.1.5/setup.py` & `session-repository-0.1.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.1.5"
+version = "0.1.6"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
     ],
```

