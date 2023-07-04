# Comparing `tmp/django_ninja_crud-0.1.3.tar.gz` & `tmp/django_ninja_crud-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ninja_crud-0.1.3.tar", max compression
+gzip compressed data, was "django_ninja_crud-0.2.0.tar", max compression
```

## Comparing `django_ninja_crud-0.1.3.tar` & `django_ninja_crud-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1069 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/LICENSE
--rw-r--r--   0        0        0     7755 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/__init__.py
--rw-r--r--   0        0        0      151 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/apps.py
--rw-r--r--   0        0        0      239 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/schemas.py
--rw-r--r--   0        0        0      574 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/tests/__init__.py
--rw-r--r--   0        0        0     5288 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/tests/test_abstract.py
--rw-r--r--   0        0        0     4581 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/tests/test_create.py
--rw-r--r--   0        0        0     2761 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/tests/test_delete.py
--rw-r--r--   0        0        0     5103 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/tests/test_list.py
--rw-r--r--   0        0        0     3244 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/tests/test_retrieve.py
--rw-r--r--   0        0        0     4668 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/tests/test_update.py
--rw-r--r--   0        0        0      303 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/tests/utils.py
--rw-r--r--   0        0        0      397 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/ninja_crud/utils.py
--rw-r--r--   0        0        0      409 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/ninja_crud/views/__init__.py
--rw-r--r--   0        0        0      794 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/ninja_crud/views/abstract.py
--rw-r--r--   0        0        0     3894 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/ninja_crud/views/create.py
--rw-r--r--   0        0        0     1582 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/ninja_crud/views/delete.py
--rw-r--r--   0        0        0     3971 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/ninja_crud/views/list.py
--rw-r--r--   0        0        0     1567 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/ninja_crud/views/retrieve.py
--rw-r--r--   0        0        0     2000 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/ninja_crud/views/update.py
--rw-r--r--   0        0        0     1611 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     9411 1970-01-01 00:00:00.000000 django_ninja_crud-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-04 20:35:06.226429 django_ninja_crud-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7601 2023-07-04 20:35:06.226429 django_ninja_crud-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-04 20:35:06.226429 django_ninja_crud-0.2.0/ninja_crud/__init__.py
+-rw-r--r--   0        0        0      151 2023-07-04 20:35:06.226429 django_ninja_crud-0.2.0/ninja_crud/apps.py
+-rw-r--r--   0        0        0      239 2023-07-04 20:35:06.226429 django_ninja_crud-0.2.0/ninja_crud/schemas.py
+-rw-r--r--   0        0        0      646 2023-07-04 20:35:06.226429 django_ninja_crud-0.2.0/ninja_crud/tests/__init__.py
+-rw-r--r--   0        0        0     6439 2023-07-04 20:35:06.230429 django_ninja_crud-0.2.0/ninja_crud/tests/test_abstract.py
+-rw-r--r--   0        0        0     4610 2023-07-04 20:35:06.230429 django_ninja_crud-0.2.0/ninja_crud/tests/test_create.py
+-rw-r--r--   0        0        0     2855 2023-07-04 20:35:06.230429 django_ninja_crud-0.2.0/ninja_crud/tests/test_delete.py
+-rw-r--r--   0        0        0     5050 2023-07-04 20:35:06.230429 django_ninja_crud-0.2.0/ninja_crud/tests/test_list.py
+-rw-r--r--   0        0        0     3235 2023-07-04 20:35:06.230429 django_ninja_crud-0.2.0/ninja_crud/tests/test_retrieve.py
+-rw-r--r--   0        0        0     4565 2023-07-04 20:35:06.230429 django_ninja_crud-0.2.0/ninja_crud/tests/test_update.py
+-rw-r--r--   0        0        0      303 2023-07-04 20:35:06.230429 django_ninja_crud-0.2.0/ninja_crud/tests/utils.py
+-rw-r--r--   0        0        0      409 2023-07-04 20:35:06.230429 django_ninja_crud-0.2.0/ninja_crud/views/__init__.py
+-rw-r--r--   0        0        0      794 2023-07-04 20:35:06.230429 django_ninja_crud-0.2.0/ninja_crud/views/abstract.py
+-rw-r--r--   0        0        0     4244 2023-07-04 20:35:06.230429 django_ninja_crud-0.2.0/ninja_crud/views/create.py
+-rw-r--r--   0        0        0     1678 2023-07-04 20:35:06.230429 django_ninja_crud-0.2.0/ninja_crud/views/delete.py
+-rw-r--r--   0        0        0     4541 2023-07-04 20:35:06.230429 django_ninja_crud-0.2.0/ninja_crud/views/list.py
+-rw-r--r--   0        0        0     1792 2023-07-04 20:35:06.230429 django_ninja_crud-0.2.0/ninja_crud/views/retrieve.py
+-rw-r--r--   0        0        0     2082 2023-07-04 20:35:06.230429 django_ninja_crud-0.2.0/ninja_crud/views/update.py
+-rw-r--r--   0        0        0     1121 2023-07-04 20:35:06.230429 django_ninja_crud-0.2.0/ninja_crud/views/utils.py
+-rw-r--r--   0        0        0     1611 2023-07-04 20:35:06.230429 django_ninja_crud-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9207 1970-01-01 00:00:00.000000 django_ninja_crud-0.2.0/PKG-INFO
```

### Comparing `django_ninja_crud-0.1.3/LICENSE` & `django_ninja_crud-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ninja_crud-0.1.3/README.md` & `django_ninja_crud-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Django Ninja CRUD
 [![example workflow](https://github.com/hbakri/django-ninja-crud/actions/workflows/tests.yml/badge.svg)](https://github.com/hbakri/django-ninja-crud/actions)
 [![Coverage](https://img.shields.io/codecov/c/github/hbakri/django-ninja-crud/main.svg?label=coverage&logo=codecov&logoColor=white)](https://codecov.io/gh/hbakri/django-ninja-crud)
-[![PyPI version](https://img.shields.io/pypi/v/django-ninja-crud?color=g&logo=python&logoColor=white)](https://pypi.org/project/django-ninja-crud/)
-[![Downloads](https://pepy.tech/badge/django-ninja-crud)](https://pepy.tech/project/django-ninja-crud)
-[![License: MIT](https://img.shields.io/badge/license-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://img.shields.io/pypi/v/django-ninja-crud?color=g&logo=pypi&logoColor=white)](https://pypi.org/project/django-ninja-crud/)
+[![Downloads](https://pepy.tech/badge/django-ninja-crud/month)](https://pepy.tech/project/django-ninja-crud)
+[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 ![Django Ninja CRUD](https://media.discordapp.net/attachments/1093869226202234930/1117550925083590677/Hicham_B._Django-ninja_cover_ce78724c-1512-41e5-86de-3ffa2cfd0ea9.png?width=2688&height=1070)
 
 Django Ninja CRUD is a powerful tool designed to streamline the development of **CRUD** (**C**reate, **R**ead, **U**pdate, **D**elete) operations in Django applications using the [Django Ninja](https://django-ninja.rest-framework.com) framework. It is intended to help developers save significant time by eliminating the need to write repetitive code for each operation and even more on the associated tests.
 
 Developing these features from scratch every time can be _time-consuming_ and _error-prone_. That's where Django Ninja CRUD comes in—it provides a set of predefined, customizable "blueprints" for these operations, allowing developers to set them up quickly and reliably. Instead of getting bogged down with the details of how these operations are performed, developers can focus on the unique, creative aspects of their applications.
 
@@ -19,18 +19,16 @@
 - **Transparency:** _What you see is what you get_. The operations you define are the operations you perform, making it easy to understand and follow the data flow. It encourages practices that make your code easy to read and maintain. Also, it allows for easy testing of the defined operations, ensuring that everything works as expected.
 - **Configurability:** _Provides a high degree of customization_. You're not locked into a rigid structure; instead, you can adjust and fine-tune your operations to suit your project's unique needs. You can use the built-in tools to quickly set up standard operations, and if needed, you can customize them or even build your own from scratch.
 
 By using this package, developers can write efficient and clear code, saving time and reducing potential errors. It's a tool that accommodates the developer's workflow, rather than forcing the developer to adapt to it.
 
 ## 📝 Requirements
 
-![Python versions](https://img.shields.io/badge/python-3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11-blue)
-
+![Python versions](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11-blue)
 ![Django versions](https://img.shields.io/badge/django-3.2%20|%204.1%20|%204.2-blue)
-
 ![Django Ninja versions](https://img.shields.io/badge/django--ninja-0.21.0%20|%200.22.0-blue)
 
 ## 📈 Installation
 ```bash
 pip install django-ninja-crud
 ```
 For more information, see the [installation guide](https://django-ninja-crud.readme.io/docs/installation).
@@ -95,44 +93,44 @@
 
 ```python
 # tests.py
 from django.test import TestCase
 from example.models import Department
 from example.views.view_department import DepartmentViewSet
 from ninja_crud.tests import CreateModelViewTest, DeleteModelViewTest, \
-    ListModelViewTest, ModelViewSetTest, Payloads, RetrieveModelViewTest, \
-    UpdateModelViewTest
+    ListModelViewTest, ModelViewSetTest, RetrieveModelViewTest, UpdateModelViewTest, \
+    BodyParams, PathParams
 
 
 class DepartmentViewSetTest(ModelViewSetTest, TestCase):
     model_view_set = DepartmentViewSet
 
     @classmethod
     def setUpTestData(cls):
         super().setUpTestData()
         cls.department_1 = Department.objects.create(title="department-1")
         cls.department_2 = Department.objects.create(title="department-2")
 
-    def get_instance(self):
-        return self.department_1
+    def get_path_params(self):
+        return PathParams(ok={"id": self.department_1.id}, not_found={"id": 9999})
 
-    department_payloads = Payloads(
-        ok={"title": "department-updated"},
-        bad_request={"bad-key": "department-updated"},
+    body_params = BodyParams(
+        ok={"title": "new_title"},
+        bad_request={"bad-title": 1},
         conflict={"title": "department-2"},
     )
 
-    test_list = ListModelViewTest(instance_getter=get_instance)
-    test_create = CreateModelViewTest(payloads=department_payloads, instance_getter=get_instance)
-    test_retrieve = RetrieveModelViewTest(instance_getter=get_instance)
-    test_update = UpdateModelViewTest(payloads=department_payloads, instance_getter=get_instance)
-    test_delete = DeleteModelViewTest(instance_getter=get_instance)
+    test_list = ListModelViewTest()
+    test_create = CreateModelViewTest(body_params=body_params)
+    test_retrieve = RetrieveModelViewTest(path_params=get_path_params)
+    test_update = UpdateModelViewTest(path_params=get_path_params, body_params=body_params)
+    test_delete = DeleteModelViewTest(path_params=get_path_params)
 ```
-With this package, these tests can be written in a consistent, straightforward way, making it easier to ensure your views are working as expected. Once you've written these tests, you can run them whenever you make changes to your views, giving you confidence that your changes haven't broken anything.
+With this package, these tests can be written in a consistent, straightforward way, making it easier to ensure your views are working as expected.
 
 In summary, this package simplifies the process of setting up and testing **CRUD** operations in Django Ninja, letting you focus on what makes your application unique. By providing a flexible, transparent, and configurable solution, this package is a powerful tool for accelerating web development.
 
 ## 📚 Documentation
-https://django-ninja-crud.readme.io/docs
+For more information, see the [documentation](https://django-ninja-crud.readme.io/docs).
 
 ## 🫶 Support
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/hbakri)
```

### Comparing `django_ninja_crud-0.1.3/ninja_crud/tests/test_abstract.py` & `django_ninja_crud-0.2.0/ninja_crud/tests/test_abstract.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,94 @@
 import inspect
 import json
 from http import HTTPStatus
-from typing import Callable, List, NamedTuple, Optional, Tuple, Type
+from typing import Callable, List, NamedTuple, Optional, Tuple, Type, TypeVar, Union
 
 from django.db.models import Model, QuerySet
 from django.http import HttpResponse
 from django.test import Client, TestCase
 from ninja import Schema
 
 from ninja_crud.tests.utils import default_serializer
 from ninja_crud.views import (
     AbstractModelView,
     CreateModelView,
     ListModelView,
     ModelViewSet,
 )
 
+T = TypeVar("T")
+TestCaseType = TypeVar("TestCaseType", bound=TestCase)
+ArgOrCallable = Union[T, Callable[[TestCaseType], T]]
 
-class Credentials(NamedTuple):
+
+class PathParams(NamedTuple):
+    ok: dict
+    not_found: Optional[dict] = None
+
+
+class QueryParams(NamedTuple):
+    ok: dict
+    bad_request: Optional[dict] = None
+
+
+class AuthParams(NamedTuple):
     ok: dict
     forbidden: Optional[dict] = None
     unauthorized: Optional[dict] = None
 
 
-class Payloads(NamedTuple):
+class BodyParams(NamedTuple):
     ok: dict
     bad_request: Optional[dict] = None
     conflict: Optional[dict] = None
 
 
-def default_credentials_getter(_: TestCase) -> Credentials:
-    return Credentials(ok={})
-
-
 class AbstractModelViewTest:
     model_view_set: ModelViewSet
     test_case: TestCase
     client: Client
     model_view: Type[AbstractModelView]
     name: str
 
     def __init__(
         self,
-        instance_getter: Callable[[TestCase], Model],
-        credentials_getter: Callable[[TestCase], Credentials] = None,
+        path_params: ArgOrCallable[PathParams, TestCaseType] = None,
+        query_params: ArgOrCallable[QueryParams, TestCaseType] = None,
+        auth_params: ArgOrCallable[AuthParams, TestCaseType] = None,
+        body_params: ArgOrCallable[BodyParams, TestCaseType] = None,
     ) -> None:
-        self.get_instance = instance_getter
-        if credentials_getter is None:
-            credentials_getter = default_credentials_getter
-        self.get_credentials = credentials_getter
+        if path_params is None:
+            path_params = PathParams(ok={})
+        if auth_params is None:
+            auth_params = AuthParams(ok={})
+        if body_params is None:
+            body_params = BodyParams(ok={})
+
+        self.path_params = path_params
+        self.query_params = query_params
+        self.auth_params = auth_params
+        self.body_params = body_params
+
+    def get_abstract_params(self, params: ArgOrCallable[T, TestCaseType]) -> T:
+        return params(self.test_case) if callable(params) else params
+
+    def get_path_params(self) -> PathParams:
+        return self.get_abstract_params(self.path_params)
+
+    def get_query_params(self) -> QueryParams:
+        return self.get_abstract_params(self.query_params)
+
+    def get_auth_params(self) -> AuthParams:
+        return self.get_abstract_params(self.auth_params)
+
+    def get_body_params(self) -> BodyParams:
+        return self.get_abstract_params(self.body_params)
 
-    def get_tests(self) -> List[Tuple[str, Callable]]:
+    def get_test_methods(self) -> List[Tuple[str, Callable]]:
         return [
             (name, method)
             for name, method in inspect.getmembers(self, predicate=inspect.ismethod)
             if name.startswith("test")
         ]
 
     def get_model_view(self):
@@ -132,15 +166,15 @@
         for attr_name in dir(new_cls):
             attr_value = getattr(new_cls, attr_name)
             if isinstance(attr_value, AbstractModelViewTest):
                 attr_value.model_view_set = new_cls.model_view_set
                 attr_value.test_case = test_case
                 attr_value.client = new_cls.client_class()
                 attr_value.name = attr_name
-                for test_name, test_func in attr_value.get_tests():
+                for test_name, test_func in attr_value.get_test_methods():
                     method = attr_value.get_model_view()
                     model_name = new_cls.model_view_set.model.__name__.lower()
                     substring_replace = model_name
                     if isinstance(method, (ListModelView, CreateModelView)):
                         if method.detail:
                             related_model_name = method.related_model.__name__.lower()
                             substring_replace = f"{model_name}_{related_model_name}"
```

### Comparing `django_ninja_crud-0.1.3/ninja_crud/views/abstract.py` & `django_ninja_crud-0.2.0/ninja_crud/views/abstract.py`

 * *Files identical despite different names*

### Comparing `django_ninja_crud-0.1.3/ninja_crud/views/create.py` & `django_ninja_crud-0.2.0/ninja_crud/views/create.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 from http import HTTPStatus
-from typing import Callable, List, Type, Union
-from uuid import UUID
+from typing import Any, Callable, List, Type, Union
 
 from django.db.models import Model
 from django.http import HttpRequest
 from ninja import Router, Schema
 
-from ninja_crud import utils
-from ninja_crud.utils import merge_decorators
+from ninja_crud.views import utils
 from ninja_crud.views.abstract import AbstractModelView
 
 
 class CreateModelView(AbstractModelView):
     def __init__(
         self,
         input_schema: Type[Schema],
         output_schema: Type[Schema],
         decorators: List[Callable] = None,
         detail: bool = False,
         related_model: Type[Model] = None,
         pre_save: Union[
             Callable[[HttpRequest, Model], None],
-            Callable[[HttpRequest, Union[int, UUID], Model], None],
+            Callable[[HttpRequest, Any, Model], None],
         ] = None,
         post_save: Union[
             Callable[[HttpRequest, Model], None],
-            Callable[[HttpRequest, Union[int, UUID], Model], None],
+            Callable[[HttpRequest, Any, Model], None],
         ] = None,
     ) -> None:
         super().__init__(decorators=decorators)
         self.input_schema = input_schema
         self.output_schema = output_schema
         self.detail = detail
         self.related_model = related_model
@@ -49,19 +47,19 @@
 
         input_schema = self.input_schema
         output_schema = self.output_schema
 
         @router.post(
             "/",
             response={HTTPStatus.CREATED: output_schema},
-            url_name=f"{model_name}s",
+            url_name=self.get_url_name(model),
             operation_id=operation_id,
             summary=summary,
         )
-        @merge_decorators(self.decorators)
+        @utils.merge_decorators(self.decorators)
         def create_model(request: HttpRequest, payload: input_schema):
             instance = model()
             for field, value in payload.dict(exclude_unset=True).items():
                 setattr(instance, field, value)
             if self.pre_save:
                 self.pre_save(request, instance)
             instance.full_clean()
@@ -71,34 +69,42 @@
             return HTTPStatus.CREATED, instance
 
     def register_instance_route(self, router: Router, model: Type[Model]) -> None:
         parent_model_name = utils.to_snake_case(model.__name__)
         model_name = utils.to_snake_case(self.related_model.__name__)
         plural_model_name = f"{model_name}s"
         url = "/{id}/" + plural_model_name
-        operation_id = f"create_{parent_model_name}_{plural_model_name}"
-        summary = f"Create {self.related_model.__name__} of a {model.__name__}"
+        operation_id = f"create_{parent_model_name}_{model_name}"
+        summary = f"Create {self.related_model.__name__}"
 
         input_schema = self.input_schema
         output_schema = self.output_schema
+        id_type = utils.get_id_type(model)
 
         @router.post(
             url,
             response={HTTPStatus.CREATED: output_schema},
-            url_name=f"{parent_model_name}_{plural_model_name}",
+            url_name=self.get_url_name(model),
             operation_id=operation_id,
             summary=summary,
         )
-        @merge_decorators(self.decorators)
-        def create_model(
-            request: HttpRequest, id: Union[int, UUID], payload: input_schema
-        ):
-            instance = self.related_model()
+        @utils.merge_decorators(self.decorators)
+        def create_model(request: HttpRequest, id: id_type, payload: input_schema):
+            instance = model.objects.get(pk=id)
+            related_instance = self.related_model()
             for field, value in payload.dict(exclude_unset=True).items():
-                setattr(instance, field, value)
+                setattr(related_instance, field, value)
             if self.pre_save:
-                self.pre_save(request, id, instance)
-            instance.full_clean()
-            instance.save()
+                self.pre_save(request, instance.pk, related_instance)
+            related_instance.full_clean()
+            related_instance.save()
             if self.post_save:
-                self.post_save(request, id, instance)
-            return HTTPStatus.CREATED, instance
+                self.post_save(request, instance.pk, related_instance)
+            return HTTPStatus.CREATED, related_instance
+
+    def get_url_name(self, model: Type[Model]) -> str:
+        model_name = utils.to_snake_case(model.__name__)
+        if self.detail:
+            related_model_name = utils.to_snake_case(self.related_model.__name__)
+            return f"{model_name}_{related_model_name}s"
+        else:
+            return f"{model_name}s"
```

### Comparing `django_ninja_crud-0.1.3/ninja_crud/views/delete.py` & `django_ninja_crud-0.2.0/ninja_crud/views/delete.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 from http import HTTPStatus
-from typing import Callable, List, Type, Union
-from uuid import UUID
+from typing import Any, Callable, List, Type
 
 from django.db.models import Model
 from django.http import HttpRequest
 from ninja import Router
 
-from ninja_crud import utils
-from ninja_crud.utils import merge_decorators
+from ninja_crud.views import utils
 from ninja_crud.views.abstract import AbstractModelView
 
 
 class DeleteModelView(AbstractModelView):
     def __init__(
         self,
         decorators: List[Callable] = None,
         pre_delete: Callable[[HttpRequest, Model], None] = None,
-        post_delete: Callable[[HttpRequest, Union[int, UUID]], None] = None,
+        post_delete: Callable[[HttpRequest, Any], None] = None,
     ) -> None:
         super().__init__(decorators=decorators)
         self.pre_delete = pre_delete
         self.post_delete = post_delete
 
     def register_route(self, router: Router, model: Type[Model]) -> None:
         model_name = utils.to_snake_case(model.__name__)
         operation_id = f"delete_{model_name}"
         summary = f"Delete {model.__name__}"
+        id_type = utils.get_id_type(model)
 
         @router.delete(
             "/{id}",
             response={HTTPStatus.NO_CONTENT: None},
-            url_name=model_name,
+            url_name=self.get_url_name(model),
             operation_id=operation_id,
             summary=summary,
         )
-        @merge_decorators(self.decorators)
-        def delete_model(request: HttpRequest, id: Union[int, UUID]):
+        @utils.merge_decorators(self.decorators)
+        def delete_model(request: HttpRequest, id: id_type):
             instance = model.objects.get(pk=id)
             if self.pre_delete is not None:
                 self.pre_delete(request, instance)
             instance.delete()
             if self.post_delete is not None:
                 self.post_delete(request, id)
             return HTTPStatus.NO_CONTENT, None
+
+    @staticmethod
+    def get_url_name(model: Type[Model]) -> str:
+        return utils.to_snake_case(model.__name__)
```

### Comparing `django_ninja_crud-0.1.3/ninja_crud/views/list.py` & `django_ninja_crud-0.2.0/ninja_crud/views/list.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from http import HTTPStatus
-from typing import Callable, List, Type, Union
-from uuid import UUID
+from typing import Any, Callable, List, Type, Union
 
 from django.db.models import Model, QuerySet
 from django.http import HttpRequest
 from ninja import FilterSchema, Query, Router, Schema
 from ninja.pagination import LimitOffsetPagination, paginate
 
-from ninja_crud import utils
-from ninja_crud.utils import merge_decorators
+from ninja_crud.views import utils
 from ninja_crud.views.abstract import AbstractModelView
 
 
 class ListModelView(AbstractModelView):
     def __init__(
         self,
         output_schema: Type[Schema],
         filter_schema: Type[FilterSchema] = None,
         queryset_getter: Union[
-            Callable[[], QuerySet[Model]], Callable[[Union[int, UUID]], QuerySet[Model]]
+            Callable[[], QuerySet[Model]], Callable[[Any], QuerySet[Model]]
         ] = None,
         related_model: Type[Model] = None,
         detail: bool = False,
         decorators: List[Callable] = None,
     ) -> None:
         super().__init__(decorators=decorators)
         self.output_schema = output_schema
         self.filter_schema = filter_schema
-        self.get_queryset = queryset_getter
+        self.queryset_getter = queryset_getter
         self.related_model = related_model
         self.detail = detail
 
     def register_route(self, router: Router, model: Type[Model]) -> None:
         if self.detail:
             self.register_instance_route(router, model)
         else:
@@ -44,61 +42,77 @@
 
         output_schema = self.output_schema
         filter_schema = self.filter_schema
 
         @router.get(
             "/",
             response={HTTPStatus.OK: List[output_schema]},
-            url_name=f"{model_name}s",
+            url_name=self.get_url_name(model),
             operation_id=operation_id,
             summary=summary,
         )
-        @merge_decorators(self.decorators)
+        @utils.merge_decorators(self.decorators)
         @paginate(LimitOffsetPagination)
         def list_models(
             request: HttpRequest, filters: filter_schema = Query(default=FilterSchema())
         ):
-            if self.get_queryset is not None:
-                queryset = self.get_queryset()
-            else:
-                queryset = model.objects.get_queryset()
+            queryset = self.get_queryset(model)
             return self.filter_queryset(queryset=queryset, filters=filters)
 
     def register_instance_route(self, router: Router, model: Type[Model]) -> None:
         parent_model_name = utils.to_snake_case(model.__name__)
         model_name = utils.to_snake_case(self.related_model.__name__)
         plural_model_name = f"{model_name}s"
         url = "/{id}/" + plural_model_name
         operation_id = f"list_{parent_model_name}_{plural_model_name}"
         summary = f"List {self.related_model.__name__}s of a {model.__name__}"
 
         output_schema = self.output_schema
         filter_schema = self.filter_schema
+        id_type = utils.get_id_type(model)
 
         @router.get(
             url,
             response={HTTPStatus.OK: List[output_schema]},
-            url_name=f"{parent_model_name}_{plural_model_name}",
+            url_name=self.get_url_name(model),
             operation_id=operation_id,
             summary=summary,
         )
-        @merge_decorators(self.decorators)
+        @utils.merge_decorators(self.decorators)
         @paginate(LimitOffsetPagination)
         def list_models(
             request: HttpRequest,
-            id: Union[int, UUID],
+            id: id_type,
             filters: filter_schema = Query(default=FilterSchema()),
         ):
-            if self.get_queryset is not None:
-                queryset = self.get_queryset(id)
-            else:
-                queryset = self.related_model.objects.get_queryset()
+            instance = model.objects.get(pk=id)
+            queryset = self.get_queryset(model, instance.pk)
             return self.filter_queryset(queryset=queryset, filters=filters)
 
+    def get_queryset(self, model: Type[Model], id: Any = None) -> QuerySet[Model]:
+        if self.detail:
+            if self.queryset_getter is not None:
+                return self.queryset_getter(id)
+            else:
+                return self.related_model.objects.get_queryset()
+        else:
+            if self.queryset_getter is not None:
+                return self.queryset_getter()
+            else:
+                return model.objects.get_queryset()
+
     @staticmethod
     def filter_queryset(queryset: QuerySet[Model], filters: FilterSchema):
         filters_dict = filters.dict()
         if "order_by" in filters_dict and filters_dict["order_by"] is not None:
             queryset = queryset.order_by(*filters_dict.pop("order_by"))
 
         queryset = filters.filter(queryset)
         return queryset
+
+    def get_url_name(self, model: Type[Model]) -> str:
+        model_name = utils.to_snake_case(model.__name__)
+        if self.detail:
+            related_model_name = utils.to_snake_case(self.related_model.__name__)
+            return f"{model_name}_{related_model_name}s"
+        else:
+            return f"{model_name}s"
```

### Comparing `django_ninja_crud-0.1.3/ninja_crud/views/retrieve.py` & `django_ninja_crud-0.2.0/ninja_crud/views/retrieve.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 from http import HTTPStatus
-from typing import Callable, List, Type, Union
-from uuid import UUID
+from typing import Any, Callable, List, Type
 
 from django.db.models import Model, QuerySet
 from django.http import HttpRequest
 from ninja import Router, Schema
 
-from ninja_crud import utils
-from ninja_crud.utils import merge_decorators
+from ninja_crud.views import utils
 from ninja_crud.views.abstract import AbstractModelView
 
 
 class RetrieveModelView(AbstractModelView):
     def __init__(
         self,
         output_schema: Type[Schema],
-        queryset_getter: Callable[[UUID], QuerySet[Model]] = None,
+        queryset_getter: Callable[[Any], QuerySet[Model]] = None,
         decorators: List[Callable] = None,
     ) -> None:
         super().__init__(decorators=decorators)
         self.output_schema = output_schema
-        self.get_queryset = queryset_getter
+        self.queryset_getter = queryset_getter
 
     def register_route(self, router: Router, model: Type[Model]) -> None:
         model_name = utils.to_snake_case(model.__name__)
         operation_id = f"retrieve_{model_name}"
         summary = f"Retrieve {model.__name__}"
 
         output_schema = self.output_schema
+        id_type = utils.get_id_type(model)
 
         @router.get(
             "/{id}",
             response={HTTPStatus.OK: output_schema},
-            url_name=model_name,
+            url_name=self.get_url_name(model),
             operation_id=operation_id,
             summary=summary,
         )
-        @merge_decorators(self.decorators)
-        def retrieve_model(request: HttpRequest, id: Union[int, UUID]):
-            if self.get_queryset is not None:
-                queryset = self.get_queryset(id)
-            else:
-                queryset = model.objects.get_queryset()
+        @utils.merge_decorators(self.decorators)
+        def retrieve_model(request: HttpRequest, id: id_type):
+            queryset = self.get_queryset(model, id)
             instance = queryset.get(pk=id)
             return HTTPStatus.OK, instance
+
+    def get_queryset(self, model: Type[Model], id: Any = None) -> QuerySet[Model]:
+        if self.queryset_getter is None:
+            return model.objects.get_queryset()
+        else:
+            return self.queryset_getter(id)
+
+    @staticmethod
+    def get_url_name(model: Type[Model]) -> str:
+        return utils.to_snake_case(model.__name__)
```

### Comparing `django_ninja_crud-0.1.3/ninja_crud/views/update.py` & `django_ninja_crud-0.2.0/ninja_crud/views/update.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from http import HTTPStatus
-from typing import Callable, List, Type, Union
-from uuid import UUID
+from typing import Callable, List, Type
 
 from django.db.models import Model
 from django.http import HttpRequest
 from ninja import Router, Schema
 
-from ninja_crud import utils
-from ninja_crud.utils import merge_decorators
+from ninja_crud.views import utils
 from ninja_crud.views.abstract import AbstractModelView
 
 
 class UpdateModelView(AbstractModelView):
     def __init__(
         self,
         input_schema: Type[Schema],
@@ -29,29 +27,32 @@
     def register_route(self, router: Router, model: Type[Model]) -> None:
         model_name = utils.to_snake_case(model.__name__)
         operation_id = f"update_{model_name}"
         summary = f"Update {model.__name__}"
 
         input_schema = self.input_schema
         output_schema = self.output_schema
+        id_type = utils.get_id_type(model)
 
         @router.put(
             "/{id}",
             response={HTTPStatus.OK: output_schema},
-            url_name=model_name,
+            url_name=self.get_url_name(model),
             operation_id=operation_id,
             summary=summary,
         )
-        @merge_decorators(self.decorators)
-        def update_model(
-            request: HttpRequest, id: Union[int, UUID], payload: input_schema
-        ):
-            instance = model.objects.get(id=id)
+        @utils.merge_decorators(self.decorators)
+        def update_model(request: HttpRequest, id: id_type, payload: input_schema):
+            instance = model.objects.get(pk=id)
             for field, value in payload.dict(exclude_unset=True).items():
                 setattr(instance, field, value)
             if self.pre_save is not None:
                 self.pre_save(request, instance)
             instance.full_clean()
             instance.save()
             if self.post_save is not None:
                 self.post_save(request, instance)
             return HTTPStatus.OK, instance
+
+    @staticmethod
+    def get_url_name(model: Type[Model]) -> str:
+        return utils.to_snake_case(model.__name__)
```

### Comparing `django_ninja_crud-0.1.3/pyproject.toml` & `django_ninja_crud-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 src_paths = ["ninja_crud", "tests", "examples"]
 
 [tool.pycln]
 all = true
 
 [tool.poetry]
 name = "django-ninja-crud"
-version = "0.1.3"
+version = "0.2.0"
 description = "Django Ninja CRUD is a library that allows you to create CRUD APIs in a few lines of code."
 authors = ["Hicham Bakri <hicham.bakri76@gmail.com>"]
 maintainers = ["Hicham Bakri <hicham.bakri76@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/hbakri/django-ninja-crud"
 license = "MIT"
 classifiers = [
@@ -34,15 +34,15 @@
     "Framework :: AsyncIO",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 packages = [{ include = "ninja_crud" },]
 
 [tool.poetry.dependencies]
-python = ">= 3.7"
+python = ">= 3.8"
 Django = ">= 3.2"
 django-ninja = ">= 0.21"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^6.5.0"
 pre-commit = "^2.20.0"
```

### Comparing `django_ninja_crud-0.1.3/PKG-INFO` & `django_ninja_crud-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: django-ninja-crud
-Version: 0.1.3
+Version: 0.2.0
 Summary: Django Ninja CRUD is a library that allows you to create CRUD APIs in a few lines of code.
 Home-page: https://github.com/hbakri/django-ninja-crud
 License: MIT
 Author: Hicham Bakri
 Author-email: hicham.bakri76@gmail.com
 Maintainer: Hicham Bakri
 Maintainer-email: hicham.bakri76@gmail.com
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
@@ -36,17 +35,17 @@
 Requires-Dist: Django (>=3.2)
 Requires-Dist: django-ninja (>=0.21)
 Description-Content-Type: text/markdown
 
 # Django Ninja CRUD
 [![example workflow](https://github.com/hbakri/django-ninja-crud/actions/workflows/tests.yml/badge.svg)](https://github.com/hbakri/django-ninja-crud/actions)
 [![Coverage](https://img.shields.io/codecov/c/github/hbakri/django-ninja-crud/main.svg?label=coverage&logo=codecov&logoColor=white)](https://codecov.io/gh/hbakri/django-ninja-crud)
-[![PyPI version](https://img.shields.io/pypi/v/django-ninja-crud?color=g&logo=python&logoColor=white)](https://pypi.org/project/django-ninja-crud/)
-[![Downloads](https://pepy.tech/badge/django-ninja-crud)](https://pepy.tech/project/django-ninja-crud)
-[![License: MIT](https://img.shields.io/badge/license-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://img.shields.io/pypi/v/django-ninja-crud?color=g&logo=pypi&logoColor=white)](https://pypi.org/project/django-ninja-crud/)
+[![Downloads](https://pepy.tech/badge/django-ninja-crud/month)](https://pepy.tech/project/django-ninja-crud)
+[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 ![Django Ninja CRUD](https://media.discordapp.net/attachments/1093869226202234930/1117550925083590677/Hicham_B._Django-ninja_cover_ce78724c-1512-41e5-86de-3ffa2cfd0ea9.png?width=2688&height=1070)
 
 Django Ninja CRUD is a powerful tool designed to streamline the development of **CRUD** (**C**reate, **R**ead, **U**pdate, **D**elete) operations in Django applications using the [Django Ninja](https://django-ninja.rest-framework.com) framework. It is intended to help developers save significant time by eliminating the need to write repetitive code for each operation and even more on the associated tests.
 
 Developing these features from scratch every time can be _time-consuming_ and _error-prone_. That's where Django Ninja CRUD comes in—it provides a set of predefined, customizable "blueprints" for these operations, allowing developers to set them up quickly and reliably. Instead of getting bogged down with the details of how these operations are performed, developers can focus on the unique, creative aspects of their applications.
 
@@ -58,18 +57,16 @@
 - **Transparency:** _What you see is what you get_. The operations you define are the operations you perform, making it easy to understand and follow the data flow. It encourages practices that make your code easy to read and maintain. Also, it allows for easy testing of the defined operations, ensuring that everything works as expected.
 - **Configurability:** _Provides a high degree of customization_. You're not locked into a rigid structure; instead, you can adjust and fine-tune your operations to suit your project's unique needs. You can use the built-in tools to quickly set up standard operations, and if needed, you can customize them or even build your own from scratch.
 
 By using this package, developers can write efficient and clear code, saving time and reducing potential errors. It's a tool that accommodates the developer's workflow, rather than forcing the developer to adapt to it.
 
 ## 📝 Requirements
 
-![Python versions](https://img.shields.io/badge/python-3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11-blue)
-
+![Python versions](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11-blue)
 ![Django versions](https://img.shields.io/badge/django-3.2%20|%204.1%20|%204.2-blue)
-
 ![Django Ninja versions](https://img.shields.io/badge/django--ninja-0.21.0%20|%200.22.0-blue)
 
 ## 📈 Installation
 ```bash
 pip install django-ninja-crud
 ```
 For more information, see the [installation guide](https://django-ninja-crud.readme.io/docs/installation).
@@ -134,45 +131,45 @@
 
 ```python
 # tests.py
 from django.test import TestCase
 from example.models import Department
 from example.views.view_department import DepartmentViewSet
 from ninja_crud.tests import CreateModelViewTest, DeleteModelViewTest, \
-    ListModelViewTest, ModelViewSetTest, Payloads, RetrieveModelViewTest, \
-    UpdateModelViewTest
+    ListModelViewTest, ModelViewSetTest, RetrieveModelViewTest, UpdateModelViewTest, \
+    BodyParams, PathParams
 
 
 class DepartmentViewSetTest(ModelViewSetTest, TestCase):
     model_view_set = DepartmentViewSet
 
     @classmethod
     def setUpTestData(cls):
         super().setUpTestData()
         cls.department_1 = Department.objects.create(title="department-1")
         cls.department_2 = Department.objects.create(title="department-2")
 
-    def get_instance(self):
-        return self.department_1
+    def get_path_params(self):
+        return PathParams(ok={"id": self.department_1.id}, not_found={"id": 9999})
 
-    department_payloads = Payloads(
-        ok={"title": "department-updated"},
-        bad_request={"bad-key": "department-updated"},
+    body_params = BodyParams(
+        ok={"title": "new_title"},
+        bad_request={"bad-title": 1},
         conflict={"title": "department-2"},
     )
 
-    test_list = ListModelViewTest(instance_getter=get_instance)
-    test_create = CreateModelViewTest(payloads=department_payloads, instance_getter=get_instance)
-    test_retrieve = RetrieveModelViewTest(instance_getter=get_instance)
-    test_update = UpdateModelViewTest(payloads=department_payloads, instance_getter=get_instance)
-    test_delete = DeleteModelViewTest(instance_getter=get_instance)
+    test_list = ListModelViewTest()
+    test_create = CreateModelViewTest(body_params=body_params)
+    test_retrieve = RetrieveModelViewTest(path_params=get_path_params)
+    test_update = UpdateModelViewTest(path_params=get_path_params, body_params=body_params)
+    test_delete = DeleteModelViewTest(path_params=get_path_params)
 ```
-With this package, these tests can be written in a consistent, straightforward way, making it easier to ensure your views are working as expected. Once you've written these tests, you can run them whenever you make changes to your views, giving you confidence that your changes haven't broken anything.
+With this package, these tests can be written in a consistent, straightforward way, making it easier to ensure your views are working as expected.
 
 In summary, this package simplifies the process of setting up and testing **CRUD** operations in Django Ninja, letting you focus on what makes your application unique. By providing a flexible, transparent, and configurable solution, this package is a powerful tool for accelerating web development.
 
 ## 📚 Documentation
-https://django-ninja-crud.readme.io/docs
+For more information, see the [documentation](https://django-ninja-crud.readme.io/docs).
 
 ## 🫶 Support
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/hbakri)
```

