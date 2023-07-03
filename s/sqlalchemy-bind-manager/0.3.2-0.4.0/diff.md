# Comparing `tmp/sqlalchemy_bind_manager-0.3.2.tar.gz` & `tmp/sqlalchemy_bind_manager-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_bind_manager-0.3.2.tar", max compression
+gzip compressed data, was "sqlalchemy_bind_manager-0.4.0.tar", max compression
```

## Comparing `sqlalchemy_bind_manager-0.3.2.tar` & `sqlalchemy_bind_manager-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1073 2023-07-03 10:48:06.193385 sqlalchemy_bind_manager-0.3.2/LICENSE
--rw-r--r--   0        0        0     8733 2023-07-03 10:48:06.193385 sqlalchemy_bind_manager-0.3.2/README.md
--rw-r--r--   0        0        0     2375 2023-07-03 10:48:24.013456 sqlalchemy_bind_manager-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      107 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/__init__.py
--rw-r--r--   0        0        0     5241 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_bind_manager.py
--rw-r--r--   0        0        0      197 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/__init__.py
--rw-r--r--   0        0        0     5734 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/async_.py
--rw-r--r--   0        0        0    11340 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/base_repository.py
--rw-r--r--   0        0        0     1099 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/common.py
--rw-r--r--   0        0        0     7429 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/result_presenters.py
--rw-r--r--   0        0        0     5045 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/sync.py
--rw-r--r--   0        0        0     3229 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_transaction_handler.py
--rw-r--r--   0        0        0     1722 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_unit_of_work/__init__.py
--rw-r--r--   0        0        0      310 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/exceptions.py
--rw-r--r--   0        0        0    10397 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/protocols.py
--rw-r--r--   0        0        0        0 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/py.typed
--rw-r--r--   0        0        0      242 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/repository.py
--rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 sqlalchemy_bind_manager-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-03 22:38:35.648099 sqlalchemy_bind_manager-0.4.0/LICENSE
+-rw-r--r--   0        0        0     8733 2023-07-03 22:38:35.648099 sqlalchemy_bind_manager-0.4.0/README.md
+-rw-r--r--   0        0        0     2375 2023-07-03 22:38:47.900125 sqlalchemy_bind_manager-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/__init__.py
+-rw-r--r--   0        0        0     5241 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_bind_manager.py
+-rw-r--r--   0        0        0      197 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/__init__.py
+-rw-r--r--   0        0        0     6084 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/async_.py
+-rw-r--r--   0        0        0    11340 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/base_repository.py
+-rw-r--r--   0        0        0     1099 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/common.py
+-rw-r--r--   0        0        0     7429 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/result_presenters.py
+-rw-r--r--   0        0        0     5380 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/sync.py
+-rw-r--r--   0        0        0     3229 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_transaction_handler.py
+-rw-r--r--   0        0        0     1722 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_unit_of_work/__init__.py
+-rw-r--r--   0        0        0      310 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/exceptions.py
+-rw-r--r--   0        0        0    11155 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/protocols.py
+-rw-r--r--   0        0        0        0 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/py.typed
+-rw-r--r--   0        0        0      242 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/repository.py
+-rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 sqlalchemy_bind_manager-0.4.0/PKG-INFO
```

### Comparing `sqlalchemy_bind_manager-0.3.2/LICENSE` & `sqlalchemy_bind_manager-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.2/README.md` & `sqlalchemy_bind_manager-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.2/pyproject.toml` & `sqlalchemy_bind_manager-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlalchemy-bind-manager"
-version = "0.3.2"
+version = "0.4.0"
 description = "A manager to easily handle multiple SQLAlchemy configurations"
 license = "MIT"
 authors = ["Federico Busetti <729029+febus982@users.noreply.github.com>"]
 repository = "https://github.com/febus982/sqlalchemy-bind-manager"
 homepage = "https://febus982.github.io/sqlalchemy-bind-manager"
 readme = "README.md"
 packages = [{include = "sqlalchemy_bind_manager"}]
```

### Comparing `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_bind_manager.py` & `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_bind_manager.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/async_.py` & `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/async_.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     List,
     Mapping,
     Tuple,
     Type,
     Union,
 )
 
+from sqlalchemy import select
 from sqlalchemy.ext.asyncio import AsyncSession
 
 from .._bind_manager import SQLAlchemyAsyncBind
 from .._transaction_handler import AsyncSessionHandler
 from ..exceptions import InvalidConfig, ModelNotFound
 from .base_repository import (
     BaseRepository,
@@ -80,25 +81,30 @@
     async def get(self, identifier: PRIMARY_KEY) -> MODEL:
         async with self._get_session(commit=False) as session:
             model = await session.get(self._model, identifier)
         if model is None:
             raise ModelNotFound("No rows found for provided primary key.")
         return model
 
-    async def delete(
-        self,
-        entity: Union[MODEL, PRIMARY_KEY],
-    ) -> None:
-        # TODO: delete without loading the model
-        if isinstance(entity, self._model):
-            obj = entity
-        else:
-            obj = await self.get(entity)  # type: ignore
+    async def get_many(self, identifiers: Iterable[PRIMARY_KEY]) -> List[MODEL]:
+        stmt = select(self._model).where(
+            getattr(self._model, self._model_pk()).in_(identifiers)
+        )
+
+        async with self._get_session(commit=False) as session:
+            return [x for x in (await session.execute(stmt)).scalars()]
+
+    async def delete(self, instance: MODEL) -> None:
+        async with self._get_session() as session:
+            await session.delete(instance)
+
+    async def delete_many(self, instances: Iterable[MODEL]) -> None:
         async with self._get_session() as session:
-            await session.delete(obj)
+            for instance in instances:
+                await session.delete(instance)
 
     async def find(
         self,
         search_params: Union[None, Mapping[str, Any]] = None,
         order_by: Union[None, Iterable[Union[str, Tuple[str, SortDirection]]]] = None,
     ) -> List[MODEL]:
         stmt = self._find_query(search_params, order_by)
```

### Comparing `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/base_repository.py` & `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/base_repository.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/common.py` & `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/common.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/result_presenters.py` & `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/result_presenters.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/sync.py` & `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     List,
     Mapping,
     Tuple,
     Type,
     Union,
 )
 
+from sqlalchemy import select
 from sqlalchemy.orm import Session
 
 from .._bind_manager import SQLAlchemyBind
 from .._transaction_handler import SessionHandler
 from ..exceptions import InvalidConfig, ModelNotFound
 from .base_repository import (
     BaseRepository,
@@ -69,22 +70,30 @@
     def get(self, identifier: PRIMARY_KEY) -> MODEL:
         with self._get_session(commit=False) as session:
             model = session.get(self._model, identifier)
         if model is None:
             raise ModelNotFound("No rows found for provided primary key.")
         return model
 
-    def delete(self, entity: Union[MODEL, PRIMARY_KEY]) -> None:
-        # TODO: delete without loading the model
-        if isinstance(entity, self._model):
-            obj = entity
-        else:
-            obj = self.get(entity)  # type: ignore
+    def get_many(self, identifiers: Iterable[PRIMARY_KEY]) -> List[MODEL]:
+        stmt = select(self._model).where(
+            getattr(self._model, self._model_pk()).in_(identifiers)
+        )
+
+        with self._get_session(commit=False) as session:
+            return [x for x in session.execute(stmt).scalars()]
+
+    def delete(self, instance: MODEL) -> None:
+        with self._get_session() as session:
+            session.delete(instance)
+
+    def delete_many(self, instances: Iterable[MODEL]) -> None:
         with self._get_session() as session:
-            session.delete(obj)
+            for model in instances:
+                session.delete(model)
 
     def find(
         self,
         search_params: Union[None, Mapping[str, Any]] = None,
         order_by: Union[None, Iterable[Union[str, Tuple[str, SortDirection]]]] = None,
     ) -> List[MODEL]:
         stmt = self._find_query(search_params, order_by)
```

### Comparing `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_transaction_handler.py` & `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_transaction_handler.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_unit_of_work/__init__.py` & `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_unit_of_work/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/protocols.py` & `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/protocols.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,22 +43,37 @@
     async def get(self, identifier: PRIMARY_KEY) -> MODEL:
         """Get a model by primary key.
 
         :param identifier: The primary key
         :return: A model instance
         :raises ModelNotFound: No model has been found using the primary key
         """
-        # TODO: implement get_many()
         ...
 
-    async def delete(self, entity: Union[MODEL, PRIMARY_KEY]) -> None:
+    async def get_many(self, identifiers: Iterable[PRIMARY_KEY]) -> List[MODEL]:
+        """Get a list of models by primary keys.
+
+        :param identifiers: A list of primary keys
+        :type identifiers: List
+        :return: A list of models
+        :rtype: List
+        """
+        ...
+
+    async def delete(self, instance: MODEL) -> None:
         """Deletes a model.
 
-        :param entity: The model instance or the primary key
-        :type entity: Union[MODEL, PRIMARY_KEY]
+        :param instance: The model instance
+        """
+        ...
+
+    async def delete_many(self, instances: Iterable[MODEL]) -> None:
+        """Deletes a collection of models in a single transaction.
+
+        :param instances: The model instances
         """
         ...
 
     async def find(
         self,
         search_params: Union[None, Mapping[str, Any]] = None,
         order_by: Union[None, Iterable[Union[str, Tuple[str, SortDirection]]]] = None,
@@ -184,22 +199,37 @@
     def get(self, identifier: PRIMARY_KEY) -> MODEL:
         """Get a model by primary key.
 
         :param identifier: The primary key
         :return: A model instance
         :raises ModelNotFound: No model has been found using the primary key
         """
-        # TODO: implement get_many()
         ...
 
-    def delete(self, entity: Union[MODEL, PRIMARY_KEY]) -> None:
+    def get_many(self, identifiers: Iterable[PRIMARY_KEY]) -> List[MODEL]:
+        """Get a list of models by primary keys.
+
+        :param identifiers: A list of primary keys
+        :type identifiers: List
+        :return: A list of models
+        :rtype: List
+        """
+        ...
+
+    def delete(self, instance: MODEL) -> None:
         """Deletes a model.
 
-        :param entity: The model instance or the primary key
-        :type entity: Union[MODEL, PRIMARY_KEY]
+        :param instance: The model instance
+        """
+        ...
+
+    async def delete_many(self, instances: Iterable[MODEL]) -> None:
+        """Deletes a collection of models in a single transaction.
+
+        :param instances: The model instances
         """
         ...
 
     def find(
         self,
         search_params: Union[None, Mapping[str, Any]] = None,
         order_by: Union[None, Iterable[Union[str, Tuple[str, SortDirection]]]] = None,
```

### Comparing `sqlalchemy_bind_manager-0.3.2/PKG-INFO` & `sqlalchemy_bind_manager-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-bind-manager
-Version: 0.3.2
+Version: 0.4.0
 Summary: A manager to easily handle multiple SQLAlchemy configurations
 Home-page: https://febus982.github.io/sqlalchemy-bind-manager
 License: MIT
 Keywords: sqlalchemy,config,manager
 Author: Federico Busetti
 Author-email: 729029+febus982@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
```

