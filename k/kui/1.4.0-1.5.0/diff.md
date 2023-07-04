# Comparing `tmp/kui-1.4.0.tar.gz` & `tmp/kui-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kui-1.4.0.tar", last modified: Mon Jun  5 05:55:36 2023, max compression
+gzip compressed data, was "kui-1.5.0.tar", last modified: Tue Jul  4 09:19:35 2023, max compression
```

## Comparing `kui-1.4.0.tar` & `kui-1.5.0.tar`

### file list

```diff
@@ -1,86 +1,88 @@
--rw-r--r--   0        0        0    11341 2023-06-05 05:55:19.288698 kui-1.4.0/LICENSE
--rw-r--r--   0        0        0      440 2023-06-05 05:55:19.288698 kui-1.4.0/README.md
--rw-r--r--   0        0        0        0 2023-06-05 05:55:19.288698 kui-1.4.0/kui/__init__.py
--rw-r--r--   0        0        0       63 2023-06-05 05:55:19.288698 kui-1.4.0/kui/__version__.py
--rw-r--r--   0        0        0     1754 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/__init__.py
--rw-r--r--   0        0        0     8405 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/applications.py
--rw-r--r--   0        0        0     2090 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/cors.py
--rw-r--r--   0        0        0     2366 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/exceptions.py
--rw-r--r--   0        0        0     1470 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/openapi.py
--rw-r--r--   0        0        0     5502 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/parameters.py
--rw-r--r--   0        0        0     3754 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/requests.py
--rw-r--r--   0        0        0     2879 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/responses.py
--rw-r--r--   0        0        0      972 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/routing.py
--rw-r--r--   0        0        0     3177 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/templates.py
--rw-r--r--   0        0        0     4614 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/views.py
--rw-r--r--   0        0        0      304 2023-06-05 05:55:19.288698 kui-1.4.0/kui/cors.py
--rw-r--r--   0        0        0     3849 2023-06-05 05:55:19.288698 kui-1.4.0/kui/exceptions.py
--rw-r--r--   0        0        0      123 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/__init__.py
--rw-r--r--   0        0        0     9465 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/application.py
--rw-r--r--   0        0        0     1565 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/extra_docs.py
--rw-r--r--   0        0        0     1632 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/schema.py
--rw-r--r--   0        0        0     7726 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/specification.py
--rw-r--r--   0        0        0      224 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/templates/rapidoc.html
--rw-r--r--   0        0        0      743 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/templates/redoc.html
--rw-r--r--   0        0        0     1522 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/templates/swagger.html
--rw-r--r--   0        0        0      586 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/types.py
--rw-r--r--   0        0        0    15327 2023-06-05 05:55:19.288698 kui-1.4.0/kui/parameters/__init__.py
--rw-r--r--   0        0        0     9051 2023-06-05 05:55:19.288698 kui-1.4.0/kui/parameters/field_functions.py
--rw-r--r--   0        0        0     2219 2023-06-05 05:55:19.288698 kui-1.4.0/kui/parameters/fields.py
--rw-r--r--   0        0        0        0 2023-06-05 05:55:19.288698 kui-1.4.0/kui/py.typed
--rw-r--r--   0        0        0     7577 2023-06-05 05:55:19.288698 kui-1.4.0/kui/responses.py
--rw-r--r--   0        0        0      429 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/__init__.py
--rw-r--r--   0        0        0       82 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/__main__.py
--rw-r--r--   0        0        0     1402 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/commands.py
--rw-r--r--   0        0        0      130 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/extensions/__init__.py
--rw-r--r--   0        0        0     2551 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/extensions/file.py
--rw-r--r--   0        0        0     2982 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/extensions/multimethod.py
--rw-r--r--   0        0        0    17890 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/routers.py
--rw-r--r--   0        0        0     3040 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/routes.py
--rw-r--r--   0        0        0     6234 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/tree.py
--rw-r--r--   0        0        0      273 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/typing.py
--rw-r--r--   0        0        0     2825 2023-06-05 05:55:19.288698 kui-1.4.0/kui/security.py
--rw-r--r--   0        0        0     2783 2023-06-05 05:55:19.288698 kui-1.4.0/kui/status.py
--rw-r--r--   0        0        0     1250 2023-06-05 05:55:19.288698 kui-1.4.0/kui/templates.py
--rw-r--r--   0        0        0      757 2023-06-05 05:55:19.288698 kui-1.4.0/kui/utils/__init__.py
--rw-r--r--   0        0        0      856 2023-06-05 05:55:19.288698 kui-1.4.0/kui/utils/contextvars.py
--rw-r--r--   0        0        0     1576 2023-06-05 05:55:19.288698 kui-1.4.0/kui/utils/importer.py
--rw-r--r--   0        0        0     1907 2023-06-05 05:55:19.288698 kui-1.4.0/kui/utils/inspect.py
--rw-r--r--   0        0        0     1647 2023-06-05 05:55:19.288698 kui-1.4.0/kui/utils/objects.py
--rw-r--r--   0        0        0      530 2023-06-05 05:55:19.288698 kui-1.4.0/kui/utils/pipe.py
--rw-r--r--   0        0        0     1123 2023-06-05 05:55:19.288698 kui-1.4.0/kui/utils/state.py
--rw-r--r--   0        0        0     1603 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/__init__.py
--rw-r--r--   0        0        0     5515 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/applications.py
--rw-r--r--   0        0        0     2067 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/cors.py
--rw-r--r--   0        0        0     2309 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/exceptions.py
--rw-r--r--   0        0        0     1428 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/openapi.py
--rw-r--r--   0        0        0     4204 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/parameters.py
--rw-r--r--   0        0        0     1833 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/requests.py
--rw-r--r--   0        0        0     2879 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/responses.py
--rw-r--r--   0        0        0      966 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/routing.py
--rw-r--r--   0        0        0     2884 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/templates.py
--rw-r--r--   0        0        0     2281 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/views.py
--rw-r--r--   0        0        0     2189 2023-06-05 05:55:19.292698 kui-1.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 05:55:19.292698 kui-1.4.0/tests/asgi/__init__.py
--rw-r--r--   0        0        0     2416 2023-06-05 05:55:19.292698 kui-1.4.0/tests/asgi/test_application.py
--rw-r--r--   0        0        0     1338 2023-06-05 05:55:19.292698 kui-1.4.0/tests/asgi/test_cors.py
--rw-r--r--   0        0        0     7058 2023-06-05 05:55:19.292698 kui-1.4.0/tests/asgi/test_parameters.py
--rw-r--r--   0        0        0      535 2023-06-05 05:55:19.292698 kui-1.4.0/tests/asgi/test_views.py
--rw-r--r--   0        0        0    32402 2023-06-05 05:55:19.292698 kui-1.4.0/tests/openapi/test_application.py
--rw-r--r--   0        0        0      429 2023-06-05 05:55:19.292698 kui-1.4.0/tests/openapi/test_extra_docs.py
--rw-r--r--   0        0        0      247 2023-06-05 05:55:19.292698 kui-1.4.0/tests/routing/extensions/test_fileroutes.py
--rw-r--r--   0        0        0     3155 2023-06-05 05:55:19.292698 kui-1.4.0/tests/routing/extensions/test_multimethod.py
--rw-r--r--   0        0        0       88 2023-06-05 05:55:19.292698 kui-1.4.0/tests/routing/test_commands.py
--rw-r--r--   0        0        0     4076 2023-06-05 05:55:19.292698 kui-1.4.0/tests/routing/test_routes.py
--rw-r--r--   0        0        0     2444 2023-06-05 05:55:19.292698 kui-1.4.0/tests/routing/test_tree.py
--rw-r--r--   0        0        0      242 2023-06-05 05:55:19.292698 kui-1.4.0/tests/test_export_all.py
--rw-r--r--   0        0        0     4505 2023-06-05 05:55:19.292698 kui-1.4.0/tests/test_responses.py
--rw-r--r--   0        0        0     3032 2023-06-05 05:55:19.292698 kui-1.4.0/tests/test_security.py
--rw-r--r--   0        0        0        0 2023-06-05 05:55:19.292698 kui-1.4.0/tests/utils/__init__.py
--rw-r--r--   0        0        0      722 2023-06-05 05:55:19.292698 kui-1.4.0/tests/utils/test_importer.py
--rw-r--r--   0        0        0      170 2023-06-05 05:55:19.292698 kui-1.4.0/tests/utils/test_objects.py
--rw-r--r--   0        0        0      426 2023-06-05 05:55:19.292698 kui-1.4.0/tests/utils/test_state.py
--rw-r--r--   0        0        0     1290 2023-06-05 05:55:19.292698 kui-1.4.0/tests/wsgi/test_cors.py
--rw-r--r--   0        0        0     6790 2023-06-05 05:55:19.292698 kui-1.4.0/tests/wsgi/test_parameters.py
--rw-r--r--   0        0        0      453 2023-06-05 05:55:19.292698 kui-1.4.0/tests/wsgi/test_views.py
--rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 kui-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-07-04 09:19:13.869283 kui-1.5.0/LICENSE
+-rw-r--r--   0        0        0      440 2023-07-04 09:19:13.869283 kui-1.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-04 09:19:13.869283 kui-1.5.0/kui/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-04 09:19:13.869283 kui-1.5.0/kui/__version__.py
+-rw-r--r--   0        0        0     1718 2023-07-04 09:19:13.869283 kui-1.5.0/kui/asgi/__init__.py
+-rw-r--r--   0        0        0     6977 2023-07-04 09:19:13.869283 kui-1.5.0/kui/asgi/applications.py
+-rw-r--r--   0        0        0     2054 2023-07-04 09:19:13.873283 kui-1.5.0/kui/asgi/cors.py
+-rw-r--r--   0        0        0     2382 2023-07-04 09:19:13.873283 kui-1.5.0/kui/asgi/exceptions.py
+-rw-r--r--   0        0        0     2439 2023-07-04 09:19:13.873283 kui-1.5.0/kui/asgi/lifespan.py
+-rw-r--r--   0        0        0     1470 2023-07-04 09:19:13.873283 kui-1.5.0/kui/asgi/openapi.py
+-rw-r--r--   0        0        0     5261 2023-07-04 09:19:13.873283 kui-1.5.0/kui/asgi/parameters.py
+-rw-r--r--   0        0        0     3756 2023-07-04 09:19:13.873283 kui-1.5.0/kui/asgi/requests.py
+-rw-r--r--   0        0        0     2879 2023-07-04 09:19:13.873283 kui-1.5.0/kui/asgi/responses.py
+-rw-r--r--   0        0        0      972 2023-07-04 09:19:13.873283 kui-1.5.0/kui/asgi/routing.py
+-rw-r--r--   0        0        0     3177 2023-07-04 09:19:13.873283 kui-1.5.0/kui/asgi/templates.py
+-rw-r--r--   0        0        0     4532 2023-07-04 09:19:13.873283 kui-1.5.0/kui/asgi/views.py
+-rw-r--r--   0        0        0      304 2023-07-04 09:19:13.873283 kui-1.5.0/kui/cors.py
+-rw-r--r--   0        0        0     3794 2023-07-04 09:19:13.873283 kui-1.5.0/kui/exceptions.py
+-rw-r--r--   0        0        0      123 2023-07-04 09:19:13.873283 kui-1.5.0/kui/openapi/__init__.py
+-rw-r--r--   0        0        0     9388 2023-07-04 09:19:13.873283 kui-1.5.0/kui/openapi/application.py
+-rw-r--r--   0        0        0     1565 2023-07-04 09:19:13.873283 kui-1.5.0/kui/openapi/extra_docs.py
+-rw-r--r--   0        0        0     1644 2023-07-04 09:19:13.873283 kui-1.5.0/kui/openapi/schema.py
+-rw-r--r--   0        0        0     7726 2023-07-04 09:19:13.873283 kui-1.5.0/kui/openapi/specification.py
+-rw-r--r--   0        0        0      224 2023-07-04 09:19:13.873283 kui-1.5.0/kui/openapi/templates/rapidoc.html
+-rw-r--r--   0        0        0      743 2023-07-04 09:19:13.873283 kui-1.5.0/kui/openapi/templates/redoc.html
+-rw-r--r--   0        0        0     1522 2023-07-04 09:19:13.873283 kui-1.5.0/kui/openapi/templates/swagger.html
+-rw-r--r--   0        0        0     1284 2023-07-04 09:19:13.873283 kui-1.5.0/kui/openapi/types.py
+-rw-r--r--   0        0        0    14614 2023-07-04 09:19:13.873283 kui-1.5.0/kui/parameters/__init__.py
+-rw-r--r--   0        0        0     6803 2023-07-04 09:19:13.873283 kui-1.5.0/kui/parameters/field_functions.py
+-rw-r--r--   0        0        0      960 2023-07-04 09:19:13.873283 kui-1.5.0/kui/parameters/fields.py
+-rw-r--r--   0        0        0        0 2023-07-04 09:19:13.873283 kui-1.5.0/kui/py.typed
+-rw-r--r--   0        0        0     7408 2023-07-04 09:19:13.873283 kui-1.5.0/kui/responses.py
+-rw-r--r--   0        0        0      429 2023-07-04 09:19:13.873283 kui-1.5.0/kui/routing/__init__.py
+-rw-r--r--   0        0        0       82 2023-07-04 09:19:13.873283 kui-1.5.0/kui/routing/__main__.py
+-rw-r--r--   0        0        0     1402 2023-07-04 09:19:13.873283 kui-1.5.0/kui/routing/commands.py
+-rw-r--r--   0        0        0      130 2023-07-04 09:19:13.873283 kui-1.5.0/kui/routing/extensions/__init__.py
+-rw-r--r--   0        0        0     2551 2023-07-04 09:19:13.873283 kui-1.5.0/kui/routing/extensions/file.py
+-rw-r--r--   0        0        0     3008 2023-07-04 09:19:13.873283 kui-1.5.0/kui/routing/extensions/multimethod.py
+-rw-r--r--   0        0        0    17890 2023-07-04 09:19:13.873283 kui-1.5.0/kui/routing/routers.py
+-rw-r--r--   0        0        0     3368 2023-07-04 09:19:13.873283 kui-1.5.0/kui/routing/routes.py
+-rw-r--r--   0        0        0     6234 2023-07-04 09:19:13.873283 kui-1.5.0/kui/routing/tree.py
+-rw-r--r--   0        0        0      385 2023-07-04 09:19:13.873283 kui-1.5.0/kui/routing/typing.py
+-rw-r--r--   0        0        0     4073 2023-07-04 09:19:13.873283 kui-1.5.0/kui/security.py
+-rw-r--r--   0        0        0     2783 2023-07-04 09:19:13.873283 kui-1.5.0/kui/status.py
+-rw-r--r--   0        0        0     1250 2023-07-04 09:19:13.873283 kui-1.5.0/kui/templates.py
+-rw-r--r--   0        0        0      757 2023-07-04 09:19:13.873283 kui-1.5.0/kui/utils/__init__.py
+-rw-r--r--   0        0        0      856 2023-07-04 09:19:13.873283 kui-1.5.0/kui/utils/contextvars.py
+-rw-r--r--   0        0        0     1576 2023-07-04 09:19:13.873283 kui-1.5.0/kui/utils/importer.py
+-rw-r--r--   0        0        0     1907 2023-07-04 09:19:13.873283 kui-1.5.0/kui/utils/inspect.py
+-rw-r--r--   0        0        0     1647 2023-07-04 09:19:13.873283 kui-1.5.0/kui/utils/objects.py
+-rw-r--r--   0        0        0      530 2023-07-04 09:19:13.873283 kui-1.5.0/kui/utils/pipe.py
+-rw-r--r--   0        0        0     1139 2023-07-04 09:19:13.873283 kui-1.5.0/kui/utils/state.py
+-rw-r--r--   0        0        0     1567 2023-07-04 09:19:13.873283 kui-1.5.0/kui/wsgi/__init__.py
+-rw-r--r--   0        0        0     5515 2023-07-04 09:19:13.873283 kui-1.5.0/kui/wsgi/applications.py
+-rw-r--r--   0        0        0     2031 2023-07-04 09:19:13.873283 kui-1.5.0/kui/wsgi/cors.py
+-rw-r--r--   0        0        0     2325 2023-07-04 09:19:13.873283 kui-1.5.0/kui/wsgi/exceptions.py
+-rw-r--r--   0        0        0     1428 2023-07-04 09:19:13.873283 kui-1.5.0/kui/wsgi/openapi.py
+-rw-r--r--   0        0        0     3963 2023-07-04 09:19:13.873283 kui-1.5.0/kui/wsgi/parameters.py
+-rw-r--r--   0        0        0     1835 2023-07-04 09:19:13.873283 kui-1.5.0/kui/wsgi/requests.py
+-rw-r--r--   0        0        0     2879 2023-07-04 09:19:13.873283 kui-1.5.0/kui/wsgi/responses.py
+-rw-r--r--   0        0        0      966 2023-07-04 09:19:13.873283 kui-1.5.0/kui/wsgi/routing.py
+-rw-r--r--   0        0        0     2884 2023-07-04 09:19:13.873283 kui-1.5.0/kui/wsgi/templates.py
+-rw-r--r--   0        0        0     2229 2023-07-04 09:19:13.873283 kui-1.5.0/kui/wsgi/views.py
+-rw-r--r--   0        0        0     1959 2023-07-04 09:19:13.877283 kui-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-04 09:19:13.877283 kui-1.5.0/tests/asgi/__init__.py
+-rw-r--r--   0        0        0     2416 2023-07-04 09:19:13.877283 kui-1.5.0/tests/asgi/test_application.py
+-rw-r--r--   0        0        0     1338 2023-07-04 09:19:13.877283 kui-1.5.0/tests/asgi/test_cors.py
+-rw-r--r--   0        0        0      506 2023-07-04 09:19:13.877283 kui-1.5.0/tests/asgi/test_lifespan.py
+-rw-r--r--   0        0        0     5841 2023-07-04 09:19:13.877283 kui-1.5.0/tests/asgi/test_parameters.py
+-rw-r--r--   0        0        0      535 2023-07-04 09:19:13.877283 kui-1.5.0/tests/asgi/test_views.py
+-rw-r--r--   0        0        0    32395 2023-07-04 09:19:13.877283 kui-1.5.0/tests/openapi/test_application.py
+-rw-r--r--   0        0        0      429 2023-07-04 09:19:13.877283 kui-1.5.0/tests/openapi/test_extra_docs.py
+-rw-r--r--   0        0        0      247 2023-07-04 09:19:13.877283 kui-1.5.0/tests/routing/extensions/test_fileroutes.py
+-rw-r--r--   0        0        0     3363 2023-07-04 09:19:13.877283 kui-1.5.0/tests/routing/extensions/test_multimethod.py
+-rw-r--r--   0        0        0       88 2023-07-04 09:19:13.877283 kui-1.5.0/tests/routing/test_commands.py
+-rw-r--r--   0        0        0     4558 2023-07-04 09:19:13.877283 kui-1.5.0/tests/routing/test_routes.py
+-rw-r--r--   0        0        0     2444 2023-07-04 09:19:13.877283 kui-1.5.0/tests/routing/test_tree.py
+-rw-r--r--   0        0        0      242 2023-07-04 09:19:13.877283 kui-1.5.0/tests/test_export_all.py
+-rw-r--r--   0        0        0     4505 2023-07-04 09:19:13.877283 kui-1.5.0/tests/test_responses.py
+-rw-r--r--   0        0        0     3032 2023-07-04 09:19:13.877283 kui-1.5.0/tests/test_security.py
+-rw-r--r--   0        0        0        0 2023-07-04 09:19:13.877283 kui-1.5.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0      722 2023-07-04 09:19:13.877283 kui-1.5.0/tests/utils/test_importer.py
+-rw-r--r--   0        0        0      170 2023-07-04 09:19:13.877283 kui-1.5.0/tests/utils/test_objects.py
+-rw-r--r--   0        0        0      426 2023-07-04 09:19:13.877283 kui-1.5.0/tests/utils/test_state.py
+-rw-r--r--   0        0        0     1290 2023-07-04 09:19:13.877283 kui-1.5.0/tests/wsgi/test_cors.py
+-rw-r--r--   0        0        0     5610 2023-07-04 09:19:13.877283 kui-1.5.0/tests/wsgi/test_parameters.py
+-rw-r--r--   0        0        0      453 2023-07-04 09:19:13.877283 kui-1.5.0/tests/wsgi/test_views.py
+-rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 kui-1.5.0/PKG-INFO
```

### Comparing `kui-1.4.0/LICENSE` & `kui-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/asgi/__init__.py` & `kui-1.5.0/kui/asgi/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from ..parameters.field_functions import (
     Body,
     Cookie,
     Depends,
     Header,
     Path,
     Query,
-    RequestAttr,
 )
 from ..security import api_key_auth_dependency, basic_auth, bearer_auth
 from .applications import FactoryClass, Kui
 from .cors import allow_cors
 from .openapi import OpenAPI
 from .requests import (
     HttpRequest,
@@ -52,15 +51,14 @@
     "websocket_var",
     "HTTPException",
     "Body",
     "Cookie",
     "Header",
     "Path",
     "Query",
-    "RequestAttr",
     "Depends",
     "api_key_auth_dependency",
     "basic_auth",
     "bearer_auth",
     "UploadFile",
     "HttpResponse",
     "FileResponse",
```

### Comparing `kui-1.4.0/kui/asgi/applications.py` & `kui-1.5.0/kui/asgi/applications.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 
 import copy
 import dataclasses
 import functools
-import inspect
-import traceback
 from pathlib import PurePath
 from types import AsyncGeneratorType
 from typing import (
     Any,
     Callable,
     Iterable,
     List,
@@ -36,55 +34,18 @@
     PlainTextResponse,
     RedirectResponse,
     SendEventResponse,
 )
 from .routing import Router
 from .templates import BaseTemplates
 
-LifespanCallback = Callable[["Kui"], Any]
-T_LifespanCallback = TypeVar("T_LifespanCallback", bound=LifespanCallback)
+from .lifespan import Lifespan, LifespanCallback
 
 
-@dataclasses.dataclass
-class Lifespan:
-    on_startup: List[LifespanCallback] = dataclasses.field(default_factory=list)
-    on_shutdown: List[LifespanCallback] = dataclasses.field(default_factory=list)
-
-    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
-        """
-        Handle ASGI lifespan messages, which allows us to manage application
-        startup and shutdown events.
-        """
-        app: Kui = scope["app"]
-
-        message = await receive()
-        assert message["type"] == "lifespan.startup"
-        try:
-            for handler in self.on_startup:
-                result = handler(app)
-                if inspect.isawaitable(result):
-                    await result
-        except BaseException:
-            msg = traceback.format_exc()
-            await send({"type": "lifespan.startup.failed", "message": msg})
-            raise
-        await send({"type": "lifespan.startup.complete"})
-
-        message = await receive()
-        assert message["type"] == "lifespan.shutdown"
-        try:
-            for handler in self.on_shutdown:
-                result = handler(app)
-                if inspect.isawaitable(result):
-                    await result
-        except BaseException:
-            msg = traceback.format_exc()
-            await send({"type": "lifespan.shutdown.failed", "message": msg})
-            raise
-        await send({"type": "lifespan.shutdown.complete"})
+LifespanCallbackTypeVar = TypeVar("LifespanCallbackTypeVar", bound=LifespanCallback)
 
 
 @dataclasses.dataclass
 class FactoryClass:
     http: Type[HttpRequest] = HttpRequest
     websocket: Type[WebSocket] = WebSocket
 
@@ -136,19 +97,19 @@
     ) -> Callable[[ErrorHandlerType], ErrorHandlerType]:
         def decorator(func: ErrorHandlerType) -> ErrorHandlerType:
             self.add_exception_handler(exc_class_or_status_code, func)
             return func
 
         return decorator
 
-    def on_startup(self, func: T_LifespanCallback) -> T_LifespanCallback:
+    def on_startup(self, func: LifespanCallbackTypeVar) -> LifespanCallbackTypeVar:
         self.lifespan.on_startup.append(func)
         return func
 
-    def on_shutdown(self, func: T_LifespanCallback) -> T_LifespanCallback:
+    def on_shutdown(self, func: LifespanCallbackTypeVar) -> LifespanCallbackTypeVar:
         self.lifespan.on_shutdown.append(func)
         return func
 
     async def app(self, scope: Scope, receive: Receive, send: Send) -> None:
         scope_type: Literal["lifespan", "http", "websocket"] = scope["type"]
         return await getattr(self, scope_type)(scope, receive, send)
```

### Comparing `kui-1.4.0/kui/asgi/cors.py` & `kui-1.5.0/kui/asgi/cors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import functools
 import re
 from typing import Any, Callable, Dict, Iterable, Pattern
 
 from .requests import request
 from .responses import HttpResponse, convert_response
 from .routing import AsyncViewType
 
@@ -39,15 +38,14 @@
         "Access-Control-Expose-Headers": ", ".join(expose_headers),
         "Access-Control-Allow-Credentials": "true" if allow_credentials else "false",
         "Access-Control-Max-Age": str(max_age),
     }
     config_dict = {k: v for k, v in config_dict.items() if v}
 
     def decorator(endpoint: AsyncViewType) -> AsyncViewType:
-        @functools.wraps(endpoint)
         async def cors_wrapper() -> Any:
             origin = request.headers.get("origin", None)
             if origin and any(
                 origin_pattern.fullmatch(origin) for origin_pattern in allow_origins
             ):
                 # Preflight request
                 if request.method == "OPTIONS":
@@ -56,10 +54,10 @@
                     response = convert_response(await endpoint())
                 response.headers.update(config_dict)
                 response.headers["Access-Control-Allow-Origin"] = origin
                 return response
             else:
                 return await endpoint()
 
-        return cors_wrapper
+        return cors_wrapper  # type: ignore
 
     return decorator
```

### Comparing `kui-1.4.0/kui/asgi/exceptions.py` & `kui-1.5.0/kui/asgi/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             except BaseException as exc:
                 handler = self.lookup_handler(exc)
                 if handler is None:
                     raise
                 else:
                     return await handler(exc)
 
-        return wrapper
+        return wrapper  # type: ignore
 
     def _init_internal_handlers(self) -> None:
         self.add_exception_handler(HTTPException, self.http_exception)
         self.add_exception_handler(RequestValidationError, self.validation_error)
 
     @staticmethod
     async def http_exception(exc: HTTPException) -> HttpResponse:
```

### Comparing `kui-1.4.0/kui/asgi/openapi.py` & `kui-1.5.0/kui/asgi/openapi.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/asgi/parameters.py` & `kui-1.5.0/kui/asgi/parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,16 @@
 from ..exceptions import RequestValidationError
 from ..parameters import (
     _convert_model_data_to_keyword_arguments,
     _create_new_signature,
     _merge_multi_value,
     _parse_depends_attrs,
     _parse_parameters_and_request_body_to_model,
-    _parse_request_attrs,
     _update_docs,
     _validate_parameters,
-    _validate_request_attr,
     create_auto_params,
 )
 from ..utils import is_async_gen_callable, is_coroutine_callable, is_gen_callable
 from .requests import request
 
 CallableObject = TypeVar("CallableObject", bound=Callable)
 
@@ -41,24 +39,23 @@
 def _create_new_callback(callback: CallableObject) -> CallableObject:
     sig = inspect.signature(callback)
 
     (
         parameters,
         request_body,
         exclusive_models,
+        security_info,
     ) = _parse_parameters_and_request_body_to_model(sig)
 
-    request_attrs = _parse_request_attrs(sig)
-
     depend_attrs = _parse_depends_attrs(sig)
     depend_functions = {
         name: _create_new_callback(info.call) for name, info in depend_attrs.items()
     }
 
-    if not (parameters or request_body or request_attrs or depend_attrs):
+    if not (parameters or request_body or depend_attrs):
         callback_with_auto_bound_params = callback
     else:
 
         @functools.wraps(callback)
         async def callback_with_auto_bound_params(*args, **kwargs) -> Any:
             data: List[BaseModel] = []
             keyword_params: Dict[str, Any] = {}
@@ -104,24 +101,20 @@
                 # try to get body model and parse
                 if request_body:
                     _body_data = await request.data()
                     if isinstance(_body_data, FormData):
                         _body_data = _merge_multi_value(_body_data.multi_items())
 
                     try:
-                        data.append(request_body.parse_obj(_body_data))
+                        data.append(
+                            request_body.model_validate(_body_data)
+                        )
                     except ValidationError as e:
                         raise RequestValidationError(e, "body")
 
-                # try to get request instance attributes
-                if request_attrs:
-                    keyword_params.update(
-                        _validate_request_attr(request_attrs, request)
-                    )
-
                 keyword_params.update(
                     _convert_model_data_to_keyword_arguments(data, exclusive_models)
                 )
 
                 result = callback(*args, **{**keyword_params, **kwargs})
                 if inspect.isawaitable(result):
                     result = await result
@@ -141,13 +134,14 @@
 
     _update_docs(
         callback,
         callback_with_auto_bound_params,
         parameters,
         request_body,
         depend_functions,
+        security_info,
     )
 
     return typing_cast(CallableObject, callback_with_auto_bound_params)
 
 
 auto_params = create_auto_params(_create_new_callback)
```

### Comparing `kui-1.4.0/kui/asgi/requests.py` & `kui-1.5.0/kui/asgi/requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self._scope[name] = value
 
     def __delitem__(self, name: str) -> None:
         del self._scope[name]
 
     @cached_property
     def state(self) -> State:
-        return self.setdefault("state", State())
+        return State(self.setdefault("state", {}))
 
     @cached_property
     def app(self) -> Kui:
         return self["app"]  # type: ignore
 
     def url_for(self, name: str, path_params: typing.Mapping[str, typing.Any]) -> URL:
         return self.url.replace(path=self.app.router.url_for(name, path_params))
```

### Comparing `kui-1.4.0/kui/asgi/responses.py` & `kui-1.5.0/kui/asgi/responses.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/asgi/routing.py` & `kui-1.5.0/kui/asgi/routing.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/asgi/templates.py` & `kui-1.5.0/kui/asgi/templates.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/asgi/views.py` & `kui-1.5.0/kui/asgi/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import functools
 import json
 from inspect import isfunction
 from typing import TYPE_CHECKING, Any, Callable, Generator, List
 from typing import cast as typing_cast
 
 from baize.typing import Message
 from typing_extensions import Literal
@@ -21,18 +20,17 @@
     allow_methods = {"HEAD", "GET"} if method == "GET" else {method}
     headers = {"Allow": ", ".join(allow_methods)}
 
     def decorator(function: AsyncViewType) -> AsyncViewType:
         if not isfunction(function):
             raise TypeError("`required_method` can only decorate function")
 
-        @functools.wraps(function)
-        async def wrapper(*args, **kwargs):
+        async def wrapper():
             if request.method in allow_methods:
-                return await function(*args, **kwargs)
+                return await function()
             elif request.method == "OPTIONS":
                 return HttpResponse(headers=headers)
             else:
                 return HttpResponse(status_code=405, headers=headers)
 
         setattr(wrapper, "__method__", method.upper())
         return typing_cast(AsyncViewType, wrapper)
```

### Comparing `kui-1.4.0/kui/exceptions.py` & `kui-1.5.0/kui/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from __future__ import annotations
 
 import abc
-import json
 from typing import Any, Callable, Dict, Generic, List, Mapping, Type, TypeVar, Union
 
 from baize.exceptions import HTTPException
 from pydantic import ValidationError
-from pydantic.json import pydantic_encoder
 from typing_extensions import Literal
 
 
 class RequestValidationError(Exception):
     def __init__(
         self,
         validation_error: ValidationError,
@@ -21,16 +19,16 @@
 
     def errors(self) -> List[Dict[str, Any]]:
         errors = self.validation_error.errors()
         for error in errors:
             error["in"] = self.in_  # type: ignore
         return errors  # type: ignore
 
-    def json(self, *, indent: Union[None, int, str] = 2) -> str:
-        return json.dumps(self.errors(), indent=indent, default=pydantic_encoder)
+    def json(self, *, indent: Union[None, int] = 2) -> str:
+        return self.validation_error.json(indent=indent)
 
     @staticmethod
     def schema() -> Dict[str, Any]:
         return {
             "type": "array",
             "items": {
                 "type": "object",
@@ -96,15 +94,17 @@
             self._exception_handlers[exc_class_or_status_code] = handler
 
     def lookup_handler(self, exc: BaseException) -> ErrorHandlerType | None:
         handler = None
         if isinstance(exc, HTTPException):
             handler = self._status_handlers.get(exc.status_code)
         if handler is None:
-            handler = self._lookup_exception_handler(exc)
+            handler = self._lookup_exception_handler(type(exc))
         return handler
 
-    def _lookup_exception_handler(self, exc: BaseException) -> ErrorHandlerType | None:
-        for cls in type(exc).__mro__:
+    def _lookup_exception_handler(
+        self, exc_type: Type[BaseException]
+    ) -> ErrorHandlerType | None:
+        for cls in exc_type.__mro__:
             if cls in self._exception_handlers:
                 return self._exception_handlers[cls]
         return None
```

### Comparing `kui-1.4.0/kui/openapi/application.py` & `kui-1.5.0/kui/openapi/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import copy
 import typing
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Sequence, TypeVar
 
-from pydantic import BaseModel, ValidationError
 from typing_extensions import Literal, TypedDict
 
 if TYPE_CHECKING:
     from ..asgi import Kui as ASGIKui, HttpRequest as ASGIHttpRequest
     from ..wsgi import Kui as WSGIKui, HttpRequest as WSGIHttpRequest
 
 from ..exceptions import RequestValidationError
@@ -141,16 +140,16 @@
 
         # generate responses schema
         responses: spec.Responses = {}
         __docs_responses__: List[spec.Responses] = getattr(
             func, "__docs_responses__", []
         )
         if parameters or request_body:
-            handler = application.exception_middleware.lookup_handler(
-                RequestValidationError(ValidationError([], BaseModel), "body")
+            handler = application.exception_middleware._lookup_exception_handler(
+                RequestValidationError
             )
             if handler is None:
                 raise RuntimeError
             __docs_responses__.extend(_get_response_docs(handler))
 
         for response_docs in __docs_responses__:
             for k, v in list(response_docs.items()):
```

### Comparing `kui-1.4.0/kui/openapi/extra_docs.py` & `kui-1.5.0/kui/openapi/extra_docs.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/openapi/schema.py` & `kui-1.5.0/kui/openapi/schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from __future__ import annotations
 
-import inspect
 from copy import deepcopy
 from typing import TYPE_CHECKING, Optional, Type, Union
 from typing import cast as typing_cast
 
 from baize.datastructures import ContentType
 from pydantic import BaseModel
 from typing_extensions import get_args, get_type_hints
 
+from ..utils import safe_issubclass
+
 if TYPE_CHECKING:
     from ..asgi import Kui as ASGIKui
     from ..wsgi import Kui as WSGIKui
 
 from . import specification as spec
 from .types import UploadFile
 
 REF_TEMPLATE = "#/components/schemas/{model}"
 
 
 def _schema(model: Type[BaseModel]) -> spec.Schema:
-    schema = deepcopy(model.schema(ref_template=REF_TEMPLATE))
+    schema = deepcopy(model.model_json_schema(ref_template=REF_TEMPLATE))
     schema.pop("title")
     return typing_cast(spec.Schema, schema)
 
 
 def schema_request_body(
     body: Type[BaseModel] | None, application: ASGIKui | WSGIKui
 ) -> Optional[spec.RequestBody]:
@@ -37,16 +38,16 @@
             get_type_hints(application.factory_class.http.data, include_extras=True)[
                 "return"
             ]
         )
         if isinstance(v, ContentType)
     ]
 
-    for field in body.__fields__.values():
-        if inspect.isclass(field.type_) and issubclass(field.type_, UploadFile):
+    for field in body.model_fields.values():
+        if safe_issubclass(field.annotation, UploadFile):
             content_types = ["multipart/form-data"]
 
     return {
         "required": True,
         "content": {
             content_type: {"schema": _schema(body)} for content_type in content_types
         },
```

### Comparing `kui-1.4.0/kui/openapi/specification.py` & `kui-1.5.0/kui/openapi/specification.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/openapi/templates/redoc.html` & `kui-1.5.0/kui/openapi/templates/redoc.html`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/openapi/templates/swagger.html` & `kui-1.5.0/kui/openapi/templates/swagger.html`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/parameters/__init__.py` & `kui-1.5.0/kui/parameters/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,48 +8,54 @@
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     List,
     Optional,
     Sequence,
+    Set,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 from typing import cast as typing_cast
 
-from pydantic import BaseConfig, BaseModel, ValidationError, create_model
+from pydantic import BaseModel, RootModel, ValidationError, create_model
+from pydantic.fields import FieldInfo
 from typing_extensions import Annotated, Literal, get_args, get_origin, get_type_hints
 
 if TYPE_CHECKING:
     from ..asgi import HttpRequest as ASGIHttpRequest
     from ..wsgi import HttpRequest as WSGIHttpRequest
     from ..openapi import specification as spec
 
 from ..exceptions import RequestValidationError
 from ..utils import safe_issubclass
-from .fields import DependInfo, FieldInfo, RequestAttrInfo, Undefined
+from .fields import (
+    BaseHTTPFieldInfo,
+    InPath,
+    InQuery,
+    InHeader,
+    InCookie,
+    InBody,
+    Depends,
+)
 
 CallableObject = TypeVar("CallableObject", bound=Callable)
 
 
-def create_model_config(
-    title: str | None = None, description: str | None = None
-) -> Type[BaseConfig]:
-    class ExclusiveModelConfig(BaseConfig):
-        schema_extra = {
-            k: v
-            for k, v in {"title": title, "description": description}.items()
-            if v is not None
-        }
-
-    return ExclusiveModelConfig
-
+get_annotated_args = lambda tp: [
+    j
+    for i in (
+        (get_annotated_args(t) if get_origin(t) is Annotated else [t])  # type: ignore
+        for t in get_args(tp)
+    )
+    for j in i
+]
 
 sorted_groupby = lambda iterable, key: groupby(sorted(iterable, key=key), key=key)
 
 
 def _merge_multi_value(
     items: Sequence[Tuple[str, Any]]
 ) -> Dict[str, Union[Any, List[Any]]]:
@@ -67,61 +73,76 @@
 
 def _parse_parameters_and_request_body_to_model(
     sig: inspect.Signature,
 ) -> Tuple[
     Dict[Literal["path", "query", "header", "cookie"], Type[BaseModel]] | None,
     Type[BaseModel] | None,
     Dict[Type[BaseModel], str],
+    Dict[Literal["path", "query", "header", "cookie"], Dict[str, Any]],
 ]:
     raw_parameters: Dict[str, Any] = {
         key: {} for key in ["path", "query", "header", "cookie", "body"]
     }
     exclusive_models: Dict[Type[BaseModel], str] = {}
+    security_info: Dict[
+        Literal["path", "query", "header", "cookie"], Dict[str, Any]
+    ] = {"path": {}, "query": {}, "header": {}, "cookie": {}}
 
     for name, param in sig.parameters.items():
         if not (
-            isinstance(param.default, FieldInfo)
-            or (
-                get_origin(param.annotation) is Annotated
-                and isinstance(get_args(param.annotation)[1], FieldInfo)
-            )
+            get_origin(param.default) is Annotated
+            or get_origin(param.annotation) is Annotated
         ):
             continue
 
         if param.POSITIONAL_ONLY:
             raise TypeError(
                 f"Parameter {name} cannot be defined as positional only parameters."
             )
 
-        if isinstance(param.default, FieldInfo):
-            type_ = param.annotation
-            info = param.default
+        if get_origin(param.default) is Annotated:
+            raise RuntimeError(
+                f"Parameter {name} default value cannot be defined as {param.default}."
+            )
+
+        type_, *annontated_list = get_annotated_args(param.annotation)
+        kui_field: Union[InPath, InQuery, InHeader, InCookie, InBody]
+        for kui_field in filter(
+            lambda x: isinstance(x, (InPath, InQuery, InHeader, InCookie, InBody)),
+            annontated_list,
+        ):
+            break
         else:
-            type_, info = get_args(param.annotation)
+            # If there is no kui field, skip it.
+            continue
 
-        if getattr(info, "exclusive", False):
+        if kui_field.exclusive:
             if safe_issubclass(type_, BaseModel):
                 model = type_
             else:
-                model = create_model(
-                    "temporary_exclusive_model",
-                    __config__=create_model_config(info.title, info.description),
-                    __root__=(type_, ...),
-                )
-            raw_parameters[info._in] = model
+                model = RootModel[type_]  # type: ignore
+            raw_parameters[kui_field._in] = model
             exclusive_models[model] = name
         else:
-            if safe_issubclass(raw_parameters[info._in], BaseModel):
+            if safe_issubclass(raw_parameters[kui_field._in], BaseModel):
                 raise RuntimeError(
-                    f"{info._in.capitalize()}(exclusive=True) "
-                    f"and {info._in.capitalize()} cannot be used at the same time"
+                    f"{kui_field._in.capitalize()}(exclusive=True) "
+                    f"and {kui_field._in.capitalize()} cannot be used at the same time"
                 )
-            if type_ == param.empty:
-                type_ = Any
-            raw_parameters[info._in][name] = (type_, info)
+            field_info = next(
+                filter(lambda x: isinstance(x, FieldInfo), annontated_list)
+            )
+            raw_parameters[kui_field._in][name] = (type_, field_info)
+            if (
+                isinstance(kui_field, (InQuery, InHeader, InCookie))
+                and kui_field.security
+            ):
+                security_info[kui_field._in][
+                    field_info.alias or name
+                ] = kui_field.security
 
     for key, params in filter(
         lambda kv: kv[1],
         ((key, raw_parameters.pop(key)) for key in tuple(raw_parameters.keys())),
     ):
         if safe_issubclass(params, BaseModel):
             model = params
@@ -144,87 +165,62 @@
     return (
         typing_cast(
             Dict[Literal["path", "query", "header", "cookie"], Type[BaseModel]],
             parameters,
         ),
         request_body,
         exclusive_models,
+        security_info,
     )
 
 
-def _parse_depends_attrs(sig: inspect.Signature) -> Dict[str, DependInfo]:
-    return {
-        **{
-            name: param.default
-            for name, param in sig.parameters.items()
-            if isinstance(param.default, DependInfo)
-        },
-        **{
-            name: get_args(param.annotation)[1]
-            for name, param in sig.parameters.items()
-            if get_origin(param.annotation) is Annotated
-            and isinstance(get_args(param.annotation)[1], DependInfo)
-        },
-    }
-
+def _parse_depends_attrs(sig: inspect.Signature) -> Dict[str, Depends]:
+    if {
+        name: param.default
+        for name, param in sig.parameters.items()
+        if isinstance(param.default, Depends)
+    }:
+        raise RuntimeError("Depends cannot be used as default value of parameters.")
 
-def _parse_request_attrs(sig: inspect.Signature) -> Dict[str, RequestAttrInfo]:
     return {
-        **{
-            name: param.default
-            for name, param in sig.parameters.items()
-            if isinstance(param.default, RequestAttrInfo)
-        },
-        **{
-            name: get_args(param.annotation)[1]
-            for name, param in sig.parameters.items()
-            if get_origin(param.annotation) is Annotated
-            and isinstance(get_args(param.annotation)[1], RequestAttrInfo)
-        },
+        name: get_args(param.annotation)[1]
+        for name, param in sig.parameters.items()
+        if get_origin(param.annotation) is Annotated
+        and isinstance(get_args(param.annotation)[1], Depends)
     }
 
 
 def _create_new_signature(sig: inspect.Signature) -> inspect.Signature:
     return inspect.Signature(
         parameters=[
             param
             for param in sig.parameters.values()
             if not (
-                isinstance(param.default, (FieldInfo, RequestAttrInfo, DependInfo))
+                isinstance(param.default, (BaseHTTPFieldInfo, Depends))
                 or (
                     get_origin(param.annotation) is Annotated
-                    and isinstance(
-                        get_args(param.annotation)[1], (FieldInfo, RequestAttrInfo)
-                    )
+                    and isinstance(get_args(param.annotation)[1], FieldInfo)
                 )
             )
         ],
         return_annotation=sig.return_annotation,
     )
 
 
-def _get_security(m: Type[BaseModel]) -> Dict[str, Dict[Any, Any]]:
-    return {
-        field.alias: field.field_info.extra["security"]
-        for field in m.__fields__.values()
-        if field.field_info.extra.get("security", None)
-    }
-
-
 def _get_parameters_docs(
     m: Optional[Type[BaseModel]],
     position: Literal["path", "query", "header", "cookie"],
+    security_fields: Set[str],
 ) -> List[spec.Parameter]:
     if m is None:
         return []
 
-    _schemas: Dict[str, Any] = copy.deepcopy(m.schema())
+    _schemas: Dict[str, Any] = copy.deepcopy(m.model_json_schema())
     properties: Dict[str, Any] = _schemas["properties"]
     required: Sequence[str] = _schemas.get("required", ())
-    security_fields = set(_get_security(m).keys())
 
     return [
         {
             "in": position,
             "name": name,
             "description": schema.pop("description", ""),
             "required": name in required,
@@ -274,14 +270,15 @@
 def _update_docs(
     old_handler: Callable[..., Any],
     handler: Callable[..., Any],
     parameters: Dict[Literal["path", "query", "header", "cookie"], Type[BaseModel]]
     | None,
     request_body: Type[BaseModel] | None,
     depend_functions: Dict[str, Callable[..., Any]],
+    security_info: Dict[Literal["path", "query", "header", "cookie"], Dict[str, Any]],
 ) -> None:
     if inspect.ismethod(handler):
         handler = handler.__func__  # type: ignore
 
     if isinstance(handler.__doc__, str):
         clean_doc = inspect.cleandoc(handler.__doc__)
         if not hasattr(handler, "__docs_summary__") and not hasattr(
@@ -300,18 +297,20 @@
         setattr(handler, "__docs_request_body__", __request_body__)
 
     if parameters is not None:
         __parameters__: List[Any] = getattr(handler, "__docs_parameters__", [])
         __security__: List[Any] = getattr(handler, "__docs_security__", [])
         for position, model in parameters.items():
             __parameters__ = _merge_parameters_docs(
-                __parameters__, _get_parameters_docs(model, position)
+                __parameters__,
+                _get_parameters_docs(
+                    model, position, set(security_info[position].keys())
+                ),
             )
-            for security in _get_security(model).values():
-                __security__.append(security)
+        __security__.extend(info for p in security_info.values() for info in p.values())
         setattr(handler, "__docs_security__", __security__)
         setattr(handler, "__docs_parameters__", __parameters__)
 
     setattr(handler, "__docs_responses__", parse_docs_responses(old_handler))
 
     for func in depend_functions.values():
         __request_body__ = getattr(handler, "__docs_request_body__", [])
@@ -340,77 +339,54 @@
     parameters: Dict[Literal["path", "query", "header", "cookie"], Type[BaseModel]],
     request: ASGIHttpRequest | WSGIHttpRequest,
 ) -> List[BaseModel]:
     data = []
 
     if "path" in parameters:
         try:
-            data.append(parameters["path"].parse_obj(request.path_params))
+            data.append(parameters["path"].model_validate(request.path_params))
         except ValidationError as e:
             raise RequestValidationError(e, "path")
 
     if "query" in parameters:
         try:
             data.append(
-                parameters["query"].parse_obj(
+                parameters["query"].model_validate(
                     _merge_multi_value(request.query_params.multi_items())
                 )
             )
         except ValidationError as e:
             raise RequestValidationError(e, "query")
 
     if "header" in parameters:
         try:
-            data.append(parameters["header"].parse_obj(request.headers))
+            data.append(parameters["header"].model_validate(request.headers._dict))
         except ValidationError as e:
             raise RequestValidationError(e, "header")
 
     if "cookie" in parameters:
         try:
-            data.append(parameters["cookie"].parse_obj(request.cookies))
+            data.append(parameters["cookie"].model_validate(request.cookies))
         except ValidationError as e:
             raise RequestValidationError(e, "cookie")
 
     return data
 
 
-def _validate_request_attr(
-    request_attrs: Dict[str, RequestAttrInfo],
-    request: ASGIHttpRequest | WSGIHttpRequest,
-) -> Dict[str, Any]:
-    result = {}
-    for name, info in request_attrs.items():
-        try:
-            value: Any = functools.reduce(
-                lambda attr, name: getattr(attr, name),
-                (info.alias or name).split("."),
-                request,
-            )
-        except AttributeError:
-            if info.default is not Undefined:
-                value = info.default
-            elif info.default_factory is not None:
-                value = info.default_factory()
-            else:
-                raise
-        result[name] = value
-    return result
-
-
 def _convert_model_data_to_keyword_arguments(
     data: List[BaseModel], exclusive_models: Dict[Type[BaseModel], str]
 ) -> Dict[str, Any]:
     result = {}
     for _data in data:
         if _data.__class__.__name__ == "temporary_model":
             result.update(
-                {name: getattr(_data, name) for name in _data.__fields__.keys()}
+                {name: getattr(_data, name) for name in _data.model_fields.keys()}
             )
-        elif _data.__class__.__name__ == "temporary_exclusive_model":
-            result[exclusive_models[_data.__class__]] = _data.__root__  # type: ignore
+        elif isinstance(_data, RootModel):
+            result[exclusive_models[_data.__class__]] = _data.root  # type: ignore
         else:
             result[exclusive_models[_data.__class__]] = _data
     return result
 
 
 def _create_new_class(cls):
     """
```

### Comparing `kui-1.4.0/kui/responses.py` & `kui-1.5.0/kui/responses.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from __future__ import annotations
 
 import typing
 from http import HTTPStatus
 
-from pydantic import BaseModel, create_model
-from pydantic.json import pydantic_encoder
-from pydantic.typing import display_as_type
+from pydantic import BaseModel, RootModel
+from pydantic_core import to_jsonable_python
 
 from .openapi import specification as spec
 from .utils import safe_issubclass
 
 
 def _json_encoder(obj: typing.Any) -> typing.Any:
-    if isinstance(obj, BaseModel):
-        return obj.dict(by_alias=True)
-    return pydantic_encoder(obj)
+    return to_jsonable_python(obj)
 
 
 class JSONResponseMixin:
     def __class_getitem__(
         cls,
         parameters: typing.Tuple[
             int,
@@ -50,27 +47,27 @@
             str(status_code): {
                 "description": HTTPStatus(status_code).description,
                 "headers": headers,
             }
         }
 
         if content:
-            real_content: spec.Schema | typing.Type[BaseModel] | typing.Dict[
-                typing.Any, typing.Any
-            ]
+            real_content: (
+                spec.Schema
+                | typing.Type[BaseModel]
+                | typing.Dict[typing.Any, typing.Any]
+            )
             if isinstance(content, dict):
                 real_content = content
             elif getattr(content, "__origin__", None) is None and safe_issubclass(
                 content, BaseModel
             ):
                 real_content = content
             else:
-                real_content = create_model(
-                    f"ParsingModel[{display_as_type(content)}]", __root__=(content, ...)
-                )
+                real_content = RootModel[content]  # type: ignore
             docs[str(status_code)]["content"] = {
                 "application/json": {"schema": real_content}
             }
 
         return docs
```

### Comparing `kui-1.4.0/kui/routing/commands.py` & `kui-1.5.0/kui/routing/commands.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/routing/extensions/file.py` & `kui-1.5.0/kui/routing/extensions/file.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/routing/extensions/multimethod.py` & `kui-1.5.0/kui/routing/extensions/multimethod.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from typing_extensions import Self
 
 from ...routing import BaseRoute, HttpRoute, Routes
 from ..typing import ViewType
 
 
-class MultimethodRoutes(Routes[ViewType]):
+class MultimethodRoutes(Routes[ViewType], typing.Generic[ViewType]):
     def __init__(
         self,
         *iterable: typing.Union[
             BaseRoute[ViewType], typing.Iterable[BaseRoute[ViewType]]
         ],
         base_class: type,
         namespace: str = "",
```

### Comparing `kui-1.4.0/kui/routing/routers.py` & `kui-1.5.0/kui/routing/routers.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/routing/routes.py` & `kui-1.5.0/kui/routing/routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,21 +31,25 @@
 
     def __matmul__(self: Self, middleware: MiddlewareType[ViewType]) -> Self:
         endpoint = self.endpoint
         if hasattr(endpoint, "__methods__"):
             for method in map(str.lower, endpoint.__methods__):
                 old_callback = getattr(endpoint, method)
                 new_callback = middleware(old_callback)
+                if getattr(new_callback, "__wrapped__", None) is old_callback:
+                    raise RuntimeError("Cannot use `@functools.wraps` on a middleware.")
                 if new_callback is not old_callback:
                     update_wrapper(new_callback, old_callback)
                     new_callback = self._auto_params(new_callback)
                 setattr(endpoint, method, staticmethod(new_callback))
         else:
             old_callback = endpoint
             new_callback = middleware(old_callback)
+            if getattr(new_callback, "__wrapped__", None) is old_callback:
+                raise RuntimeError("Cannot use `@functools.wraps` on a middleware.")
             if new_callback is not old_callback:
                 update_wrapper(new_callback, old_callback)
                 new_callback = self._auto_params(new_callback)
             self.endpoint = new_callback
         return self
 
     def __post_init__(self) -> None:
```

### Comparing `kui-1.4.0/kui/routing/tree.py` & `kui-1.5.0/kui/routing/tree.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/security.py` & `kui-1.5.0/kui/security.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 import base64
 from http import HTTPStatus
-from typing import Callable, Tuple, Union
+from typing import Callable, Tuple, Type, Union
 
 from typing_extensions import Annotated, Literal
 
+from pydantic import Field
+
 from .exceptions import HTTPException
-from .parameters.field_functions import (
-    RequiredApiKeyAuth,
-    RequiredBasicAuth,
-    RequiredBearerAuth,
-)
+from .parameters.fields import InHeader, InQuery, InCookie
 
 __all__ = [
     "bearer_auth",
 ]
 
 
 def bearer_auth(
-    authorization: Annotated[Union[str, None], RequiredBearerAuth()]
+    authorization: Annotated[
+        Union[str, None],
+        Field(default=None, alias="authorization", title="Bearer Auth"),
+        InHeader(
+            security={
+                "scheme": {"BearerAuth": {"type": "http", "scheme": "bearer"}},
+                "required": {"BearerAuth": []},
+            }
+        ),
+    ]
 ) -> Annotated[
     str,
     {
         401: {
             "description": HTTPStatus(401).description,
             "headers": {
                 "WWW-Authenticate": {
@@ -52,15 +59,24 @@
             401,
             headers={"WWW-Authenticate": "Bearer"},
         )
     return token
 
 
 def basic_auth(
-    authorization: Annotated[Union[str, None], RequiredBasicAuth()]
+    authorization: Annotated[
+        Union[str, None],
+        Field(default=None, alias="authorization", title="Basic Auth"),
+        InHeader(
+            security={
+                "scheme": {"BasicAuth": {"type": "http", "scheme": "basic"}},
+                "required": {"BasicAuth": []},
+            }
+        ),
+    ]
 ) -> Annotated[
     Tuple[str, str],
     {
         401: {
             "description": HTTPStatus(401).description,
             "headers": {
                 "WWW-Authenticate": {
@@ -98,16 +114,42 @@
 def api_key_auth_dependency(
     name: str,
     position: Literal["query", "header", "cookie"] = "header",
 ) -> Callable[[Union[str, None]], str]:
     """
     Create API key authentication dependency.
     """
+    class_: Union[Type[InQuery], Type[InHeader], Type[InCookie]]
+    if position == "query":
+        class_ = InQuery
+    elif position == "header":
+        class_ = InHeader
+    elif position == "cookie":
+        class_ = InCookie
+    else:
+        raise ValueError(
+            f"Invalid position {position}, must be one of ('query', 'header', 'cookie')"
+        )
 
     def api_key_auth(
-        api_key: Annotated[Union[str, None], RequiredApiKeyAuth(name, position)]
+        api_key: Annotated[
+            Union[str, None],
+            Field(
+                default=None,
+                alias=name,
+                title="API Key",
+            ),
+            class_(
+                security={
+                    "scheme": {
+                        "ApiKeyAuth": {"type": "apiKey", "name": name, "in": position}
+                    },
+                    "required": {"ApiKeyAuth": []},
+                }
+            ),
+        ]
     ) -> Annotated[str, {401: {"description": HTTPStatus(401).description}}]:
         if api_key is None:
             raise HTTPException(401)
         return api_key
 
     return api_key_auth
```

### Comparing `kui-1.4.0/kui/status.py` & `kui-1.5.0/kui/status.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/templates.py` & `kui-1.5.0/kui/templates.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/utils/__init__.py` & `kui-1.5.0/kui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/utils/contextvars.py` & `kui-1.5.0/kui/utils/contextvars.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/utils/importer.py` & `kui-1.5.0/kui/utils/importer.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/utils/inspect.py` & `kui-1.5.0/kui/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/utils/objects.py` & `kui-1.5.0/kui/utils/objects.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/utils/pipe.py` & `kui-1.5.0/kui/utils/pipe.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/utils/state.py` & `kui-1.5.0/kui/utils/state.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import threading
-from typing import Any
+from typing import Any, Dict
 
 
-class State(dict):
+class State(Dict[str, Any]):
     """
     An object that can be used to store arbitrary state.
     """
 
     def __enter__(self):
         if not hasattr(self, "sync_lock"):
             self.sync_lock = threading.Lock()
```

### Comparing `kui-1.4.0/kui/wsgi/__init__.py` & `kui-1.5.0/kui/wsgi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from ..parameters.field_functions import (
     Body,
     Cookie,
     Depends,
     Header,
     Path,
     Query,
-    RequestAttr,
 )
 from ..security import api_key_auth_dependency, basic_auth, bearer_auth
 from .applications import FactoryClass, Kui
 from .cors import allow_cors
 from .openapi import OpenAPI
 from .requests import HttpRequest, request, request_var
 from .responses import (
@@ -42,15 +41,14 @@
     "request_var",
     "HTTPException",
     "Body",
     "Cookie",
     "Header",
     "Path",
     "Query",
-    "RequestAttr",
     "Depends",
     "api_key_auth_dependency",
     "basic_auth",
     "bearer_auth",
     "UploadFile",
     "HttpResponse",
     "FileResponse",
```

### Comparing `kui-1.4.0/kui/wsgi/applications.py` & `kui-1.5.0/kui/wsgi/applications.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/wsgi/cors.py` & `kui-1.5.0/kui/wsgi/cors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import functools
 import re
 from typing import Any, Callable, Dict, Iterable, Pattern
 
 from .requests import request
 from .responses import HttpResponse, convert_response
 from .routing import SyncViewType
 
@@ -39,15 +38,14 @@
         "Access-Control-Expose-Headers": ", ".join(expose_headers),
         "Access-Control-Allow-Credentials": "true" if allow_credentials else "false",
         "Access-Control-Max-Age": str(max_age),
     }
     config_dict = {k: v for k, v in config_dict.items() if v}
 
     def decorator(endpoint: SyncViewType) -> SyncViewType:
-        @functools.wraps(endpoint)
         def cors_wrapper() -> Any:
             origin = request.headers.get("origin", None)
             if origin and any(
                 origin_pattern.fullmatch(origin) for origin_pattern in allow_origins
             ):
                 # Preflight request
                 if request.method == "OPTIONS":
@@ -56,10 +54,10 @@
                     response = convert_response(endpoint())
                 response.headers.update(config_dict)
                 response.headers["Access-Control-Allow-Origin"] = origin
                 return response
             else:
                 return endpoint()
 
-        return cors_wrapper
+        return cors_wrapper  # type: ignore
 
     return decorator
```

### Comparing `kui-1.4.0/kui/wsgi/exceptions.py` & `kui-1.5.0/kui/wsgi/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             except BaseException as exc:
                 handler = self.lookup_handler(exc)
                 if handler is None:
                     raise
                 else:
                     return handler(exc)
 
-        return wrapper
+        return wrapper  # type: ignore
 
     def _init_internal_handlers(self) -> None:
         self.add_exception_handler(HTTPException, self.http_exception)
         self.add_exception_handler(RequestValidationError, self.validation_error)
 
     @staticmethod
     def http_exception(exc: HTTPException) -> HttpResponse:
```

### Comparing `kui-1.4.0/kui/wsgi/openapi.py` & `kui-1.5.0/kui/wsgi/openapi.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/wsgi/parameters.py` & `kui-1.5.0/kui/wsgi/parameters.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,18 +12,16 @@
 from ..exceptions import RequestValidationError
 from ..parameters import (
     _convert_model_data_to_keyword_arguments,
     _create_new_signature,
     _merge_multi_value,
     _parse_depends_attrs,
     _parse_parameters_and_request_body_to_model,
-    _parse_request_attrs,
     _update_docs,
     _validate_parameters,
-    _validate_request_attr,
     create_auto_params,
 )
 from ..utils import is_gen_callable
 from .requests import request
 
 CallableObject = TypeVar("CallableObject", bound=Callable)
 
@@ -36,24 +34,23 @@
 def _create_new_callback(callback: CallableObject) -> CallableObject:
     sig = inspect.signature(callback)
 
     (
         parameters,
         request_body,
         exclusive_models,
+        security_info,
     ) = _parse_parameters_and_request_body_to_model(sig)
 
-    request_attrs = _parse_request_attrs(sig)
-
     depend_attrs = _parse_depends_attrs(sig)
     depend_functions = {
         name: _create_new_callback(info.call) for name, info in depend_attrs.items()
     }
 
-    if not (parameters or request_body or request_attrs or depend_attrs):
+    if not (parameters or request_body or depend_attrs):
         callback_with_auto_bound_params = callback
     else:
 
         @functools.wraps(callback)
         def callback_with_auto_bound_params(*args, **kwargs) -> Any:
             data: List[BaseModel] = []
             keyword_params: Dict[str, Any] = {}
@@ -85,24 +82,20 @@
                 # try to get body model and parse
                 if request_body:
                     _body_data = request.data()
                     if isinstance(_body_data, FormData):
                         _body_data = _merge_multi_value(_body_data.multi_items())
 
                     try:
-                        data.append(request_body.parse_obj(_body_data))
+                        data.append(
+                            request_body.model_validate(_body_data)
+                        )
                     except ValidationError as e:
                         raise RequestValidationError(e, "body")
 
-                # try to get request instance attributes
-                if request_attrs:
-                    keyword_params.update(
-                        _validate_request_attr(request_attrs, request)
-                    )
-
                 keyword_params.update(
                     _convert_model_data_to_keyword_arguments(data, exclusive_models)
                 )
 
                 result = callback(*args, **{**keyword_params, **kwargs})
                 return result
             finally:
@@ -117,13 +110,14 @@
 
     _update_docs(
         callback,
         callback_with_auto_bound_params,
         parameters,
         request_body,
         depend_functions,
+        security_info,
     )
 
     return typing_cast(CallableObject, callback_with_auto_bound_params)
 
 
 auto_params = create_auto_params(_create_new_callback)
```

### Comparing `kui-1.4.0/kui/wsgi/requests.py` & `kui-1.5.0/kui/wsgi/requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self._environ[name] = value
 
     def __delitem__(self, name: str) -> None:
         del self._environ[name]
 
     @cached_property
     def state(self) -> State:
-        return self.setdefault("state", State())
+        return State(self.setdefault("state", {}))
 
     @cached_property
     def app(self) -> Kui:
         return self["app"]  # type: ignore
 
     def url_for(self, name: str, path_params: typing.Mapping[str, typing.Any]) -> URL:
         return self.url.replace(path=self.app.router.url_for(name, path_params))
```

### Comparing `kui-1.4.0/kui/wsgi/responses.py` & `kui-1.5.0/kui/wsgi/responses.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/wsgi/routing.py` & `kui-1.5.0/kui/wsgi/routing.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/wsgi/templates.py` & `kui-1.5.0/kui/wsgi/templates.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/kui/wsgi/views.py` & `kui-1.5.0/kui/wsgi/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import functools
 from inspect import isfunction
 from typing import TYPE_CHECKING, Any, Callable, List
 from typing import cast as typing_cast
 
 from ..routing import SyncViewType
 from .requests import request
 from .responses import HttpResponse
@@ -17,15 +16,14 @@
     allow_methods = {"HEAD", "GET"} if method == "GET" else {method}
     headers = {"Allow": ", ".join(allow_methods)}
 
     def decorator(function: SyncViewType) -> SyncViewType:
         if not isfunction(function):
             raise TypeError("`required_method` can only decorate function")
 
-        @functools.wraps(function)
         def wrapper(*args, **kwargs):
             if request.method in allow_methods:
                 return function(*args, **kwargs)
             elif request.method == "OPTIONS":
                 return HttpResponse(headers=headers)
             else:
                 return HttpResponse(status_code=405, headers=headers)
```

### Comparing `kui-1.4.0/pyproject.toml` & `kui-1.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "kui"
-version = "1.4.0"
+version = "1.5.0"
 description = "An easy-to-use web framework."
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "baize<0.21.0,>=0.20.0",
-    "pydantic<2.0,>=1.8",
+    "pydantic>=2.0",
     "typing-extensions>=4.2.0",
 ]
 requires-python = ">=3.7,<4.0"
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
@@ -28,44 +28,35 @@
 
 [project.optional-dependencies]
 cli = [
     "click<9.0,>=8.0",
 ]
 
 [tool.pdm.scripts]
-lint-isort = "isort {args}"
-lint-black = "black {args}"
-check-isort = "isort --check --diff {args}"
-check-black = "black --check --diff {args}"
-check-flake8 = "flake8 --ignore W503,E203,E501,E731 {args}"
+lint-ruff = "ruff --fix {args}"
+check-ruff = "ruff check {args}"
 check-mypy = "mypy {args}"
 test = "pytest {args}"
 
 [tool.pdm.scripts.lint]
 composite = [
-    "lint-isort kui tests",
-    "lint-black kui tests",
-    "check-flake8 kui tests",
-    "check-mypy kui tests",
+    "lint-ruff kui tests",
+    "check",
 ]
 
 [tool.pdm.scripts.check]
 composite = [
-    "check-isort",
-    "check-black",
-    "check-flake8",
-    "check-mypy",
+    "check-ruff kui tests",
+    "check-mypy kui tests",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "flake8>=5.0.4",
-    "black>=23.1.0",
-    "isort>=5.11.5",
     "mypy>=1.0.0",
+    "ruff>=0.0.270",
 ]
 test = [
     "async-asgi-testclient<2.0.0,>=1.4.11",
     "pytest<8.0.0,>=7.2.1",
     "pytest-asyncio<1.0,>=0.20.3",
     "pytest-cov<5.0.0,>=4.0.0",
     "httpx>=0.23.3",
@@ -78,14 +69,20 @@
 
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.isort]
 profile = "black"
 
+[tool.ruff]
+ignore = [
+    "E501",
+    "E731",
+]
+
 [tool.coverage.run]
 omit = [
     "*/.venv/*",
     "*/tests/*",
     "kui/status.py",
 ]
```

### Comparing `kui-1.4.0/tests/asgi/test_application.py` & `kui-1.5.0/tests/asgi/test_application.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/tests/asgi/test_cors.py` & `kui-1.5.0/tests/asgi/test_cors.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/tests/asgi/test_parameters.py` & `kui-1.5.0/tests/asgi/test_parameters.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     Body,
     Cookie,
     Depends,
     Header,
     Kui,
     Path,
     Query,
-    RequestAttr,
     UploadFile,
 )
 
 
 @pytest.mark.asyncio
 async def test_path():
     app = Kui()
@@ -111,52 +110,14 @@
         resp = await client.post("/", form={"name0": "aber"})
         assert resp.status_code == 422
 
     assert not inspect.signature(app.router.search("http", "/")[1]).parameters
 
 
 @pytest.mark.asyncio
-async def test_request():
-    app0 = Kui()
-
-    @app0.router.http.get("/")
-    async def homepage(app: Annotated[Kui, RequestAttr()]):
-        return str(app is app0)
-
-    @app0.router.http.get("/no-attr")
-    async def no_attr(application: Annotated[Kui, RequestAttr()]):
-        return str(application is app0)
-
-    @app0.router.http.get("/no-attr-with-default")
-    async def no_attr_with_default(application: Annotated[Kui, RequestAttr(app0)]):
-        return str(application is app0)
-
-    @app0.router.http.get("/no-attr-with-default-factory")
-    async def no_attr_with_default_factory(
-        application: Annotated[Kui, RequestAttr(default_factory=lambda: app0)],
-    ):
-        return str(application is app0)
-
-    async with TestClient(app0) as client:
-        resp = await client.get("/")
-        assert resp.text == "True"
-
-        with pytest.raises(AttributeError):
-            await client.get("/no-attr")
-
-        resp = await client.get("/no-attr-with-default")
-        assert resp.text == "True"
-
-        resp = await client.get("/no-attr-with-default-factory")
-        assert resp.text == "True"
-
-    assert not inspect.signature(app0.router.search("http", "/")[1]).parameters
-
-
-@pytest.mark.asyncio
 async def test_depend():
     app = Kui()
 
     def get_name(name: Annotated[str, Body(...)]):
         return name
 
     @app.router.http.get("/")
@@ -215,21 +176,21 @@
 
 
 @pytest.mark.asyncio
 async def test_middleware():
     app = Kui()
 
     def middleware(endpoint):
-        async def middleware_wrapper(query: str = Query(...)):
+        async def middleware_wrapper(query: Annotated[str, Query(...)]):
             return await endpoint()
 
         return middleware_wrapper
 
     @app.router.http.get("/", middlewares=[middleware])
-    async def cookie(name: str = Cookie()):
+    async def cookie(name: Annotated[str, Cookie()]):
         return name
 
     async with TestClient(app) as client:
         resp = await client.get("/", cookies={"name": "aber"})
         assert resp.status_code == 422
 
         resp = await client.get("/?query=123", cookies={"name": "aber"})
```

### Comparing `kui-1.4.0/tests/asgi/test_views.py` & `kui-1.5.0/tests/asgi/test_views.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/tests/openapi/test_application.py` & `kui-1.5.0/tests/openapi/test_application.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,47 +39,48 @@
         """
         pass
 
     class Username(BaseModel):
         name: str
 
     @app.router.http.get("/path/{name}")
-    async def path(name: str = Path(...)):
+    async def path(name: Annotated[str, Path(...)]):
         pass
 
     @app.router.http("/http-view")
     class HTTPClass(HttpView):
-        async def get(self) -> Annotated[Any, HTMLResponse[200]]:
+        @classmethod
+        async def get(cls) -> Annotated[Any, HTMLResponse[200]]:
             """
             ...
 
             ......
             """
 
-        async def post(
-            self,
-        ) -> Annotated[Any, JSONResponse[201, {}, Username]]:
+        @classmethod
+        async def post(cls) -> Annotated[Any, JSONResponse[201, {}, Username]]:
             """
             ...
 
             ......
             """
 
+        @classmethod
         async def delete(
-            self,
+            cls,
         ) -> Annotated[Any, {"204": {"description": HTTPStatus(204).description}}]:
             """
             ...
 
             ......
             """
 
     def just_middleware(endpoint):
         async def wrapper(
-            authorization: str = Header(..., description="JWT Token")
+            authorization: Annotated[str, Header(..., description="JWT Token")]
         ) -> Annotated[Any, {"401": {"description": HTTPStatus(401).description}}]:
             return await endpoint()
 
         return wrapper
 
     middleware_routes = "/middleware" // Routes(
         HttpRoute("/path/{name}", path),
@@ -106,15 +107,14 @@
     assert json.loads(openapi_docs_text) == {
         "openapi": "3.0.3",
         "info": {"title": "Kuí API", "version": "1.0.0"},
         "paths": {
             "/hello": {
                 "get": {
                     "summary": "hello",
-                    "description": "hello",
                     "responses": {
                         "200": {
                             "description": "Request fulfilled, document follows",
                             "headers": {},
                             "content": {
                                 "application/json": {
                                     "schema": {
@@ -516,15 +516,15 @@
     assert openapi._generate_path(app, app.router.search("http", "/0")[1], "/") == {
         "get": {"summary": "Summary", "description": "Description"}
     }
     assert openapi._generate_path(app, app.router.search("http", "/1")[1], "/") == {
         "get": {"summary": "Summary"}
     }
     assert openapi._generate_path(app, app.router.search("http", "/2")[1], "/") == {
-        "get": {"summary": "Summary", "description": "Description"}
+        "get": {"summary": "Summary"}
     }
     assert openapi._generate_path(app, app.router.search("http", "/3")[1], "/") == {
         "get": {"summary": "Summary", "description": "Description"}
     }
 
 
 def test_openapi_single_function_tags():
@@ -661,15 +661,15 @@
 
 def test_openapi_depend_response():
     app = Kui()
     openapi = OpenAPI()
     app.router <<= "/docs" // openapi.routes
 
     async def get_current_user(
-        authorization: str = Header(..., description="JWT Token")
+        authorization: Annotated[str, Header(..., description="JWT Token")]
     ) -> Annotated[Any, {"401": {"description": HTTPStatus(401).description}}]:
         pass
 
     @app.router.http.get("/")
     async def homepage(user: Annotated[Any, Depends(get_current_user)]) -> Any:
         pass
```

### Comparing `kui-1.4.0/tests/routing/extensions/test_multimethod.py` & `kui-1.5.0/tests/routing/extensions/test_multimethod.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from __future__ import annotations
+from typing_extensions import Annotated
 
 import pytest
 from async_asgi_testclient import TestClient
 
-from kui.asgi import HttpRoute, HttpView
+from kui.asgi import HttpRoute, HttpView, Path, Kui, Query
 from kui.asgi import MultimethodRoutes as Routes
 from kui.asgi import required_method
 from kui.utils import safe_issubclass
 
 
 def test_routes():
     async def endpoint():
@@ -103,27 +103,32 @@
         and hasattr(endpoint, "post")
         and hasattr(endpoint, "delete")
     )
 
 
 @pytest.mark.asyncio
 async def test_mulitmethodroutes_with_parameters():
-    from kui.asgi import Kui, Path
-
     routes = Routes(base_class=HttpView)
 
     @routes.http.get("/{name}", name=None)
     @routes.http.post("/{name}", name=None)
     @routes.http.put("/{name}", name=None)
     @routes.http.patch("/{name}", name=None)
     @routes.http.delete("/{name}", name=None)
-    async def name(name: str = Path(...)):
-        return name
+    async def name(
+        name: Annotated[str, Path()],
+        status: Annotated[int, Query(200)],
+    ):
+        return name, status
 
     app = Kui(routes=routes)
 
     async with TestClient(app) as client:
         resp = await client.get("/aber")
         assert resp.text == "aber"
 
+        resp = await client.post("/aber", query_string={"status": 201})
+        assert resp.status_code == 201
+        assert resp.text == "aber"
+
         resp = await client.get("/")
         assert resp.status_code == 404
```

### Comparing `kui-1.4.0/tests/routing/test_routes.py` & `kui-1.5.0/tests/routing/test_routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 from __future__ import annotations
+import functools
+
+import pytest
 
 
 def test_decorator():
     from kui.asgi import Kui
 
     app = Kui()
 
@@ -174,7 +177,27 @@
     routes = Routes(
         HttpRoute("/login", endpoint),
         HttpRoute("/register", endpoint),
     )
 
     assert routes[:] == routes
     assert routes[1:] == [routes[1]]
+
+
+def test_middleware_check_wraps():
+    from kui.asgi import HttpRoute
+
+    async def endpoint():
+        return "hello world"
+
+    def middleware(endpoint):
+        @functools.wraps(endpoint)
+        async def wrapped():
+            return endpoint()
+
+        return wrapped
+
+    with pytest.raises(
+        RuntimeError,
+        match="Cannot use `@functools.wraps` on a middleware.",
+    ):
+        _ = HttpRoute("/hello", endpoint) @ middleware
```

### Comparing `kui-1.4.0/tests/routing/test_tree.py` & `kui-1.5.0/tests/routing/test_tree.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/tests/test_responses.py` & `kui-1.5.0/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/tests/test_security.py` & `kui-1.5.0/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/tests/utils/test_importer.py` & `kui-1.5.0/tests/utils/test_importer.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/tests/wsgi/test_cors.py` & `kui-1.5.0/tests/wsgi/test_cors.py`

 * *Files identical despite different names*

### Comparing `kui-1.4.0/tests/wsgi/test_parameters.py` & `kui-1.5.0/tests/wsgi/test_parameters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import inspect
 import io
 
 import httpx
-import pytest
 from httpx import Client
 from typing_extensions import Annotated
 
 from kui.wsgi import (
     Body,
     Cookie,
     Depends,
     Header,
     Kui,
     Path,
     Query,
-    RequestAttr,
     UploadFile,
 )
 
 
 def test_path():
     app = Kui()
 
@@ -110,51 +108,14 @@
 
         resp = client.post("/", data={"name0": "aber"})
         assert resp.status_code == 422
 
     assert not inspect.signature(app.router.search("http", "/")[1]).parameters
 
 
-def test_request():
-    app0 = Kui()
-
-    @app0.router.http.get("/")
-    def homepage(app: Annotated[Kui, RequestAttr()]):
-        return str(app is app0)
-
-    @app0.router.http.get("/no-attr")
-    def no_attr(application: Annotated[Kui, RequestAttr()]):
-        return str(application is app0)
-
-    @app0.router.http.get("/no-attr-with-default")
-    def no_attr_with_default(application: Annotated[Kui, RequestAttr(app0)]):
-        return str(application is app0)
-
-    @app0.router.http.get("/no-attr-with-default-factory")
-    def no_attr_with_default_factory(
-        application: Annotated[Kui, RequestAttr(default_factory=lambda: app0)],
-    ):
-        return str(application is app0)
-
-    with Client(app=app0, base_url="http://testServer") as client:
-        resp = client.get("/")
-        assert resp.text == "True"
-
-        with pytest.raises(AttributeError):
-            client.get("/no-attr")
-
-        resp = client.get("/no-attr-with-default")
-        assert resp.text == "True"
-
-        resp = client.get("/no-attr-with-default-factory")
-        assert resp.text == "True"
-
-    assert not inspect.signature(app0.router.search("http", "/")[1]).parameters
-
-
 def test_depend():
     app = Kui()
 
     def get_name(name: Annotated[str, Body(...)]):
         return name
 
     @app.router.http.post("/")
@@ -212,21 +173,21 @@
         assert not in_gen
 
 
 def test_middleware():
     app = Kui()
 
     def middleware(endpoint):
-        def middleware_wrapper(query: str = Query(...)):
+        def middleware_wrapper(query: Annotated[str, Query(...)]):
             return endpoint()
 
         return middleware_wrapper
 
     @app.router.http.get("/", middlewares=[middleware])
-    def cookie(name: str = Cookie()):
+    def cookie(name: Annotated[str, Cookie()]):
         return name
 
     with Client(
         app=app, base_url="http://testServer", cookies={"name": "aber"}
     ) as client:
         resp = client.get("/")
         assert resp.status_code == 422
```

### Comparing `kui-1.4.0/PKG-INFO` & `kui-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kui
-Version: 1.4.0
+Version: 1.5.0
 Summary: An easy-to-use web framework.
 License: Apache-2.0
 Author-email: abersheeran <me@abersheeran.com>
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

