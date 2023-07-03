# Comparing `tmp/django-extra-settings-0.9.0.tar.gz` & `tmp/django-extra-settings-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-extra-settings-0.9.0.tar", last modified: Tue Mar  7 00:46:35 2023, max compression
+gzip compressed data, was "django-extra-settings-0.9.1.tar", last modified: Tue Mar  7 14:28:32 2023, max compression
```

## Comparing `django-extra-settings-0.9.0.tar` & `django-extra-settings-0.9.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 00:46:35.394898 django-extra-settings-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-03-07 00:46:35.394898 django-extra-settings-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 00:46:35.382898 django-extra-settings-0.9.0/django_extra_settings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-03-07 00:46:35.000000 django-extra-settings-0.9.0/django_extra_settings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-07 00:46:35.000000 django-extra-settings-0.9.0/django_extra_settings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 00:46:35.000000 django-extra-settings-0.9.0/django_extra_settings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-07 00:46:35.000000 django-extra-settings-0.9.0/django_extra_settings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-07 00:46:35.000000 django-extra-settings-0.9.0/django_extra_settings.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 00:46:35.386898 django-extra-settings-0.9.0/extra_settings/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 00:46:35.378898 django-extra-settings-0.9.0/extra_settings/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 00:46:35.378898 django-extra-settings-0.9.0/extra_settings/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 00:46:35.386898 django-extra-settings-0.9.0/extra_settings/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 00:46:35.390898 django-extra-settings-0.9.0/extra_settings/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/migrations/0002_auto_20200826_1714.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/migrations/0003_modified_upload_to.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/migrations/0004_setting_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/migrations/0005_setting_value_json_alter_setting_value_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/migrations/0006_setting_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/migrations/0007_alter_settings_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/migrations/0008_auto_20221024_0717.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 00:46:35.378898 django-extra-settings-0.9.0/extra_settings/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 00:46:35.378898 django-extra-settings-0.9.0/extra_settings/static/extra_settings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 00:46:35.390898 django-extra-settings-0.9.0/extra_settings/static/extra_settings/css/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/static/extra_settings/css/extra_settings.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 00:46:35.390898 django-extra-settings-0.9.0/extra_settings/static/extra_settings/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/static/extra_settings/js/extra_settings.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 00:46:35.390898 django-extra-settings-0.9.0/extra_settings/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/templatetags/extra_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/extra_settings/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-03-07 00:46:35.394898 django-extra-settings-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 00:46:35.394898 django-extra-settings-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/tests/test_override_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-03-07 00:46:23.000000 django-extra-settings-0.9.0/tests/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:28:32.650360 django-extra-settings-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-03-07 14:28:32.650360 django-extra-settings-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:28:32.642359 django-extra-settings-0.9.1/django_extra_settings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-03-07 14:28:32.000000 django-extra-settings-0.9.1/django_extra_settings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-07 14:28:32.000000 django-extra-settings-0.9.1/django_extra_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 14:28:32.000000 django-extra-settings-0.9.1/django_extra_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-07 14:28:32.000000 django-extra-settings-0.9.1/django_extra_settings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-07 14:28:32.000000 django-extra-settings-0.9.1/django_extra_settings.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:28:32.646360 django-extra-settings-0.9.1/extra_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:28:32.642359 django-extra-settings-0.9.1/extra_settings/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:28:32.642359 django-extra-settings-0.9.1/extra_settings/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:28:32.646360 django-extra-settings-0.9.1/extra_settings/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:28:32.650360 django-extra-settings-0.9.1/extra_settings/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/migrations/0002_auto_20200826_1714.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/migrations/0003_modified_upload_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/migrations/0004_setting_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/migrations/0005_setting_value_json_alter_setting_value_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/migrations/0006_setting_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/migrations/0007_alter_settings_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/migrations/0008_auto_20221024_0717.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:28:32.642359 django-extra-settings-0.9.1/extra_settings/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:28:32.642359 django-extra-settings-0.9.1/extra_settings/static/extra_settings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:28:32.650360 django-extra-settings-0.9.1/extra_settings/static/extra_settings/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/static/extra_settings/css/extra_settings.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:28:32.650360 django-extra-settings-0.9.1/extra_settings/static/extra_settings/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/static/extra_settings/js/extra_settings.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:28:32.650360 django-extra-settings-0.9.1/extra_settings/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/templatetags/extra_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/extra_settings/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-03-07 14:28:32.650360 django-extra-settings-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:28:32.650360 django-extra-settings-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/tests/test_override_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-03-07 14:28:17.000000 django-extra-settings-0.9.1/tests/test_validators.py
```

### Comparing `django-extra-settings-0.9.0/LICENSE.txt` & `django-extra-settings-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/PKG-INFO` & `django-extra-settings-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-extra-settings
-Version: 0.9.0
+Version: 0.9.1
 Summary: config and manage typed extra settings using just the django admin.
 Home-page: https://github.com/fabiocaccamo/django-extra-settings
 Download-URL: https://github.com/fabiocaccamo/django-extra-settings/releases
 Author: Fabio Caccamo
 Author-email: fabio.caccamo@gmail.com
 Maintainer: Fabio Caccamo
 Maintainer-email: fabio.caccamo@gmail.com
```

### Comparing `django-extra-settings-0.9.0/README.md` & `django-extra-settings-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/django_extra_settings.egg-info/PKG-INFO` & `django-extra-settings-0.9.1/django_extra_settings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-extra-settings
-Version: 0.9.0
+Version: 0.9.1
 Summary: config and manage typed extra settings using just the django admin.
 Home-page: https://github.com/fabiocaccamo/django-extra-settings
 Download-URL: https://github.com/fabiocaccamo/django-extra-settings/releases
 Author: Fabio Caccamo
 Author-email: fabio.caccamo@gmail.com
 Maintainer: Fabio Caccamo
 Maintainer-email: fabio.caccamo@gmail.com
```

### Comparing `django-extra-settings-0.9.0/django_extra_settings.egg-info/SOURCES.txt` & `django-extra-settings-0.9.1/django_extra_settings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/extra_settings/admin.py` & `django-extra-settings-0.9.1/extra_settings/admin.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/extra_settings/apps.py` & `django-extra-settings-0.9.1/extra_settings/apps.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/extra_settings/cache.py` & `django-extra-settings-0.9.1/extra_settings/cache.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/extra_settings/fields.py` & `django-extra-settings-0.9.1/extra_settings/fields.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/extra_settings/forms.py` & `django-extra-settings-0.9.1/extra_settings/forms.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/extra_settings/locale/zh_Hans/LC_MESSAGES/django.po` & `django-extra-settings-0.9.1/extra_settings/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/extra_settings/migrations/0001_initial.py` & `django-extra-settings-0.9.1/extra_settings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/extra_settings/migrations/0002_auto_20200826_1714.py` & `django-extra-settings-0.9.1/extra_settings/migrations/0002_auto_20200826_1714.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/extra_settings/migrations/0003_modified_upload_to.py` & `django-extra-settings-0.9.1/extra_settings/migrations/0003_modified_upload_to.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/extra_settings/migrations/0005_setting_value_json_alter_setting_value_type.py` & `django-extra-settings-0.9.1/extra_settings/migrations/0005_setting_value_json_alter_setting_value_type.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/extra_settings/migrations/0007_alter_settings_validator.py` & `django-extra-settings-0.9.1/extra_settings/migrations/0007_alter_settings_validator.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     operations = [
         migrations.AlterField(
             model_name="setting",
             name="validator",
             field=models.CharField(
                 blank=True,
                 help_text=(
-                    "Full python path to a validator function, ",
-                    "eg. 'myapp.mymodule.my_validator'",
+                    "Full python path to a validator function, "
+                    "eg. 'myapp.mymodule.my_validator'"
                 ),
                 max_length=255,
                 null=True,
                 verbose_name="Validator",
             ),
         ),
     ]
```

### Comparing `django-extra-settings-0.9.0/extra_settings/migrations/0008_auto_20221024_0717.py` & `django-extra-settings-0.9.1/extra_settings/migrations/0008_auto_20221024_0717.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/extra_settings/models.py` & `django-extra-settings-0.9.1/extra_settings/models.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/extra_settings/settings.py` & `django-extra-settings-0.9.1/extra_settings/settings.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/extra_settings/signals.py` & `django-extra-settings-0.9.1/extra_settings/signals.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/extra_settings/static/extra_settings/js/extra_settings.js` & `django-extra-settings-0.9.1/extra_settings/static/extra_settings/js/extra_settings.js`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/extra_settings/test.py` & `django-extra-settings-0.9.1/extra_settings/test.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/setup.cfg` & `django-extra-settings-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/tests/test_admin.py` & `django-extra-settings-0.9.1/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/tests/test_cache.py` & `django-extra-settings-0.9.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/tests/test_forms.py` & `django-extra-settings-0.9.1/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/tests/test_metadata.py` & `django-extra-settings-0.9.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/tests/test_models.py` & `django-extra-settings-0.9.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/tests/test_override_settings.py` & `django-extra-settings-0.9.1/tests/test_override_settings.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/tests/test_templatetags.py` & `django-extra-settings-0.9.1/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-extra-settings-0.9.0/tests/test_validators.py` & `django-extra-settings-0.9.1/tests/test_validators.py`

 * *Files identical despite different names*

