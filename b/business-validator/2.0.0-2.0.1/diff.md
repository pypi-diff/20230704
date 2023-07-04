# Comparing `tmp/business_validator-2.0.0.tar.gz` & `tmp/business_validator-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "business_validator-2.0.0.tar", last modified: Tue May  9 13:11:49 2023, max compression
+gzip compressed data, was "business_validator-2.0.1.tar", last modified: Tue Jul  4 09:41:36 2023, max compression
```

## Comparing `business_validator-2.0.0.tar` & `business_validator-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1074 2023-02-10 10:09:01.557162 business_validator-2.0.0/LICENSE
--rw-r--r--   0        0        0     1674 2023-05-09 13:09:52.011288 business_validator-2.0.0/README.md
--rw-r--r--   0        0        0      289 2023-03-28 12:00:54.186864 business_validator-2.0.0/business_validator/__init__.py
--rw-r--r--   0        0        0     1285 2023-05-09 13:09:52.011746 business_validator-2.0.0/business_validator/types.py
--rw-r--r--   0        0        0     3328 2023-05-09 13:09:52.012108 business_validator-2.0.0/business_validator/validator.py
--rw-r--r--   0        0        0        0 2023-02-10 09:47:42.224957 business_validator-2.0.0/examples/__init__.py
--rw-r--r--   0        0        0     2298 2023-05-09 13:09:52.012674 business_validator-2.0.0/examples/multiple_error.py
--rw-r--r--   0        0        0     1847 2023-05-09 13:09:52.013100 business_validator-2.0.0/examples/single_error.py
--rw-r--r--   0        0        0      389 2023-03-28 13:01:06.373484 business_validator-2.0.0/examples/types.py
--rw-r--r--   0        0        0      812 2023-05-09 13:11:49.376154 business_validator-2.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 12:31:25.057797 business_validator-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0      294 2023-05-09 13:09:52.014537 business_validator-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0      239 2023-05-06 17:01:08.159610 business_validator-2.0.0/tests/factories.py
--rw-r--r--   0        0        0      300 2023-03-28 14:30:58.962078 business_validator-2.0.0/tests/test_multiple_error.py
--rw-r--r--   0        0        0      881 2023-05-06 16:57:39.505219 business_validator-2.0.0/tests/test_single_error.py
--rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 business_validator-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-06-15 14:23:21.006447 business_validator-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1744 2023-06-15 14:23:21.006447 business_validator-2.0.1/README.md
+-rw-r--r--   0        0        0      301 2023-06-15 14:23:21.006447 business_validator-2.0.1/business_validator/__init__.py
+-rw-r--r--   0        0        0     1342 2023-07-04 09:22:59.372682 business_validator-2.0.1/business_validator/types.py
+-rw-r--r--   0        0        0      287 2023-07-04 08:59:16.220112 business_validator-2.0.1/business_validator/utils.py
+-rw-r--r--   0        0        0     3676 2023-07-04 09:22:26.933206 business_validator-2.0.1/business_validator/validator.py
+-rw-r--r--   0        0        0        0 2023-06-15 14:23:21.007451 business_validator-2.0.1/examples/__init__.py
+-rw-r--r--   0        0        0     2370 2023-07-04 09:08:12.071279 business_validator-2.0.1/examples/multiple_error.py
+-rw-r--r--   0        0        0     1918 2023-06-15 14:23:21.008455 business_validator-2.0.1/examples/single_error.py
+-rw-r--r--   0        0        0      410 2023-06-15 14:23:21.008455 business_validator-2.0.1/examples/types.py
+-rw-r--r--   0        0        0      812 2023-07-04 09:41:36.693451 business_validator-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-15 14:23:21.009458 business_validator-2.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      307 2023-06-15 14:23:21.009458 business_validator-2.0.1/tests/conftest.py
+-rw-r--r--   0        0        0      251 2023-06-15 14:23:21.009458 business_validator-2.0.1/tests/factories.py
+-rw-r--r--   0        0        0      311 2023-06-15 14:23:21.009458 business_validator-2.0.1/tests/test_multiple_error.py
+-rw-r--r--   0        0        0      911 2023-06-15 14:23:21.010461 business_validator-2.0.1/tests/test_single_error.py
+-rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 business_validator-2.0.1/PKG-INFO
```

### Comparing `business_validator-2.0.0/LICENSE` & `business_validator-2.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2023 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2023 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `business_validator-2.0.0/README.md` & `business_validator-2.0.1/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-# Business-Validator
-
-## ErrorSchema
-Use business_validator.ErrorSchema if you don't know which format you're gonna use.
-
-## Quick Start
-
-### DTO
-```python
-class CommentDto(BaseModel):
-    comment: str
-    post_id: int
-    owner_id: int
-```
-
-
-### Add error source (error context)
-```python
-class Source(BaseModel):
-    local: str
-```
-
-### DTO Validator
-```python
-@dataclasses.dataclass()
-class CommentValidator(Validator[ErrorSchema[Source]]):
-    dto: CommentDto
-
-    @validate
-    async def test1(self):
-        post_ids = list(range(1, 10))
-
-        if self.dto.post_id not in post_ids:
-            self.context.add_error(
-                ErrorSchema(
-                    code=ErrorCodeEnum.not_found.value,
-                    message="Id doen't not exists",
-                    detail=f"Post with id={self.dto.post_id} not found",
-                    source=Source(
-                        local="data/post_id",
-                    ),
-                )
-            )
-
-    @validate
-    async def test2(self):
-        owner_ids = list(range(1, 10))
-
-        if self.dto.owner_id not in owner_ids:
-            self.context.add_error(
-                ErrorSchema(
-                    code=ErrorCodeEnum.not_found.value,
-                    message="Id doen't not exists",
-                    detail=f"User with id={self.dto.post_id} not found",
-                    source=Source(
-                        local="data/owner_id",
-                    ),
-                )
-            )
-```
-
-### Use
-```python
-async def function():
-    validator = CommentValidator(...)
-    errors = await validator.errors()
-    # or
-    await validator.validate() # raise ValidationError
-
-```
+# Business-Validator
+
+## ErrorSchema
+Use business_validator.ErrorSchema if you don't know which format you're gonna use.
+
+## Quick Start
+
+### DTO
+```python
+class CommentDto(BaseModel):
+    comment: str
+    post_id: int
+    owner_id: int
+```
+
+
+### Add error source (error context)
+```python
+class Source(BaseModel):
+    local: str
+```
+
+### DTO Validator
+```python
+@dataclasses.dataclass()
+class CommentValidator(Validator[ErrorSchema[Source]]):
+    dto: CommentDto
+
+    @validate
+    async def test1(self):
+        post_ids = list(range(1, 10))
+
+        if self.dto.post_id not in post_ids:
+            self.context.add_error(
+                ErrorSchema(
+                    code=ErrorCodeEnum.not_found.value,
+                    message="Id doen't not exists",
+                    detail=f"Post with id={self.dto.post_id} not found",
+                    source=Source(
+                        local="data/post_id",
+                    ),
+                )
+            )
+
+    @validate
+    async def test2(self):
+        owner_ids = list(range(1, 10))
+
+        if self.dto.owner_id not in owner_ids:
+            self.context.add_error(
+                ErrorSchema(
+                    code=ErrorCodeEnum.not_found.value,
+                    message="Id doen't not exists",
+                    detail=f"User with id={self.dto.post_id} not found",
+                    source=Source(
+                        local="data/owner_id",
+                    ),
+                )
+            )
+```
+
+### Use
+```python
+async def function():
+    validator = CommentValidator(...)
+    errors = await validator.errors()
+    # or
+    await validator.validate() # raise ValidationError
+
+```
```

### Comparing `business_validator-2.0.0/business_validator/types.py` & `business_validator-2.0.1/business_validator/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,51 @@
-import dataclasses
-from enum import Enum
-from collections.abc import Callable, Coroutine, Sequence
-from typing import Any, Generic, TypeAlias, TypeVar
-
-from pydantic.generics import GenericModel
-
-
-_T = TypeVar("_T")
-_S = TypeVar("_S")
-
-ValidatorFunc: TypeAlias = Callable[[Any], Coroutine[Any, Any, None]]
-
-
-class ErrorCodeEnum(str, Enum):
-    unique_constraint = "UNIQUE CONSTRAINT"
-    not_found = "NOT FOUND"
-    permission_denied = "PERMISSION DENIED"
-
-
-class ErrorSchema(GenericModel, Generic[_S]):
-    code: str
-    message: str
-    detail: str | None = None
-    source: _S | None = None
-
-
-class ValidationError(Generic[_T], Exception):
-    messages: list[_T]
-
-    def __init__(self, messages: list[_T], *args: object) -> None:
-        super().__init__(*args)
-        self.messages = messages
-
-
-@dataclasses.dataclass(frozen=True, slots=True)
-class ValidationContext(Generic[_T]):
-    _errors: list[_T] = dataclasses.field(default_factory=list)
-
-    def add_error(self, error: _T) -> None:
-        if error not in self._errors:
-            self._errors.append(error)
-
-    def extend_error(self, errors: Sequence[_T]) -> None:
-        self._errors.extend(errors)
-
-    @property
-    def errors(self) -> list[_T]:
-        return self._errors
-
-
-SelfValidator: TypeAlias = Any  # heh
+import dataclasses
+from enum import Enum
+from collections.abc import Callable, Coroutine, Sequence
+from typing import Any, Generic, TypeAlias, TypeVar
+
+from pydantic.generics import GenericModel
+
+
+_T = TypeVar("_T")
+_S = TypeVar("_S")
+
+SelfValidator: TypeAlias = Any  # heh
+
+ValidatorFunc: TypeAlias = Callable[[Any], Coroutine[Any, Any, None] | None]
+
+
+class ErrorCodeEnum(str, Enum):
+    unique_constraint = "UNIQUE CONSTRAINT"
+    not_found = "NOT FOUND"
+    permission_denied = "PERMISSION DENIED"
+
+
+class ErrorSchema(GenericModel, Generic[_S]):
+    code: str
+    message: str
+    detail: str | None = None
+    source: _S | None = None
+
+
+class ValidationError(Generic[_T], Exception):
+    messages: list[_T]
+
+    def __init__(self, messages: list[_T], *args: object) -> None:
+        super().__init__(*args)
+        self.messages = messages
+
+
+@dataclasses.dataclass(frozen=True, slots=True)
+class ValidationContext(Generic[_T]):
+    _errors: list[_T] = dataclasses.field(default_factory=list)
+
+    def add_error(self, error: _T) -> None:
+        if error not in self._errors:
+            self._errors.append(error)
+
+    def extend_error(self, errors: Sequence[_T]) -> None:
+        self._errors.extend(errors)
+
+    @property
+    def errors(self) -> list[_T]:
+        return self._errors
```

### Comparing `business_validator-2.0.0/examples/multiple_error.py` & `business_validator-2.0.1/examples/multiple_error.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-import asyncio
-import dataclasses
-import functools
-from business_validator import (
-    Validator,
-    ValidationError,
-    ErrorSchema,
-    ErrorCodeEnum,
-    validate,
-)
-from examples.types import CommentDto, CustomValidationContext, SourceMultiple
-
-
-@dataclasses.dataclass()
-class CommentValidator(Validator[ErrorSchema[SourceMultiple]]):
-    dto_list: list[CommentDto]
-
-    @functools.cached_property
-    def context(self) -> CustomValidationContext:  # type: ignore[override]
-        return CustomValidationContext()
-
-    @validate
-    async def test1(self):
-        post_ids = range(1, 10)
-        for i, dto in enumerate(self.dto_list):
-            if dto.post_id not in post_ids:
-                self.context.add_error(
-                    ErrorSchema(
-                        code=ErrorCodeEnum.not_found.value,
-                        message="Id doen't not exists",
-                        detail=f"Post with id={dto.post_id} not found",
-                        source=SourceMultiple(
-                            local="data/post_id",
-                            position=i,
-                        ),
-                    )
-                )
-
-    @validate
-    async def test2(self):
-        owner_ids = range(1, 10)
-        for i, dto in enumerate(self.dto_list):
-            if dto.owner_id not in owner_ids:
-                self.context.add_error(
-                    ErrorSchema(
-                        code=ErrorCodeEnum.not_found.value,
-                        message="Id doen't not exists",
-                        detail=f"User with id={dto.post_id} not found",
-                        source=SourceMultiple(
-                            local="data/owner_id",
-                            position=i,
-                        ),
-                    )
-                )
-
-
-async def main():
-    dto_list = [
-        CommentDto(comment="comment", owner_id=1, post_id=1),
-        CommentDto(comment="comment", owner_id=1, post_id=100),
-        CommentDto(comment="comment", owner_id=100, post_id=1),
-        CommentDto(comment="comment", owner_id=1234, post_id=1234),
-    ]
-    try:
-        await CommentValidator(dto_list).validate()
-    except ValidationError as e:
-        for message in e.messages:
-            print(message)
-
-
-if __name__ == "__main__":
-    asyncio.run(main())
+import asyncio
+import dataclasses
+import functools
+from business_validator import (
+    Validator,
+    ValidationError,
+    ErrorSchema,
+    ErrorCodeEnum,
+    validate,
+)
+from examples.types import CommentDto, CustomValidationContext, SourceMultiple
+
+
+@dataclasses.dataclass()
+class CommentValidator(Validator[ErrorSchema[SourceMultiple]]):
+    dto_list: list[CommentDto]
+
+    @functools.cached_property
+    def context(self) -> CustomValidationContext:  # type: ignore[override]
+        return CustomValidationContext()
+
+    @validate
+    async def test1(self):
+        post_ids = range(1, 10)
+        for i, dto in enumerate(self.dto_list):
+            if dto.post_id not in post_ids:
+                self.context.add_error(
+                    ErrorSchema(
+                        code=ErrorCodeEnum.not_found.value,
+                        message="Id doen't not exists",
+                        detail=f"Post with id={dto.post_id} not found",
+                        source=SourceMultiple(
+                            local="data/post_id",
+                            position=i,
+                        ),
+                    )
+                )
+
+    @validate
+    async def test2(self):
+        owner_ids = range(1, 10)
+        for i, dto in enumerate(self.dto_list):
+            if dto.owner_id not in owner_ids:
+                self.context.add_error(
+                    ErrorSchema(
+                        code=ErrorCodeEnum.not_found.value,
+                        message="Id doen't not exists",
+                        detail=f"User with id={dto.post_id} not found",
+                        source=SourceMultiple(
+                            local="data/owner_id",
+                            position=i,
+                        ),
+                    )
+                )
+
+
+async def main():
+    dto_list = [
+        CommentDto(comment="comment", owner_id=1, post_id=1),
+        CommentDto(comment="comment", owner_id=1, post_id=100),
+        CommentDto(comment="comment", owner_id=100, post_id=1),
+        CommentDto(comment="comment", owner_id=1234, post_id=1234),
+    ]
+    try:
+        await CommentValidator(dto_list).validate()
+    except ValidationError as e:
+        for message in e.messages:
+            print(message)
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
```

### Comparing `business_validator-2.0.0/pyproject.toml` & `business_validator-2.0.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "business-validator"
-version = "2.0.0"
+version = "2.0.1"
 authors = [
     { name = "maksyutov vlad", email = "maksyutov.vlad@gmail.com" },
 ]
 dependencies = [
     "pydantic>=1.10.4",
 ]
 requires-python = ">=3.11"
```

### Comparing `business_validator-2.0.0/tests/test_single_error.py` & `business_validator-2.0.1/tests/test_single_error.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import pytest
-from examples.types import CommentDto
-from examples.single_error import CommentValidator
-
-
-pytestmark = [pytest.mark.anyio]
-
-
-async def test_random_data(random_body: list[CommentDto]) -> None:
-    for comment in random_body:
-        validator = CommentValidator(comment)
-        post_in_db = 1 <= comment.post_id < 10
-        owner_in_db = 1 <= comment.owner_id < 10
-
-        errors = await validator.errors()
-        if not post_in_db:
-            assert any(
-                [
-                    error.source is not None and error.source.local == "data/post_id"
-                    for error in errors
-                ]
-            )
-
-        if not owner_in_db:
-            assert any(
-                [
-                    error.source is not None and error.source.local == "data/owner_id"
-                    for error in errors
-                ]
-            )
+import pytest
+from examples.types import CommentDto
+from examples.single_error import CommentValidator
+
+
+pytestmark = [pytest.mark.anyio]
+
+
+async def test_random_data(random_body: list[CommentDto]) -> None:
+    for comment in random_body:
+        validator = CommentValidator(comment)
+        post_in_db = 1 <= comment.post_id < 10
+        owner_in_db = 1 <= comment.owner_id < 10
+
+        errors = await validator.errors()
+        if not post_in_db:
+            assert any(
+                [
+                    error.source is not None and error.source.local == "data/post_id"
+                    for error in errors
+                ]
+            )
+
+        if not owner_in_db:
+            assert any(
+                [
+                    error.source is not None and error.source.local == "data/owner_id"
+                    for error in errors
+                ]
+            )
```

### Comparing `business_validator-2.0.0/PKG-INFO` & `business_validator-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: business-validator
-Version: 2.0.0
+Version: 2.0.1
 Author-Email: maksyutov vlad <maksyutov.vlad@gmail.com>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/1PaCHeK1/business-validator
 Requires-Python: >=3.11
 Requires-Dist: pydantic>=1.10.4
 Description-Content-Type: text/markdown
```

