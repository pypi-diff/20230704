# Comparing `tmp/django-pfx-1.2.dev88.tar.gz` & `tmp/django-pfx-1.2.dev90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pfx-1.2.dev88.tar", last modified: Mon Jul  3 15:35:57 2023, max compression
+gzip compressed data, was "django-pfx-1.2.dev90.tar", last modified: Tue Jul  4 11:52:10 2023, max compression
```

## Comparing `django-pfx-1.2.dev88.tar` & `django-pfx-1.2.dev90.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.813988 django-pfx-1.2.dev88/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      486 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1509 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1692 2023-07-03 15:35:57.813988 django-pfx-1.2.dev88/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.794988 django-pfx-1.2.dev88/django_pfx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1692 2023-07-03 15:35:57.000000 django-pfx-1.2.dev88/django_pfx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3417 2023-07-03 15:35:57.000000 django-pfx-1.2.dev88/django_pfx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 15:35:57.000000 django-pfx-1.2.dev88/django_pfx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-03 15:35:57.000000 django-pfx-1.2.dev88/django_pfx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-03 15:35:57.000000 django-pfx-1.2.dev88/django_pfx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.794988 django-pfx-1.2.dev88/img/
--rw-rw-rw-   0 root         (0) root         (0)     3190 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/img/pfx.png
--rw-rw-rw-   0 root         (0) root         (0)     2682 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/img/pfx.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.794988 django-pfx-1.2.dev88/pfx/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.796987 django-pfx-1.2.dev88/pfx/pfxcore/
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.797988 django-pfx-1.2.dev88/pfx/pfxcore/apidoc/
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/apidoc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/apidoc/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     3012 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/apidoc/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/apidoc/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.798987 django-pfx-1.2.dev88/pfx/pfxcore/decorator/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/decorator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2530 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/decorator/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/default_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3462 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.798987 django-pfx-1.2.dev88/pfx/pfxcore/http/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/http/json_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.788987 django-pfx-1.2.dev88/pfx/pfxcore/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.788987 django-pfx-1.2.dev88/pfx/pfxcore/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.798987 django-pfx-1.2.dev88/pfx/pfxcore/locale/fr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     3331 2023-07-03 15:35:53.000000 django-pfx-1.2.dev88/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     5332 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.799987 django-pfx-1.2.dev88/pfx/pfxcore/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.799987 django-pfx-1.2.dev88/pfx/pfxcore/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7859 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/management/commands/makeapidoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.800988 django-pfx-1.2.dev88/pfx/pfxcore/middleware/
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/middleware/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2706 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/middleware/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/middleware/locale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.801988 django-pfx-1.2.dev88/pfx/pfxcore/models/
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2098 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/models/cache_mixins.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/models/not_null_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     3419 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/models/pfx_models.py
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/models/user_filtered_queryset_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.801988 django-pfx-1.2.dev88/pfx/pfxcore/serializers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/serializers/json.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2936 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/shortcuts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.801988 django-pfx-1.2.dev88/pfx/pfxcore/storage/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2131 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/storage/s3_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.789987 django-pfx-1.2.dev88/pfx/pfxcore/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.802987 django-pfx-1.2.dev88/pfx/pfxcore/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)      511 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/templates/registration/password_reset_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/templates/registration/password_reset_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/templates/registration/welcome_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/templates/registration/welcome_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)    10198 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/test.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.803988 django-pfx-1.2.dev88/pfx/pfxcore/views/
--rw-rw-rw-   0 root         (0) root         (0)      628 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15850 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/authentication_views.py
--rw-rw-rw-   0 root         (0) root         (0)    12218 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     4561 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/filters_views.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/locale_views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.807988 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      566 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/date_format.py
--rw-rw-rw-   0 root         (0) root         (0)     1192 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      492 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/list_count.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/list_items.py
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/list_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/list_order.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/list_search.py
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/media_redirect.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/meta_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/meta_filters.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/meta_orders.py
--rw-rw-rw-   0 root         (0) root         (0)     1412 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/subset.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/subset_limit.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/subset_offset.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/subset_page.py
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/subset_page_size.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/subset_page_subset.py
--rw-rw-rw-   0 root         (0) root         (0)    28550 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pfx/pfxcore/views/rest_views.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      440 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/runtest.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-07-03 15:35:57.814988 django-pfx-1.2.dev88/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.808987 django-pfx-1.2.dev88/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6487 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.809988 django-pfx-1.2.dev88/tests/settings/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/settings/ci.py
--rw-rw-rw-   0 root         (0) root         (0)     1644 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/settings/common.py
--rw-rw-rw-   0 root         (0) root         (0)      297 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/settings/dev.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/settings/dev_custom_example.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/settings/dev_default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:35:57.813988 django-pfx-1.2.dev88/tests/tests/
--rw-rw-rw-   0 root         (0) root         (0)      647 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2073 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/tests/basic_api_errors.py
--rw-rw-rw-   0 root         (0) root         (0)    46979 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/tests/basic_api_test.py
--rw-rw-rw-   0 root         (0) root         (0)    19335 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/tests/test_api_doc.py
--rw-rw-rw-   0 root         (0) root         (0)    29106 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/tests/test_auth_api.py
--rw-rw-rw-   0 root         (0) root         (0)     4221 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     9909 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/tests/test_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/tests/test_filters.py
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/tests/test_locale_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/tests/test_perm_tests.py
--rw-rw-rw-   0 root         (0) root         (0)     3725 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/tests/test_perms_api.py
--rw-rw-rw-   0 root         (0) root         (0)     6810 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/tests/test_shortcuts.py
--rw-rw-rw-   0 root         (0) root         (0)     1131 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/tests/test_timezone_middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     3395 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/tests/test_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/tests/test_user_queryset.py
--rw-rw-rw-   0 root         (0) root         (0)     3558 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/tests/test_view_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     7356 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/tests/test_view_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     8416 2023-07-03 15:35:13.000000 django-pfx-1.2.dev88/tests/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.225080 django-pfx-1.2.dev90/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      486 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-07-04 11:52:10.225080 django-pfx-1.2.dev90/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.205080 django-pfx-1.2.dev90/django_pfx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-07-04 11:52:10.000000 django-pfx-1.2.dev90/django_pfx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3417 2023-07-04 11:52:10.000000 django-pfx-1.2.dev90/django_pfx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 11:52:10.000000 django-pfx-1.2.dev90/django_pfx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-04 11:52:10.000000 django-pfx-1.2.dev90/django_pfx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-04 11:52:10.000000 django-pfx-1.2.dev90/django_pfx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.206081 django-pfx-1.2.dev90/img/
+-rw-rw-rw-   0 root         (0) root         (0)     3190 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/img/pfx.png
+-rw-rw-rw-   0 root         (0) root         (0)     2682 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/img/pfx.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.206081 django-pfx-1.2.dev90/pfx/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.208080 django-pfx-1.2.dev90/pfx/pfxcore/
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.208080 django-pfx-1.2.dev90/pfx/pfxcore/apidoc/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/apidoc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/apidoc/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3012 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/apidoc/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/apidoc/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.209081 django-pfx-1.2.dev90/pfx/pfxcore/decorator/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/decorator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/decorator/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/default_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3681 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.209081 django-pfx-1.2.dev90/pfx/pfxcore/http/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/http/json_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.200080 django-pfx-1.2.dev90/pfx/pfxcore/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.200080 django-pfx-1.2.dev90/pfx/pfxcore/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.210080 django-pfx-1.2.dev90/pfx/pfxcore/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     3331 2023-07-04 11:52:05.000000 django-pfx-1.2.dev90/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     5332 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.210080 django-pfx-1.2.dev90/pfx/pfxcore/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.210080 django-pfx-1.2.dev90/pfx/pfxcore/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7859 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/management/commands/makeapidoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.211080 django-pfx-1.2.dev90/pfx/pfxcore/middleware/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/middleware/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2706 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/middleware/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/middleware/locale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.212081 django-pfx-1.2.dev90/pfx/pfxcore/models/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/models/cache_mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/models/not_null_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     3419 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/models/pfx_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/models/user_filtered_queryset_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.212081 django-pfx-1.2.dev90/pfx/pfxcore/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/serializers/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2936 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/shortcuts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.213081 django-pfx-1.2.dev90/pfx/pfxcore/storage/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2131 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/storage/s3_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.201080 django-pfx-1.2.dev90/pfx/pfxcore/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.214080 django-pfx-1.2.dev90/pfx/pfxcore/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      511 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/templates/registration/password_reset_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/templates/registration/password_reset_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/templates/registration/welcome_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/templates/registration/welcome_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)    10198 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.215080 django-pfx-1.2.dev90/pfx/pfxcore/views/
+-rw-rw-rw-   0 root         (0) root         (0)      628 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15850 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/authentication_views.py
+-rw-rw-rw-   0 root         (0) root         (0)    12339 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     4561 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/filters_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/locale_views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.219081 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      566 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/date_format.py
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      492 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/list_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/list_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/list_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/list_order.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/list_search.py
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/media_redirect.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/meta_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/meta_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/meta_orders.py
+-rw-rw-rw-   0 root         (0) root         (0)     1412 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/subset.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/subset_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/subset_offset.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/subset_page.py
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/subset_page_size.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/subset_page_subset.py
+-rw-rw-rw-   0 root         (0) root         (0)    28550 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/rest_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)      440 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/runtest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-07-04 11:52:10.225080 django-pfx-1.2.dev90/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.220080 django-pfx-1.2.dev90/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6487 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.221080 django-pfx-1.2.dev90/tests/settings/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/settings/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/settings/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      297 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/settings/dev.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/settings/dev_custom_example.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/settings/dev_default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.225080 django-pfx-1.2.dev90/tests/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      647 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/basic_api_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    46979 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/basic_api_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    19712 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_api_doc.py
+-rw-rw-rw-   0 root         (0) root         (0)    29106 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_auth_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     4221 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     9909 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_locale_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_perm_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     3725 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_perms_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     6810 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_shortcuts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_timezone_middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)     3395 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_user_queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3558 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_view_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     7356 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_view_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     8416 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/views.py
```

### Comparing `django-pfx-1.2.dev88/.gitlab-ci.yml` & `django-pfx-1.2.dev90/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/LICENSE` & `django-pfx-1.2.dev90/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/PKG-INFO` & `django-pfx-1.2.dev90/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pfx
-Version: 1.2.dev88
+Version: 1.2.dev90
 Summary: Django PFX is a toolkit to build web APIs dedicated to be used by React progressive web app.
 Author: Hervé Martinet
 Author-email: herve.martinet@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://gitlab.com/hmartinet/django-pfx
 Project-URL: Tracker, https://gitlab.com/hmartinet/django-pfx/-/issues
 Classifier: Environment :: Web Environment
```

### Comparing `django-pfx-1.2.dev88/README.md` & `django-pfx-1.2.dev90/README.md`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/django_pfx.egg-info/PKG-INFO` & `django-pfx-1.2.dev90/django_pfx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pfx
-Version: 1.2.dev88
+Version: 1.2.dev90
 Summary: Django PFX is a toolkit to build web APIs dedicated to be used by React progressive web app.
 Author: Hervé Martinet
 Author-email: herve.martinet@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://gitlab.com/hmartinet/django-pfx
 Project-URL: Tracker, https://gitlab.com/hmartinet/django-pfx/-/issues
 Classifier: Environment :: Web Environment
```

### Comparing `django-pfx-1.2.dev88/django_pfx.egg-info/SOURCES.txt` & `django-pfx-1.2.dev90/django_pfx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/img/pfx.png` & `django-pfx-1.2.dev90/img/pfx.png`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/img/pfx.svg` & `django-pfx-1.2.dev90/img/pfx.svg`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/apidoc/parameters.py` & `django-pfx-1.2.dev90/pfx/pfxcore/apidoc/parameters.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/apidoc/schema.py` & `django-pfx-1.2.dev90/pfx/pfxcore/apidoc/schema.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/decorator/rest.py` & `django-pfx-1.2.dev90/pfx/pfxcore/decorator/rest.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/exceptions.py` & `django-pfx-1.2.dev90/pfx/pfxcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/fields.py` & `django-pfx-1.2.dev90/pfx/pfxcore/fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,14 +51,18 @@
 
 
 class MinutesDurationField(models.DurationField):
     RE_FLOAT = re.compile(r'^[0-9]*(\.[0-9]*)?$')
     RE_HH_MM = re.compile(r'^([0-9]*):([0-5][0-9])?$')
     RE_HUMAN = re.compile(
         r'^\s*(?:([0-9]*(?:\.[0-9]*)?)h)?\s*(?:([0-9]*)m)?\s*$')
+    schema = dict(type='object', properties=dict(
+        minutes=dict(type='number', example=90),
+        clock_format=dict(type='string', example='01:30'),
+        human_format=dict(type='string', example='1h 30m')))
 
     def to_python(self, value):
         if value is None or value == '':
             return None
         if isinstance(value, timedelta):
             return value
         if isinstance(value, (int, float)):
```

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo` & `django-pfx-1.2.dev90/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po` & `django-pfx-1.2.dev90/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/management/commands/makeapidoc.py` & `django-pfx-1.2.dev90/pfx/pfxcore/management/commands/makeapidoc.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/middleware/authentication.py` & `django-pfx-1.2.dev90/pfx/pfxcore/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/middleware/locale.py` & `django-pfx-1.2.dev90/pfx/pfxcore/middleware/locale.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/models/cache_mixins.py` & `django-pfx-1.2.dev90/pfx/pfxcore/models/cache_mixins.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/models/pfx_models.py` & `django-pfx-1.2.dev90/pfx/pfxcore/models/pfx_models.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/shortcuts.py` & `django-pfx-1.2.dev90/pfx/pfxcore/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/storage/s3_storage.py` & `django-pfx-1.2.dev90/pfx/pfxcore/storage/s3_storage.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/test.py` & `django-pfx-1.2.dev90/pfx/pfxcore/test.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/views/__init__.py` & `django-pfx-1.2.dev90/pfx/pfxcore/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/views/authentication_views.py` & `django-pfx-1.2.dev90/pfx/pfxcore/views/authentication_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/views/fields.py` & `django-pfx-1.2.dev90/pfx/pfxcore/views/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,16 @@
                     res.pop('format', None)
                     res['oneOf'] = [
                         properties.get('pk'),
                         dict(type='object',
                              properties=dict(pk=properties.get('pk')))]
                 else:
                     res['properties'] = properties
+        elif self.field_type == FieldType.MinutesDurationField:
+            res = pfx_fields.MinutesDurationField.schema
         elif self.field_type == FieldType.ModelObjectList:
             res['items'] = dict(type='object')
         res['readonly'] = self.readonly_create and self.readonly_update
         if self.choices:
             res['enum'] = list(self.choices)
         return res
```

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/views/filters_views.py` & `django-pfx-1.2.dev90/pfx/pfxcore/views/filters_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/views/locale_views.py` & `django-pfx-1.2.dev90/pfx/pfxcore/views/locale_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/__init__.py` & `django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/date_format.py` & `django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/date_format.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/groups.py` & `django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/groups.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/list_order.py` & `django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/list_order.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/views/parameters/subset.py` & `django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/subset.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/pfx/pfxcore/views/rest_views.py` & `django-pfx-1.2.dev90/pfx/pfxcore/views/rest_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/setup.cfg` & `django-pfx-1.2.dev90/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/models.py` & `django-pfx-1.2.dev90/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/settings/common.py` & `django-pfx-1.2.dev90/tests/settings/common.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/settings/dev_custom_example.py` & `django-pfx-1.2.dev90/tests/settings/dev_custom_example.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/tests/__init__.py` & `django-pfx-1.2.dev90/tests/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/tests/basic_api_errors.py` & `django-pfx-1.2.dev90/tests/tests/basic_api_errors.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/tests/basic_api_test.py` & `django-pfx-1.2.dev90/tests/tests/basic_api_test.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/tests/test_api_doc.py` & `django-pfx-1.2.dev90/tests/tests/test_api_doc.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,21 @@
             paths,
             '/books/{pk}.get.responses.200.content.application/json.schema'
         )['$ref'].split('/')[-1]
         self.assertIn("Book", schema_key)
         props = spec['components']['schemas'][schema_key]['properties']
         # Check that json_repr docstring from model is used
         self.assertJE(props, 'author.properties.new_field.type', 'string')
+        # Check MinutesDurationField fields json schema
+        self.assertJE(props, 'read_time.type', 'object')
+        self.assertJE(props, 'read_time.properties.minutes.type', 'number')
+        self.assertJE(
+            props, 'read_time.properties.clock_format.type', 'string')
+        self.assertJE(
+            props, 'read_time.properties.human_format.type', 'string')
 
         schema_key = self.get_val(
             paths,
             '/books/meta.get.responses.200.content.application/json.schema'
         )['$ref'].split('/')[-1]
         self.assertIn("form_meta", schema_key)
         props = spec['components']['schemas'][schema_key]['properties']
```

### Comparing `django-pfx-1.2.dev88/tests/tests/test_auth_api.py` & `django-pfx-1.2.dev90/tests/tests/test_auth_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/tests/test_cache.py` & `django-pfx-1.2.dev90/tests/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/tests/test_fields.py` & `django-pfx-1.2.dev90/tests/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/tests/test_filters.py` & `django-pfx-1.2.dev90/tests/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/tests/test_locale_api.py` & `django-pfx-1.2.dev90/tests/tests/test_locale_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/tests/test_perm_tests.py` & `django-pfx-1.2.dev90/tests/tests/test_perm_tests.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/tests/test_perms_api.py` & `django-pfx-1.2.dev90/tests/tests/test_perms_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/tests/test_shortcuts.py` & `django-pfx-1.2.dev90/tests/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/tests/test_timezone_middleware.py` & `django-pfx-1.2.dev90/tests/tests/test_timezone_middleware.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/tests/test_tools.py` & `django-pfx-1.2.dev90/tests/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/tests/test_user_queryset.py` & `django-pfx-1.2.dev90/tests/tests/test_user_queryset.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/tests/test_view_decorators.py` & `django-pfx-1.2.dev90/tests/tests/test_view_decorators.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/tests/test_view_fields.py` & `django-pfx-1.2.dev90/tests/tests/test_view_fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/urls.py` & `django-pfx-1.2.dev90/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev88/tests/views.py` & `django-pfx-1.2.dev90/tests/views.py`

 * *Files identical despite different names*

