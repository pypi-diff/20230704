# Comparing `tmp/django-adminlte-ui-2.0.0.tar.gz` & `tmp/django-adminlte-ui-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-adminlte-ui-2.0.0.tar", last modified: Tue Jun  6 05:48:16 2023, max compression
+gzip compressed data, was "django-adminlte-ui-2.1.0.tar", last modified: Tue Jul  4 09:46:13 2023, max compression
```

## Comparing `django-adminlte-ui-2.0.0.tar` & `django-adminlte-ui-2.1.0.tar`

### file list

```diff
@@ -1,582 +1,579 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.160289 django-adminlte-ui-2.0.0/adminlteui/
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.160289 django-adminlte-ui-2.0.0/adminlteui/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-06-06 05:48:15.000000 django-adminlte-ui-2.0.0/adminlteui/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)      283 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     5161 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/core.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.152289 django-adminlte-ui-2.0.0/adminlteui/locale/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.152289 django-adminlte-ui-2.0.0/adminlteui/locale/zh/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.160289 django-adminlte-ui-2.0.0/adminlteui/locale/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    17514 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/locale/zh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.152289 django-adminlte-ui-2.0.0/adminlteui/locale/zh-Hans/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.160289 django-adminlte-ui-2.0.0/adminlteui/locale/zh-Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/locale/zh-Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    17514 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/locale/zh-Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.160289 django-adminlte-ui-2.0.0/adminlteui/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.152289 django-adminlte-ui-2.0.0/adminlteui/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.152289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.164289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/css/
--rw-r--r--   0 runner    (1001) docker     (122)    57193 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/css/ionicons.css
--rw-r--r--   0 runner    (1001) docker     (122)    51284 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/css/ionicons.min.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.164289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   120724 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.eot
--rw-r--r--   0 runner    (1001) docker     (122)   333834 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.svg
--rw-r--r--   0 runner    (1001) docker     (122)   188508 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.ttf
--rw-r--r--   0 runner    (1001) docker     (122)    67904 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.woff
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.180289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/
--rw-r--r--   0 runner    (1001) docker     (122)    25682 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.css
--rw-r--r--   0 runner    (1001) docker     (122)    48005 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.css.map
--rw-r--r--   0 runner    (1001) docker     (122)    23411 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (122)    75600 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.min.css.map
--rw-r--r--   0 runner    (1001) docker     (122)   145933 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (122)   390887 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (122)   121457 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (122)   540434 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.180289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)    20127 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (122)   108738 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (122)    45404 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (122)    23424 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (122)    18028 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.180289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/js/
--rw-r--r--   0 runner    (1001) docker     (122)    75484 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (122)    39680 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/js/npm.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.152289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.152289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.164289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/
--rw-r--r--   0 runner    (1001) docker     (122)    13792 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.css
--rw-r--r--   0 runner    (1001) docker     (122)    16046 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.css.map
--rw-r--r--   0 runner    (1001) docker     (122)    13084 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.152289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.164289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/alpha-horizontal.png
--rw-r--r--   0 runner    (1001) docker     (122)      488 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/alpha.png
--rw-r--r--   0 runner    (1001) docker     (122)      478 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/hue-horizontal.png
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/hue.png
--rw-r--r--   0 runner    (1001) docker     (122)     4143 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/saturation.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.164289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/
--rw-r--r--   0 runner    (1001) docker     (122)    38926 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/bootstrap-colorpicker.js
--rw-r--r--   0 runner    (1001) docker     (122)    20771 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/bootstrap-colorpicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.168289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/
--rw-r--r--   0 runner    (1001) docker     (122)    17190 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.css
--rw-r--r--   0 runner    (1001) docker     (122)    18548 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.css.map
--rw-r--r--   0 runner    (1001) docker     (122)    15731 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.min.css
--rw-r--r--   0 runner    (1001) docker     (122)    18056 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.css
--rw-r--r--   0 runner    (1001) docker     (122)    20785 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.css.map
--rw-r--r--   0 runner    (1001) docker     (122)    16452 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.min.css
--rw-r--r--   0 runner    (1001) docker     (122)    22835 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.css
--rw-r--r--   0 runner    (1001) docker     (122)    23849 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.css.map
--rw-r--r--   0 runner    (1001) docker     (122)    21100 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.min.css
--rw-r--r--   0 runner    (1001) docker     (122)    23600 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.css
--rw-r--r--   0 runner    (1001) docker     (122)    25703 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.css.map
--rw-r--r--   0 runner    (1001) docker     (122)    21734 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.min.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.168289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/
--rw-r--r--   0 runner    (1001) docker     (122)    57898 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/bootstrap-datepicker.js
--rw-r--r--   0 runner    (1001) docker     (122)    33693 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/bootstrap-datepicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.176289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker-en-CA.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      704 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ar-tn.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      714 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ar.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.az.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bg.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bm.min.js
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bn.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.br.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bs.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ca.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.cs.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      433 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.cy.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.da.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.de.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      764 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.el.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-AU.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-CA.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-GB.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-IE.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-NZ.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-ZA.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.eo.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.es.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.et.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      528 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.eu.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fa.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      528 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fi.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      488 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fo.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      512 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fr-CH.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fr.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.gl.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      563 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.he.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hi.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hr.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      541 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hu.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hy.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.id.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.is.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      506 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.it-CH.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      525 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.it.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      502 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ja.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      970 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ka.min.js
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kh.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      649 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kk.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      945 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.km.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ko.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kr.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.lt.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      526 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.lv.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.me.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.mk.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      638 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.mn.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      448 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ms.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.nl-BE.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.nl.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.no.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.oc.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.pl.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.pt-BR.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.pt.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ro.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.rs-latin.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      817 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.rs.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      731 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ru.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.si.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sk.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sl.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sq.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      478 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sr-latin.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      651 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sr.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sv.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      431 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sw.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      934 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ta.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tg.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.th.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      530 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tk.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tr.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uk.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uz-cyrl.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      516 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uz-latn.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      551 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.vi.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      613 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.zh-CN.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.zh-TW.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.176289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-daterangepicker/
--rw-r--r--   0 runner    (1001) docker     (122)     8163 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-daterangepicker/daterangepicker.css
--rw-r--r--   0 runner    (1001) docker     (122)    71115 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-daterangepicker/daterangepicker.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.180289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/
--rw-r--r--   0 runner    (1001) docker     (122)      889 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/.bower.json
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/License.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2431 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/Readme.md
--rw-r--r--   0 runner    (1001) docker     (122)      692 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/bower.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.184289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/js/
--rw-r--r--   0 runner    (1001) docker     (122)   447569 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.js
--rw-r--r--   0 runner    (1001) docker     (122)    82411 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.184289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/.bower.json
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/License.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/Readme.md
--rw-r--r--   0 runner    (1001) docker     (122)      829 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/bower.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.184289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/css/
--rw-r--r--   0 runner    (1001) docker     (122)     4791 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (122)     4188 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.184289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/js/
--rw-r--r--   0 runner    (1001) docker     (122)     4559 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (122)     1966 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/fastclick/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.184289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/fastclick/lib/
--rw-r--r--   0 runner    (1001) docker     (122)    25965 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/fastclick/lib/fastclick.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.184289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/css/
--rw-r--r--   0 runner    (1001) docker     (122)    37414 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (122)    21778 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.css.map
--rw-r--r--   0 runner    (1001) docker     (122)    31000 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.188289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   134808 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (122)   165742 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (122)   444379 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (122)   165548 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (122)    98024 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (122)    77160 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.188289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/
--rw-r--r--   0 runner    (1001) docker     (122)     9165 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/core.js
--rw-r--r--   0 runner    (1001) docker     (122)   280364 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.js
--rw-r--r--   0 runner    (1001) docker     (122)    88145 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (122)   136397 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.min.map
--rw-r--r--   0 runner    (1001) docker     (122)   227022 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.js
--rw-r--r--   0 runner    (1001) docker     (122)    71037 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.min.js
--rw-r--r--   0 runner    (1001) docker     (122)   108757 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.min.map
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.188289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/
--rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.188289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/
--rw-r--r--   0 runner    (1001) docker     (122)    65666 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.js
--rw-r--r--   0 runner    (1001) docker     (122)    19841 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.js
--rw-r--r--   0 runner    (1001) docker     (122)    30740 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.map
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.188289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery-slimscroll/
--rw-r--r--   0 runner    (1001) docker     (122)    13832 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery-slimscroll/jquery.slimscroll.js
--rw-r--r--   0 runner    (1001) docker     (122)     4724 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery-slimscroll/jquery.slimscroll.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.188289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/css/
--rw-r--r--   0 runner    (1001) docker     (122)    17340 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/css/select2.css
--rw-r--r--   0 runner    (1001) docker     (122)    14954 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/css/select2.min.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.192289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.196289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/af.js
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ar.js
--rw-r--r--   0 runner    (1001) docker     (122)      720 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/az.js
--rw-r--r--   0 runner    (1001) docker     (122)      967 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/bg.js
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/bn.js
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/bs.js
--rw-r--r--   0 runner    (1001) docker     (122)      899 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ca.js
--rw-r--r--   0 runner    (1001) docker     (122)     1291 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/cs.js
--rw-r--r--   0 runner    (1001) docker     (122)      827 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/da.js
--rw-r--r--   0 runner    (1001) docker     (122)      876 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/de.js
--rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/dsb.js
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/el.js
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/en.js
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/es.js
--rw-r--r--   0 runner    (1001) docker     (122)      800 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/et.js
--rw-r--r--   0 runner    (1001) docker     (122)      867 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/eu.js
--rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/fa.js
--rw-r--r--   0 runner    (1001) docker     (122)      802 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/fi.js
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/fr.js
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/gl.js
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/he.js
--rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hi.js
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hr.js
--rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hsb.js
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hu.js
--rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hy.js
--rw-r--r--   0 runner    (1001) docker     (122)      767 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/id.js
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/is.js
--rw-r--r--   0 runner    (1001) docker     (122)      896 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/it.js
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ja.js
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ka.js
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/km.js
--rw-r--r--   0 runner    (1001) docker     (122)      854 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ko.js
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/lt.js
--rw-r--r--   0 runner    (1001) docker     (122)      899 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/lv.js
--rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/mk.js
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ms.js
--rw-r--r--   0 runner    (1001) docker     (122)      777 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/nb.js
--rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ne.js
--rw-r--r--   0 runner    (1001) docker     (122)      903 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/nl.js
--rw-r--r--   0 runner    (1001) docker     (122)      946 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/pl.js
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ps.js
--rw-r--r--   0 runner    (1001) docker     (122)      875 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (122)      877 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/pt.js
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ro.js
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ru.js
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sk.js
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sl.js
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sq.js
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sr-Cyrl.js
--rw-r--r--   0 runner    (1001) docker     (122)      979 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sr.js
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sv.js
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/th.js
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/tk.js
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/tr.js
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/uk.js
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/vi.js
--rw-r--r--   0 runner    (1001) docker     (122)      767 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/zh-CN.js
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/zh-TW.js
--rw-r--r--   0 runner    (1001) docker     (122)   167790 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/select2.full.js
--rw-r--r--   0 runner    (1001) docker     (122)    76652 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/select2.full.min.js
--rw-r--r--   0 runner    (1001) docker     (122)   147864 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/select2.js
--rw-r--r--   0 runner    (1001) docker     (122)    68382 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/select2.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.200289 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/
--rw-r--r--   0 runner    (1001) docker     (122)   127585 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/AdminLTE.css
--rw-r--r--   0 runner    (1001) docker     (122)   106548 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/AdminLTE.min.css
--rw-r--r--   0 runner    (1001) docker     (122)   309656 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/adminlte.css.map
--rw-r--r--   0 runner    (1001) docker     (122)   306319 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/adminlte.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.200289 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/
--rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-bootstrap-social.css
--rw-r--r--   0 runner    (1001) docker     (122)    26356 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-bootstrap-social.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-fullcalendar.css
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-fullcalendar.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-select2.css
--rw-r--r--   0 runner    (1001) docker     (122)     2732 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-select2.min.css
--rw-r--r--   0 runner    (1001) docker     (122)    91800 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-without-plugins.css
--rw-r--r--   0 runner    (1001) docker     (122)    75269 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-without-plugins.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     8670 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/app.css
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/django.css
--rw-r--r--   0 runner    (1001) docker     (122)    16022 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/fontgoogle.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.204289 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/
--rw-r--r--   0 runner    (1001) docker     (122)    48473 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/_all-skins.css
--rw-r--r--   0 runner    (1001) docker     (122)    41635 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/_all-skins.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     4841 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-black-light.css
--rw-r--r--   0 runner    (1001) docker     (122)     4134 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-black-light.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     4163 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-black.css
--rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-black.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     4533 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-blue-light.css
--rw-r--r--   0 runner    (1001) docker     (122)     3916 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-blue-light.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     3688 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-blue.css
--rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-blue.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     4299 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-green-light.css
--rw-r--r--   0 runner    (1001) docker     (122)     3719 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-green-light.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-green.css
--rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-green.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     4350 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-purple-light.css
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-purple-light.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-purple.css
--rw-r--r--   0 runner    (1001) docker     (122)     3055 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-purple.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     4197 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-red-light.css
--rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-red-light.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-red.css
--rw-r--r--   0 runner    (1001) docker     (122)     2920 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-red.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     4350 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-yellow-light.css
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-yellow-light.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-yellow.css
--rw-r--r--   0 runner    (1001) docker     (122)     3055 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-yellow.min.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.204289 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/calendar-icons.svg
--rw-r--r--   0 runner    (1001) docker     (122)   223437 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/default-log.svg
--rw-r--r--   0 runner    (1001) docker     (122)     7070 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/default.jpg
--rw-r--r--   0 runner    (1001) docker     (122)     3291 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/selector-icons.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.204289 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/
--rw-r--r--   0 runner    (1001) docker     (122)    29749 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/adminlte.js
--rw-r--r--   0 runner    (1001) docker     (122)    13611 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/adminlte.min.js
--rw-r--r--   0 runner    (1001) docker     (122)    18608 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/demo.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.204289 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/pages/
--rw-r--r--   0 runner    (1001) docker     (122)     6112 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/pages/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (122)     9607 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/pages/dashboard2.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.160289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.204289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-slider/
--rw-r--r--   0 runner    (1001) docker     (122)    51062 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-slider/bootstrap-slider.js
--rw-r--r--   0 runner    (1001) docker     (122)     8486 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-slider/slider.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.208289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/
--rw-r--r--   0 runner    (1001) docker     (122)   566620 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js
--rw-r--r--   0 runner    (1001) docker     (122)   210932 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js
--rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css
--rw-r--r--   0 runner    (1001) docker     (122)     2226 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.208289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/all.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.212289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/
--rw-r--r--   0 runner    (1001) docker     (122)    13773 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/_all.css
--rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/aero.css
--rw-r--r--   0 runner    (1001) docker     (122)     1520 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/aero.png
--rw-r--r--   0 runner    (1001) docker     (122)     3218 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/aero@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/blue.css
--rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/blue.png
--rw-r--r--   0 runner    (1001) docker     (122)     3217 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/blue@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/flat.css
--rw-r--r--   0 runner    (1001) docker     (122)     1515 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/flat.png
--rw-r--r--   0 runner    (1001) docker     (122)     3217 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/flat@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/green.css
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/green.png
--rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/green@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/grey.css
--rw-r--r--   0 runner    (1001) docker     (122)     1516 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/grey.png
--rw-r--r--   0 runner    (1001) docker     (122)     3217 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/grey@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/orange.css
--rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/orange.png
--rw-r--r--   0 runner    (1001) docker     (122)     3275 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/orange@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/pink.css
--rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/pink.png
--rw-r--r--   0 runner    (1001) docker     (122)     3218 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/pink@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/purple.css
--rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/purple.png
--rw-r--r--   0 runner    (1001) docker     (122)     3218 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/purple@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/red.css
--rw-r--r--   0 runner    (1001) docker     (122)     1516 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/red.png
--rw-r--r--   0 runner    (1001) docker     (122)     3276 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/red@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/yellow.css
--rw-r--r--   0 runner    (1001) docker     (122)     1516 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/yellow.png
--rw-r--r--   0 runner    (1001) docker     (122)     3216 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/yellow@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.212289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/futurico/
--rw-r--r--   0 runner    (1001) docker     (122)     1421 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico.css
--rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico.png
--rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)    14161 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/icheck.js
--rw-r--r--   0 runner    (1001) docker     (122)     4516 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/icheck.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.212289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/
--rw-r--r--   0 runner    (1001) docker     (122)    21689 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/_all.css
--rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/aero.css
--rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/blue.css
--rw-r--r--   0 runner    (1001) docker     (122)     2244 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/green.css
--rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/grey.css
--rw-r--r--   0 runner    (1001) docker     (122)     2103 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/line.css
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/line.png
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/line@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     2260 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/orange.css
--rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/pink.css
--rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/purple.css
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/red.css
--rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/yellow.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.216289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/
--rw-r--r--   0 runner    (1001) docker     (122)    14176 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/_all.css
--rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/aero.css
--rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/aero.png
--rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/aero@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/blue.css
--rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/blue.png
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/blue@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/green.css
--rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/green.png
--rw-r--r--   0 runner    (1001) docker     (122)     1408 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/green@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/grey.css
--rw-r--r--   0 runner    (1001) docker     (122)     1142 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/grey.png
--rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/grey@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal.css
--rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal.png
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/orange.css
--rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/orange.png
--rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/orange@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/pink.css
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/pink.png
--rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/pink@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/purple.css
--rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/purple.png
--rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/purple@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/red.css
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/red.png
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/red@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow.css
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow.png
--rw-r--r--   0 runner    (1001) docker     (122)     1406 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.216289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/polaris/
--rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris.css
--rw-r--r--   0 runner    (1001) docker     (122)     6401 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris.png
--rw-r--r--   0 runner    (1001) docker     (122)    16760 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.220289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/
--rw-r--r--   0 runner    (1001) docker     (122)    15591 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/_all.css
--rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/aero.css
--rw-r--r--   0 runner    (1001) docker     (122)     2167 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/aero.png
--rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/aero@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/blue.css
--rw-r--r--   0 runner    (1001) docker     (122)     2185 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/blue.png
--rw-r--r--   0 runner    (1001) docker     (122)     4485 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/blue@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/green.css
--rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/green.png
--rw-r--r--   0 runner    (1001) docker     (122)     4498 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/green@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/grey.css
--rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/grey.png
--rw-r--r--   0 runner    (1001) docker     (122)     4483 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/grey@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/orange.css
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/orange.png
--rw-r--r--   0 runner    (1001) docker     (122)     4474 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/orange@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/pink.css
--rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/pink.png
--rw-r--r--   0 runner    (1001) docker     (122)     4479 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/pink@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/purple.css
--rw-r--r--   0 runner    (1001) docker     (122)     2188 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/purple.png
--rw-r--r--   0 runner    (1001) docker     (122)     4501 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/purple@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1594 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/red.css
--rw-r--r--   0 runner    (1001) docker     (122)     2190 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/red.png
--rw-r--r--   0 runner    (1001) docker     (122)     4490 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/red@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1546 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/square.css
--rw-r--r--   0 runner    (1001) docker     (122)     2175 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/square.png
--rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/square@2x.png
--rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/yellow.css
--rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/yellow.png
--rw-r--r--   0 runner    (1001) docker     (122)     4385 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/yellow@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.220289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/
--rw-r--r--   0 runner    (1001) docker     (122)    22814 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.date.extensions.js
--rw-r--r--   0 runner    (1001) docker     (122)     5315 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.extensions.js
--rw-r--r--   0 runner    (1001) docker     (122)    90539 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.js
--rw-r--r--   0 runner    (1001) docker     (122)     9118 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.numeric.extensions.js
--rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.phone.extensions.js
--rw-r--r--   0 runner    (1001) docker     (122)     9392 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.regex.extensions.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.224289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/phone-codes/
--rw-r--r--   0 runner    (1001) docker     (122)     3631 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/phone-codes/phone-be.json
--rw-r--r--   0 runner    (1001) docker     (122)    39492 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/phone-codes/phone-codes.json
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/phone-codes/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.224289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jQueryUI/
--rw-r--r--   0 runner    (1001) docker     (122)   470596 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jQueryUI/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (122)   240427 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jQueryUI/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.224289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-1.2.2.css
--rw-r--r--   0 runner    (1001) docker     (122)    33323 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js
--rw-r--r--   0 runner    (1001) docker     (122)    95062 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-usa-en.js
--rw-r--r--   0 runner    (1001) docker     (122)   144313 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-world-mill-en.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.224289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/
--rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/pace.css
--rw-r--r--   0 runner    (1001) docker     (122)    26566 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/pace.js
--rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/pace.min.css
--rw-r--r--   0 runner    (1001) docker     (122)    12507 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/pace.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.224289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/
--rw-r--r--   0 runner    (1001) docker     (122)    71385 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/bootstrap-slider.js
--rw-r--r--   0 runner    (1001) docker     (122)    38635 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/bootstrap-slider.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.224289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/
--rw-r--r--   0 runner    (1001) docker     (122)    10368 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/bootstrap-slider.css
--rw-r--r--   0 runner    (1001) docker     (122)     9336 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/bootstrap-slider.min.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.228289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/
--rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.css
--rw-r--r--   0 runner    (1001) docker     (122)    34375 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.js
--rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.min.css
--rw-r--r--   0 runner    (1001) docker     (122)    18685 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.160289 django-adminlte-ui-2.0.0/adminlteui/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.228289 django-adminlte-ui-2.0.0/adminlteui/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (122)      300 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/404.html
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/500.html
--rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/actions.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.160289 django-adminlte-ui-2.0.0/adminlteui/templates/admin/auth/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.228289 django-adminlte-ui-2.0.0/adminlteui/templates/admin/auth/user/
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/auth/user/add_form.html
--rw-r--r--   0 runner    (1001) docker     (122)     5326 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/auth/user/change_password.html
--rw-r--r--   0 runner    (1001) docker     (122)    25938 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     3325 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/base_site.html
--rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/change_form.html
--rw-r--r--   0 runner    (1001) docker     (122)     5698 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/change_list.html
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/change_list_object_tools.html
--rw-r--r--   0 runner    (1001) docker     (122)     1897 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/change_list_results.html
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/date_hierarchy.html
--rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/delete_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/delete_selected_confirmation.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.228289 django-adminlte-ui-2.0.0/adminlteui/templates/admin/edit_inline/
--rw-r--r--   0 runner    (1001) docker     (122)     2906 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/edit_inline/stacked.html
--rw-r--r--   0 runner    (1001) docker     (122)     5550 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/edit_inline/tabular.html
--rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/filter.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/adminlteui/templates/admin/includes/
--rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/includes/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/includes/object_delete_summary.html
--rw-r--r--   0 runner    (1001) docker     (122)     7379 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/index.html
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/invalid_setup.html
--rw-r--r--   0 runner    (1001) docker     (122)     5090 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/login.html
--rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/object_history.html
--rw-r--r--   0 runner    (1001) docker     (122)     3829 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/pagination.html
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/search_form.html
--rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/submit_line.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/adminlteui/templates/adminlte/
--rw-r--r--   0 runner    (1001) docker     (122)      707 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/adminlte/form.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/adminlteui/templates/adminlte/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/adminlte/widgets/select.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/adminlteui/templates/registration/
--rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/registration/logged_out.html
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/registration/password_change_done.html
--rw-r--r--   0 runner    (1001) docker     (122)     5828 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/registration/password_change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/adminlteui/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templatetags/adminlte_core.py
--rw-r--r--   0 runner    (1001) docker     (122)     3297 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templatetags/adminlte_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     4638 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templatetags/adminlte_menu.py
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/views.py
--rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/django_adminlte_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-06 05:48:16.000000 django-adminlte-ui-2.0.0/django_adminlte_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    33174 2023-06-06 05:48:16.000000 django-adminlte-ui-2.0.0/django_adminlte_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 05:48:16.000000 django-adminlte-ui-2.0.0/django_adminlte_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 05:48:15.000000 django-adminlte-ui-2.0.0/django_adminlte_ui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-06 05:48:16.000000 django-adminlte-ui-2.0.0/django_adminlte_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      650 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.552107 django-adminlte-ui-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-07-04 09:46:13.552107 django-adminlte-ui-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.416106 django-adminlte-ui-2.1.0/adminlteui/
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.416106 django-adminlte-ui-2.1.0/adminlteui/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-07-04 09:46:13.000000 django-adminlte-ui-2.1.0/adminlteui/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5744 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3046 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.400106 django-adminlte-ui-2.1.0/adminlteui/locale/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.400106 django-adminlte-ui-2.1.0/adminlteui/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.416106 django-adminlte-ui-2.1.0/adminlteui/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1912 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    14414 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/locale/zh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.400106 django-adminlte-ui-2.1.0/adminlteui/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.416106 django-adminlte-ui-2.1.0/adminlteui/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1912 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    14414 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.416106 django-adminlte-ui-2.1.0/adminlteui/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.400106 django-adminlte-ui-2.1.0/adminlteui/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.408106 django-adminlte-ui-2.1.0/adminlteui/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.408106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.400106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/Ionicons/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.416106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/Ionicons/css/
+-rw-r--r--   0 runner    (1001) docker     (122)    57193 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/Ionicons/css/ionicons.css
+-rw-r--r--   0 runner    (1001) docker     (122)    51284 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/Ionicons/css/ionicons.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.420106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/Ionicons/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   120724 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.eot
+-rw-r--r--   0 runner    (1001) docker     (122)   333834 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.svg
+-rw-r--r--   0 runner    (1001) docker     (122)   188508 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    67904 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.woff
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.404106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.404106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.452106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (122)    25682 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.css
+-rw-r--r--   0 runner    (1001) docker     (122)    48005 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)    23411 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)    75600 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)   145933 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (122)   390887 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)   121457 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)   540434 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.452106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)    20127 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (122)   108738 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (122)    45404 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    23424 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (122)    18028 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.452106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    75484 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (122)    39680 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/js/npm.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.400106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.404106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.420106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (122)    13792 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.css
+-rw-r--r--   0 runner    (1001) docker     (122)    16046 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)    13084 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.400106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.424106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/alpha-horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/alpha.png
+-rw-r--r--   0 runner    (1001) docker     (122)      478 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/hue-horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/hue.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4143 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/saturation.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.424106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    38926 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/bootstrap-colorpicker.js
+-rw-r--r--   0 runner    (1001) docker     (122)    20771 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/bootstrap-colorpicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.404106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.404106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.428106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (122)    17190 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.css
+-rw-r--r--   0 runner    (1001) docker     (122)    18548 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)    15731 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)    18056 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.css
+-rw-r--r--   0 runner    (1001) docker     (122)    20785 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)    16452 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)    22835 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.css
+-rw-r--r--   0 runner    (1001) docker     (122)    23849 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)    21100 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)    23600 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.css
+-rw-r--r--   0 runner    (1001) docker     (122)    25703 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)    21734 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.428106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    57898 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/bootstrap-datepicker.js
+-rw-r--r--   0 runner    (1001) docker     (122)    33693 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/bootstrap-datepicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.448106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker-en-CA.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ar-tn.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      714 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ar.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.az.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bg.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bm.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bn.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.br.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bs.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ca.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.cs.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.cy.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.da.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.de.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.el.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-AU.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-CA.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-GB.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-IE.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-NZ.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-ZA.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.eo.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.es.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.et.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.eu.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fa.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fi.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fo.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      512 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fr-CH.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fr.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.gl.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      563 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.he.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hi.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hr.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      541 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hu.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hy.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.id.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.is.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.it-CH.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      525 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.it.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      502 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ja.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ka.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kh.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      649 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kk.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      945 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.km.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ko.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kr.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.lt.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.lv.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.me.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.mk.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.mn.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      448 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ms.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.nl-BE.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.nl.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.no.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.oc.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.pl.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.pt-BR.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.pt.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ro.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.rs-latin.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      817 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.rs.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      731 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ru.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.si.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sk.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sl.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sq.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      478 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sr-latin.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      651 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sr.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sv.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      431 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sw.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      934 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ta.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tg.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.th.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tk.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tr.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uk.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uz-cyrl.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uz-latn.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      551 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.vi.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.zh-CN.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.zh-TW.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.448106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-daterangepicker/
+-rw-r--r--   0 runner    (1001) docker     (122)     8163 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-daterangepicker/daterangepicker.css
+-rw-r--r--   0 runner    (1001) docker     (122)    71115 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-daterangepicker/daterangepicker.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.404106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/datatables.net/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.456106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/datatables.net/js/
+-rw-r--r--   0 runner    (1001) docker     (122)   447569 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.js
+-rw-r--r--   0 runner    (1001) docker     (122)    82411 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.404106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/datatables.net-bs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.452106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/datatables.net-bs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     4791 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4188 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.456106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/datatables.net-bs/js/
+-rw-r--r--   0 runner    (1001) docker     (122)     4559 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1966 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.404106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/fastclick/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.456106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/fastclick/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)    25965 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/fastclick/lib/fastclick.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.404106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.456106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/css/
+-rw-r--r--   0 runner    (1001) docker     (122)    37414 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (122)    21778 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)    31000 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.460106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   134808 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (122)   165742 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (122)   444379 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (122)   165548 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    98024 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (122)    77160 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.404106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.464106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/dist/
+-rw-r--r--   0 runner    (1001) docker     (122)     9165 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/dist/core.js
+-rw-r--r--   0 runner    (1001) docker     (122)   280364 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/dist/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (122)    88145 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/dist/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)   136397 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/dist/jquery.min.map
+-rw-r--r--   0 runner    (1001) docker     (122)   227022 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.js
+-rw-r--r--   0 runner    (1001) docker     (122)    71037 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)   108757 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.min.map
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.404106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/external/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.464106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/external/sizzle/
+-rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/external/sizzle/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.464106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/
+-rw-r--r--   0 runner    (1001) docker     (122)    65666 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.js
+-rw-r--r--   0 runner    (1001) docker     (122)    19841 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)    30740 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.map
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.460106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery-slimscroll/
+-rw-r--r--   0 runner    (1001) docker     (122)    13832 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery-slimscroll/jquery.slimscroll.js
+-rw-r--r--   0 runner    (1001) docker     (122)     4724 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery-slimscroll/jquery.slimscroll.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.468106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/moment/
+-rw-r--r--   0 runner    (1001) docker     (122)   541363 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/moment/moment-with-locales.js
+-rw-r--r--   0 runner    (1001) docker     (122)   336451 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/moment/moment-with-locales.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.408106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.408106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.468106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (122)    17340 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/css/select2.css
+-rw-r--r--   0 runner    (1001) docker     (122)    14954 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/css/select2.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.468106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.484106 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/af.js
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ar.js
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/az.js
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/bg.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/bn.js
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/bs.js
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ca.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1291 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/cs.js
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/da.js
+-rw-r--r--   0 runner    (1001) docker     (122)      876 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/de.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/dsb.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/el.js
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/en.js
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/es.js
+-rw-r--r--   0 runner    (1001) docker     (122)      800 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/et.js
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/eu.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/fa.js
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/fi.js
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/fr.js
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/gl.js
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/he.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/hi.js
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/hr.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/hsb.js
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/hu.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/hy.js
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/id.js
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/is.js
+-rw-r--r--   0 runner    (1001) docker     (122)      896 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/it.js
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ja.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ka.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/km.js
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ko.js
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/lt.js
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/lv.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/mk.js
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ms.js
+-rw-r--r--   0 runner    (1001) docker     (122)      777 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/nb.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ne.js
+-rw-r--r--   0 runner    (1001) docker     (122)      903 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/nl.js
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/pl.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ps.js
+-rw-r--r--   0 runner    (1001) docker     (122)      875 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (122)      877 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/pt.js
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ro.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ru.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/sk.js
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/sl.js
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/sq.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/sr-Cyrl.js
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/sr.js
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/sv.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/th.js
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/tk.js
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/tr.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/uk.js
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/vi.js
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/zh-CN.js
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/zh-TW.js
+-rw-r--r--   0 runner    (1001) docker     (122)   167790 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/select2.full.js
+-rw-r--r--   0 runner    (1001) docker     (122)    76652 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/select2.full.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)   147864 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/select2.js
+-rw-r--r--   0 runner    (1001) docker     (122)    68382 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/select2.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.408106 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.488106 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (122)   127585 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/AdminLTE.css
+-rw-r--r--   0 runner    (1001) docker     (122)   106548 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/AdminLTE.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)   309656 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/adminlte.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)   306319 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/adminlte.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.488106 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/alt/
+-rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/alt/AdminLTE-bootstrap-social.css
+-rw-r--r--   0 runner    (1001) docker     (122)    26356 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/alt/AdminLTE-bootstrap-social.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/alt/AdminLTE-fullcalendar.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/alt/AdminLTE-fullcalendar.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/alt/AdminLTE-select2.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2732 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/alt/AdminLTE-select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)    91800 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/alt/AdminLTE-without-plugins.css
+-rw-r--r--   0 runner    (1001) docker     (122)    75269 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/alt/AdminLTE-without-plugins.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     8670 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/app.css
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/django.css
+-rw-r--r--   0 runner    (1001) docker     (122)    16022 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/fontgoogle.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.496106 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/
+-rw-r--r--   0 runner    (1001) docker     (122)    48473 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/_all-skins.css
+-rw-r--r--   0 runner    (1001) docker     (122)    41635 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/_all-skins.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4841 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-black-light.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4134 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-black-light.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4163 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-black.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-black.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4533 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-blue-light.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3916 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-blue-light.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3688 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-blue.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-blue.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4299 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-green-light.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3719 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-green-light.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-green.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-green.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4350 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-purple-light.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-purple-light.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-purple.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3055 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-purple.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4197 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-red-light.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-red-light.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-red.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2920 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-red.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4350 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-yellow-light.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-yellow-light.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-yellow.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3055 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-yellow.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.496106 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/img/
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/img/calendar-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (122)   223437 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/img/default-log.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     7070 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/img/default.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)     3291 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/img/selector-icons.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.496106 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    29749 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/js/adminlte.js
+-rw-r--r--   0 runner    (1001) docker     (122)    13611 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/js/adminlte.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)    18608 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/js/demo.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.500106 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/js/pages/
+-rw-r--r--   0 runner    (1001) docker     (122)     6112 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/js/pages/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (122)     9607 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/js/pages/dashboard2.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.412106 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.500106 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/bootstrap-slider/
+-rw-r--r--   0 runner    (1001) docker     (122)    51062 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/bootstrap-slider/bootstrap-slider.js
+-rw-r--r--   0 runner    (1001) docker     (122)     8486 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/bootstrap-slider/slider.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.500106 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/
+-rw-r--r--   0 runner    (1001) docker     (122)   566620 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js
+-rw-r--r--   0 runner    (1001) docker     (122)   210932 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2226 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.504106 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/all.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.512107 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/
+-rw-r--r--   0 runner    (1001) docker     (122)    13773 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/_all.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/aero.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1520 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/aero.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3218 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/aero@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/blue.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/blue.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3217 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/blue@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/flat.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1515 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/flat.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3217 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/flat@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/green.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/green.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/green@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/grey.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1516 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/grey.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3217 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/grey@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/orange.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/orange.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3275 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/orange@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/pink.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/pink.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3218 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/pink@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/purple.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/purple.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3218 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/purple@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/red.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1516 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/red.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3276 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/red@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/yellow.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1516 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/yellow.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3216 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/yellow@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.512107 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/futurico/
+-rw-r--r--   0 runner    (1001) docker     (122)     1421 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)    14161 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/icheck.js
+-rw-r--r--   0 runner    (1001) docker     (122)     4516 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/icheck.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.516106 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/
+-rw-r--r--   0 runner    (1001) docker     (122)    21689 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/_all.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/aero.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/blue.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2244 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/green.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/grey.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2103 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/line.css
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/line.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/line@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2260 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/orange.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/pink.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/purple.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/red.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/yellow.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.524107 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/
+-rw-r--r--   0 runner    (1001) docker     (122)    14176 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/_all.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/aero.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/aero.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/aero@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/blue.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/blue.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/blue@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/green.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/green.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1408 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/green@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/grey.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1142 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/grey.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/grey@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/orange.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/orange.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/orange@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/pink.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/pink.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/pink@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/purple.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/purple.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/purple@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/red.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/red.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/red@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1406 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.528107 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/polaris/
+-rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris.css
+-rw-r--r--   0 runner    (1001) docker     (122)     6401 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris.png
+-rw-r--r--   0 runner    (1001) docker     (122)    16760 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.532106 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/
+-rw-r--r--   0 runner    (1001) docker     (122)    15591 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/_all.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/aero.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2167 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/aero.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/aero@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/blue.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2185 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/blue.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4485 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/blue@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/green.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/green.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4498 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/green@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/grey.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/grey.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4483 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/grey@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/orange.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/orange.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4474 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/orange@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/pink.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/pink.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4479 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/pink@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/purple.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2188 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/purple.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4501 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/purple@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1594 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/red.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2190 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/red.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4490 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/red@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1546 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/square.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2175 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/square.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/square@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/yellow.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/yellow.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4385 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/yellow@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.536107 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/
+-rw-r--r--   0 runner    (1001) docker     (122)    22814 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.date.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5315 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (122)    90539 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.js
+-rw-r--r--   0 runner    (1001) docker     (122)     9118 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.numeric.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.phone.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (122)     9392 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.regex.extensions.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.536107 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/phone-codes/
+-rw-r--r--   0 runner    (1001) docker     (122)     3631 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/phone-codes/phone-be.json
+-rw-r--r--   0 runner    (1001) docker     (122)    39492 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/phone-codes/phone-codes.json
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/phone-codes/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.540107 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/jQueryUI/
+-rw-r--r--   0 runner    (1001) docker     (122)   470596 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/jQueryUI/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (122)   240427 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/jQueryUI/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.540107 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/jvectormap/
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-1.2.2.css
+-rw-r--r--   0 runner    (1001) docker     (122)    33323 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)    95062 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-usa-en.js
+-rw-r--r--   0 runner    (1001) docker     (122)   144313 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-world-mill-en.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.540107 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/pace/
+-rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/pace/pace.css
+-rw-r--r--   0 runner    (1001) docker     (122)    26566 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/pace/pace.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/pace/pace.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)    12507 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/pace/pace.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.540107 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/
+-rw-r--r--   0 runner    (1001) docker     (122)    71385 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/bootstrap-slider.js
+-rw-r--r--   0 runner    (1001) docker     (122)    38635 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/bootstrap-slider.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.540107 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/
+-rw-r--r--   0 runner    (1001) docker     (122)    10368 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/bootstrap-slider.css
+-rw-r--r--   0 runner    (1001) docker     (122)     9336 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/bootstrap-slider.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.544107 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/timepicker/
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.css
+-rw-r--r--   0 runner    (1001) docker     (122)    34375 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)    18685 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.412106 django-adminlte-ui-2.1.0/adminlteui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.548107 django-adminlte-ui-2.1.0/adminlteui/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      300 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/404.html
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/500.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/actions.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.412106 django-adminlte-ui-2.1.0/adminlteui/templates/admin/auth/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.548107 django-adminlte-ui-2.1.0/adminlteui/templates/admin/auth/user/
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/auth/user/add_form.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5326 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/auth/user/change_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)    23633 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3325 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/base_site.html
+-rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5922 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/change_list_object_tools.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1897 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/change_list_results.html
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/date_hierarchy.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/delete_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/delete_selected_confirmation.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.548107 django-adminlte-ui-2.1.0/adminlteui/templates/admin/edit_inline/
+-rw-r--r--   0 runner    (1001) docker     (122)     2906 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/edit_inline/stacked.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5550 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/edit_inline/tabular.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1346 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/filter.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.548107 django-adminlte-ui-2.1.0/adminlteui/templates/admin/includes/
+-rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/includes/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/includes/object_delete_summary.html
+-rw-r--r--   0 runner    (1001) docker     (122)     7379 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/invalid_setup.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5090 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/login.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/object_history.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3829 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/search_form.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/admin/submit_line.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.548107 django-adminlte-ui-2.1.0/adminlteui/templates/adminlte/
+-rw-r--r--   0 runner    (1001) docker     (122)     4056 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/adminlte/date_range_filter.html
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/adminlte/form.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.548107 django-adminlte-ui-2.1.0/adminlteui/templates/adminlte/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/adminlte/widgets/select.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.552107 django-adminlte-ui-2.1.0/adminlteui/templates/registration/
+-rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/registration/logged_out.html
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/registration/password_change_done.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5828 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templates/registration/password_change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.552107 django-adminlte-ui-2.1.0/adminlteui/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templatetags/adminlte_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3297 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templatetags/adminlte_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/templatetags/adminlte_menu.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/adminlteui/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 09:46:13.552107 django-adminlte-ui-2.1.0/django_adminlte_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-07-04 09:46:13.000000 django-adminlte-ui-2.1.0/django_adminlte_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    32881 2023-07-04 09:46:13.000000 django-adminlte-ui-2.1.0/django_adminlte_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-04 09:46:13.000000 django-adminlte-ui-2.1.0/django_adminlte_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-04 09:46:13.000000 django-adminlte-ui-2.1.0/django_adminlte_ui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-04 09:46:13.000000 django-adminlte-ui-2.1.0/django_adminlte_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-04 09:46:13.552107 django-adminlte-ui-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      650 2023-07-04 09:46:00.000000 django-adminlte-ui-2.1.0/setup.py
```

### Comparing `django-adminlte-ui-2.0.0/LICENSE` & `django-adminlte-ui-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/PKG-INFO` & `django-adminlte-ui-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-adminlte-ui
-Version: 2.0.0
+Version: 2.1.0
 Summary: django admin theme base on adminlte
 Home-page: https://github.com/wuyue92tree/django-adminlte-ui
 Author: wuyue
 Author-email: wuyue92tree@163.com
 Maintainer: wuyue
 Maintainer-email: wuyue92tree@163.com
 License: MIT
```

### Comparing `django-adminlte-ui-2.0.0/README.md` & `django-adminlte-ui-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/admin.py` & `django-adminlte-ui-2.1.0/adminlteui/admin.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,18 +3,25 @@
 
 class ModelAdmin(admin.ModelAdmin):
     select2_list_filter = ()
     search_field_placeholder = ''
 
     class Media:
         css = {
-            "all": ("admin/components/select2/dist/css/select2.min.css",)
+            "all": (
+                "admin/components/select2/dist/css/select2.min.css",
+                # for daterangefilter
+                "admin/components/bootstrap-daterangepicker/daterangepicker.css"
+            )
         }
         js = (
             "admin/components/select2/dist/js/select2.min.js",
+            # for daterangefilter
+            "admin/components/moment/moment-with-locales.min.js",
+            "admin/components/bootstrap-daterangepicker/daterangepicker.js",
         )
 
     def changelist_view(self, request, extra_context=None):
         view = super().changelist_view(request, extra_context)
         if hasattr(view, 'context_data'):
             cl = view.context_data.get('cl', None)
             if cl:
```

### Comparing `django-adminlte-ui-2.0.0/adminlteui/core.py` & `django-adminlte-ui-2.1.0/adminlteui/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,39 +35,53 @@
                 return None
             model = models.get(self.label)
             if not self.name:
                 menu_item['name'] = model.get('name')
             menu_item['url'] = model.get('admin_url')
         elif self.menu_type == 'link':
             menu_item['url'] = self.url
+            # check permissions when permissions are not None
+            if self.permissions:
+                if request.user.has_perms(self.permissions) is False:
+                    return None
         else:
             # menu_type: group and child is empty will hide the menu
             if not self.child:
                 return None
 
         if menu_item.get('name') is None:
             # setup name as label when name is None
             menu_item['name'] = menu_item['label']
 
         menu_item['target_blank'] = self.target_blank
         menu_item['menu_type'] = self.menu_type or 'group'
 
+        if menu_item['menu_type'] != 'group':
+            if menu_item['url'] == request.path:
+                menu_item['active'] = True
+
         if self.child:
             if deep_limit == 0 or deep <= deep_limit:
                 child_list = []
+                has_child_active = False
                 for child in self.child:
                     deep += 1
                     child_menu = child.make(request, models, deep, deep_limit)
                     if child_menu:
                         # menu_type: group and child is empty will hide the menu
                         if child_menu.get('menu_type', 'group') == 'group':
                             if len(child_menu.get('child')) == 0:
                                 continue
+                        if child_menu.get('active') is True:
+                            has_child_active = True
+
                         child_list.append(child_menu)
                 menu_item['child'] = child_list
+                if has_child_active is True:
+                    menu_item['active'] = True
             else:
                 return None
         return menu_item
 
 
 class AdminlteConfig(object):
     main_menu = []
```

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/css/ionicons.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/Ionicons/css/ionicons.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/css/ionicons.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/Ionicons/css/ionicons.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.eot` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.eot`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.svg` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.svg`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.ttf` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.ttf`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.woff` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.woff`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.css.map` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.min.css.map` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.css.map` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.min.css.map` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.eot` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.svg` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.css.map` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css.map` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/alpha-horizontal.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/alpha-horizontal.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/saturation.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/saturation.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/bootstrap-colorpicker.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/bootstrap-colorpicker.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/bootstrap-colorpicker.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/bootstrap-colorpicker.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.css.map` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.css.map` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.css.map` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.css.map` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/bootstrap-datepicker.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/bootstrap-datepicker.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/bootstrap-datepicker.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker-en-CA.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker-en-CA.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ar-tn.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ar-tn.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ar.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ar.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.az.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.az.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bg.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bg.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bm.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bm.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bn.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bn.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ca.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ca.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.cs.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.cs.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.da.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.da.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.de.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.de.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.el.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.el.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-AU.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-AU.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-CA.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-CA.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-GB.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-GB.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-IE.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-IE.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-NZ.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-NZ.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-ZA.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-ZA.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.eo.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.eo.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.es.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.es.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.et.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.et.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.eu.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.eu.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fa.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fa.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fi.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fi.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fr-CH.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fr-CH.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fr.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fr.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.he.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.he.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hi.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hi.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hu.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hu.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hy.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hy.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.it.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.it.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ka.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ka.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kh.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kh.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kk.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kk.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.km.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.km.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ko.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ko.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kr.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kr.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.lt.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.lt.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.lv.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.lv.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.mk.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.mk.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.mn.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.mn.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.nl-BE.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.nl-BE.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.nl.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.nl.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.no.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.no.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.oc.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.oc.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.pl.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.pl.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.rs-latin.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.rs-latin.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.rs.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.rs.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ru.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ru.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.si.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.si.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sq.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sq.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sr.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sr.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ta.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ta.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tg.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tg.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.th.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.th.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tk.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tk.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uk.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uk.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uz-cyrl.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uz-cyrl.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uz-latn.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uz-latn.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.vi.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.vi.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.zh-CN.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.zh-CN.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.zh-TW.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.zh-TW.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-daterangepicker/daterangepicker.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-daterangepicker/daterangepicker.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-daterangepicker/daterangepicker.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/bootstrap-daterangepicker/daterangepicker.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/License.txt` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/external/sizzle/LICENSE.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,36 @@
-Copyright SpryMedia Limited and other contributors
-http://datatables.net
+Copyright JS Foundation and other contributors, https://js.foundation/
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+This software consists of voluntary contributions made by many
+individuals. For exact contribution history, see the revision history
+available at https://github.com/jquery/sizzle
+
+The following license applies to all parts of this software except as
+documented below:
+
+====
+
+Permission is hereby granted, free of charge, to any person obtaining
+a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to
+permit persons to whom the Software is furnished to do so, subject to
+the following conditions:
+
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
+WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+====
+
+All files located in the node_modules and external directories are
+externally maintained libraries used by this software which have their
+own licenses; we recommend you read them, as their terms may differ from
+the terms above.
```

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/fastclick/lib/fastclick.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/fastclick/lib/fastclick.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.css.map` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/FontAwesome.otf` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.eot` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.svg` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.ttf` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.woff` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.woff2` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/core.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/dist/core.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/dist/jquery.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.min.map` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/dist/jquery.min.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.min.map` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.min.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.map` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery-slimscroll/jquery.slimscroll.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery-slimscroll/jquery.slimscroll.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery-slimscroll/jquery.slimscroll.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/jquery-slimscroll/jquery.slimscroll.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/css/select2.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/css/select2.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/css/select2.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/af.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/af.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ar.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ar.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/az.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/az.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/bg.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/bn.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/bn.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/bs.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/bs.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ca.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/cs.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/da.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/da.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/de.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/de.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/dsb.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/dsb.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/el.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/el.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/en.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/en.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/es.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/es.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/et.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/et.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/eu.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/fa.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/fi.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/fr.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/gl.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/he.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/he.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hi.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hr.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hsb.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/hsb.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hu.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hy.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/hy.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/id.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/id.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/is.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/is.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/it.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/it.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ja.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ja.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ka.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ka.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/km.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/km.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ko.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/lt.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/lv.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/mk.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ms.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ms.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/nb.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ne.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ne.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/nl.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/pl.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ps.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ps.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/pt-BR.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/pt.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ro.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ru.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sk.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sl.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/sl.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sq.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/sq.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sr-Cyrl.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sr.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sv.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/th.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/th.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/tk.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/tk.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/tr.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/uk.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/vi.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/zh-CN.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/zh-TW.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/select2.full.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/select2.full.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/select2.full.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/select2.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/select2.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/select2.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/components/select2/dist/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/AdminLTE.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/AdminLTE.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/AdminLTE.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/AdminLTE.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/adminlte.css.map` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/adminlte.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/adminlte.min.css.map` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/adminlte.min.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-bootstrap-social.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/alt/AdminLTE-bootstrap-social.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-bootstrap-social.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/alt/AdminLTE-bootstrap-social.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-fullcalendar.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/alt/AdminLTE-fullcalendar.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-fullcalendar.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/alt/AdminLTE-fullcalendar.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-select2.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/alt/AdminLTE-select2.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-select2.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/alt/AdminLTE-select2.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-without-plugins.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/alt/AdminLTE-without-plugins.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-without-plugins.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/alt/AdminLTE-without-plugins.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/app.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/app.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/django.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/django.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/fontgoogle.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/fontgoogle.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/_all-skins.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/_all-skins.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/_all-skins.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/_all-skins.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-black-light.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-black-light.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-black-light.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-black-light.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-black.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-black.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-black.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-black.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-blue-light.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-blue-light.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-blue-light.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-blue-light.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-blue.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-blue.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-blue.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-blue.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-green-light.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-green-light.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-green-light.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-green-light.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-green.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-green.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-green.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-green.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-purple-light.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-purple-light.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-purple-light.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-purple-light.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-purple.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-purple.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-purple.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-purple.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-red-light.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-red-light.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-red-light.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-red-light.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-red.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-red.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-red.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-red.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-yellow-light.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-yellow-light.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-yellow-light.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-yellow-light.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-yellow.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-yellow.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-yellow.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/css/skins/skin-yellow.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/calendar-icons.svg` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/img/calendar-icons.svg`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/default-log.svg` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/img/default-log.svg`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/default.jpg` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/img/default.jpg`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/selector-icons.svg` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/img/selector-icons.svg`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/adminlte.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/js/adminlte.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/adminlte.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/js/adminlte.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/demo.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/js/demo.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/pages/dashboard.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/js/pages/dashboard.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/pages/dashboard2.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/dist/js/pages/dashboard2.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-slider/bootstrap-slider.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/bootstrap-slider/bootstrap-slider.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-slider/slider.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/bootstrap-slider/slider.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/all.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/all.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/_all.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/_all.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/aero.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/aero.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/aero.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/aero.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/aero@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/aero@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/blue.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/blue.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/blue.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/blue.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/blue@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/blue@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/flat.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/flat.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/flat.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/flat.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/flat@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/flat@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/green.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/green.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/green.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/green.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/green@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/green@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/grey.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/grey.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/grey.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/grey.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/grey@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/grey@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/orange.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/orange.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/orange.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/orange.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/orange@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/orange@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/pink.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/pink.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/pink.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/pink.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/pink@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/pink@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/purple.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/purple.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/purple.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/purple.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/purple@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/purple@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/red.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/red.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/red.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/red.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/red@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/red@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/yellow.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/yellow.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/yellow.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/yellow.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/yellow@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/flat/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/icheck.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/icheck.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/icheck.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/icheck.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/_all.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/_all.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/aero.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/aero.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/blue.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/blue.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/green.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/green.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/grey.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/grey.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/line.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/line.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/line.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/line.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/line@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/line@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/orange.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/orange.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/pink.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/pink.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/purple.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/purple.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/red.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/red.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/yellow.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/line/yellow.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/_all.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/_all.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/aero.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/aero.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/aero.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/aero.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/aero@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/aero@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/blue.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/blue.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/blue.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/blue.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/blue@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/blue@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/green.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/green.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/green.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/green.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/green@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/green@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/grey.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/grey.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/grey.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/grey.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/grey@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/grey@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/orange.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/orange.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/orange.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/orange.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/orange@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/orange@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/pink.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/pink.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/pink.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/pink.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/pink@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/pink@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/purple.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/purple.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/purple.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/purple.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/purple@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/purple@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/red.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/red.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/red.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/red.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/red@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/red@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/_all.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/_all.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/aero.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/aero.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/aero.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/aero.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/aero@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/aero@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/blue.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/blue.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/blue.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/blue.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/blue@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/blue@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/green.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/green.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/green.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/green.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/green@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/green@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/grey.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/grey.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/grey.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/grey.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/grey@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/grey@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/orange.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/orange.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/orange.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/orange.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/orange@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/orange@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/pink.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/pink.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/pink.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/pink.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/pink@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/pink@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/purple.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/purple.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/purple.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/purple.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/purple@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/purple@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/red.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/red.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/red.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/red.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/red@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/red@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/square.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/square.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/square.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/square.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/square@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/square@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/yellow.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/yellow.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/yellow.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/yellow.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/yellow@2x.png` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/iCheck/square/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.date.extensions.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.date.extensions.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.extensions.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.extensions.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.numeric.extensions.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.numeric.extensions.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.phone.extensions.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.phone.extensions.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.regex.extensions.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.regex.extensions.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/phone-codes/phone-be.json` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/phone-codes/phone-be.json`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/phone-codes/phone-codes.json` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/input-mask/phone-codes/phone-codes.json`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jQueryUI/jquery-ui.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/jQueryUI/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jQueryUI/jquery-ui.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/jQueryUI/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-1.2.2.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-1.2.2.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-usa-en.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-usa-en.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-world-mill-en.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-world-mill-en.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/pace.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/pace/pace.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/pace.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/pace/pace.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/pace.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/pace/pace.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/pace.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/pace/pace.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/bootstrap-slider.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/bootstrap-slider.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/bootstrap-slider.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/bootstrap-slider.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/bootstrap-slider.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/bootstrap-slider.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/bootstrap-slider.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/bootstrap-slider.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.min.css` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.min.js` & `django-adminlte-ui-2.1.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/500.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/500.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/actions.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/actions.html`

 * *Files 7% similar despite different names*

```diff
@@ -20,9 +20,12 @@
             <span class="clear" style="display: none;"><a href="#">{% trans "Clear selection" %}</a></span>
             {% endif %}
             {% endif %}
             {% endblock %}
             {% endblock %}
         </div>
     </div>
-    <script>document.querySelector('.actions select').setAttribute('class', 'form-control')</script>
+    <script>
+        document.querySelector('.actions select').setAttribute('class', 'form-control');
+        document.querySelector('.actions select').style.minWidth='200px';
+    </script>
 </div>
```

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/auth/user/change_password.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/base.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/base.html`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,29 @@
     <!-- Font Awesome -->
     <link rel="stylesheet" href={% static "admin/components/font-awesome/css/font-awesome.min.css" %}>
     <!-- Ionicons -->
     <link rel="stylesheet" href={% static "admin/components/Ionicons/css/ionicons.min.css" %}>
 
     {% block extrastyle %} {% endblock %}
 
+    <!-- jQuery -->
+    <script src={% static "admin/components/jquery/dist/jquery.min.js" %}></script>
+    <!-- jQuery UI -->
+    <script src={% static "admin/plugins/jQueryUI/jquery-ui.min.js" %}></script>
+    <!-- Resolve conflict in jQuery UI tooltip with Bootstrap tooltip -->
+    <script>
+        $.widget.bridge('uibutton', $.ui.button);
+    </script>
+    <!-- Bootstrap -->
+    <script src={% static "admin/components/bootstrap/dist/js/bootstrap.min.js" %}></script>
+    <!-- Slimscroll -->
+    <script src={% static "admin/components/jquery-slimscroll/jquery.slimscroll.min.js" %}></script>
+    <!-- FastClick -->
+    <script src={% static "admin/components/fastclick/lib/fastclick.js" %}></script>
+
     {% block extrahead %} {% endblock %}
     <!-- Theme style -->
     <link rel="stylesheet" href={% static "admin/dist/css/AdminLTE.min.css" %}>
     <!-- AdminLTE Skins. Choose a skin from the css/skins
          folder instead of downloading all of them to reduce the load. -->
     {% if adminlte.skin %}
         <link rel="stylesheet" href={% static "admin/dist/css/skins/skin-"|add:adminlte.skin|add:".min.css" %}>
@@ -416,84 +431,20 @@
         <!-- Add the sidebar's background. This div must be placed
              immediately after the control sidebar -->
         <div class="control-sidebar-bg"></div>
     {% endif %}
 </div>
 <!-- ./wrapper -->
 
-<!-- jQuery -->
-<script src={% static "admin/components/jquery/dist/jquery.min.js" %}></script>
-<!-- jQuery UI -->
-<script src={% static "admin/plugins/jQueryUI/jquery-ui.min.js" %}></script>
-<!-- Resolve conflict in jQuery UI tooltip with Bootstrap tooltip -->
-<script>
-    $.widget.bridge('uibutton', $.ui.button);
-</script>
-<!-- Bootstrap -->
-<script src={% static "admin/components/bootstrap/dist/js/bootstrap.min.js" %}></script>
-<!-- Slimscroll -->
-<script src={% static "admin/components/jquery-slimscroll/jquery.slimscroll.min.js" %}></script>
-<!-- FastClick -->
-<script src={% static "admin/components/fastclick/lib/fastclick.js" %}></script>
 <!-- AdminLTE App -->
 <script src={% static "admin/dist/js/adminlte.min.js" %}></script>
 <!-- AdminLTE for demo purposes -->
 {% if adminlte.demo %}
     <script src={% static "admin/dist/js/demo.js" %}></script>
 {% endif %}
-<script>
-    // use js control active status of siderbar-menu
-    $(function() {
-        var menuActions = document.querySelectorAll('.sidebar-menu a')
-        var pathname = document.querySelector('#adminIndex').pathname
-        for (var i in menuActions) {
-            try {
-                if (window.location.pathname === pathname) {
-                    menuActions[i].parentNode.setAttribute('class', 'active')
-                    break
-                }
-
-                if (window.location.href.indexOf(menuActions[i].href) !== -1) {
-                    if (menuActions[i].href===window.location.origin + pathname) {
-                        continue
-                    }
-                    console.log('menu matched.', window.location.href, menuActions[i].href);
-                    menuActions[i].parentNode.setAttribute('class', 'active');
-
-                    let parent = menuActions[i].parentNode;
-                    while (true) {
-                        if (parent.parentNode.getAttribute('class') !== 'sidebar-menu tree') {
-                            if (parent.parentNode.getAttribute('class').indexOf('treeview-menu') !== -1) {
-                                parent.parentNode.setAttribute('class', 'treeview-menu menu-open');
-                                parent.parentNode.parentNode.setAttribute('class', 'treeview active');
-                            }
-                            parent = parent.parentNode;
-                        } else {
-                            break
-                        }
-                    }
-                    break
-                }
-            } catch (e) {
-                console.log(window.location.href, menuActions[i].href, e)
-            }
-        }
-
-        var topMenuActions = document.querySelectorAll('.top-menu a')
-        for (var j in topMenuActions) {
-            if (window.location.href.indexOf(topMenuActions[j].href) !== -1) {
-                topMenuActions[j].parentNode.setAttribute('class', 'active');
-                if (topMenuActions[j].parentNode.parentNode.getAttribute('class') === 'dropdown-menu') {
-                    topMenuActions[j].parentNode.parentNode.parentNode.setAttribute('class', 'dropdown active');
-                }
-                console.log('top menu matched.', window.location.href, topMenuActions[j].href);
-            }
-        }
-    })
-</script>
 
 <script>
     // sidebar push menu control
     $(function () {
         $("body")
             .on("expanded.pushMenu", function() {
                 localStorage.setItem('sidebarStatus', 'expanded')
```

#### html2text {}

```diff
@@ -4,15 +4,25 @@
  }}" {% if LANGUAGE_BIDI %}dir="rtl"{% endif %}>
 
 
 
 admin/components/bootstrap/dist/css/bootstrap.min.css" %}>
 admin/components/font-awesome/css/font-awesome.min.css" %}>
 admin/components/Ionicons/css/ionicons.min.css" %}> {% block extrastyle %} {%
-endblock %} {% block extrahead %} {% endblock %}
+endblock %}
+admin/components/jquery/dist/jquery.min.js" %}>
+
+admin/plugins/jQueryUI/jquery-ui.min.js" %}>
+
+admin/components/bootstrap/dist/js/bootstrap.min.js" %}>
+
+admin/components/jquery-slimscroll/jquery.slimscroll.min.js" %}>
+
+admin/components/fastclick/lib/fastclick.js" %}>
+{% block extrahead %} {% endblock %}
 admin/dist/css/AdminLTE.min.css" %}>  {% if adminlte.skin %}
 admin/dist/css/skins/skin-"|add:adminlte.skin|add:".min.css" %}> {% else %}
 admin/dist/css/skins/_all-skins.min.css" %}> {% endif %}
 admin/dist/css/django.css" %}> {% if adminlte.site_logo %}
 
  {% else %}
 ist/img/default-log.svg" %}">
@@ -96,22 +106,12 @@
 **** Chat Settings ****
  Show me as online *
  Turn off notifications ⁰
  Delete chat history
 
 {% endif %}
 
-admin/components/jquery/dist/jquery.min.js" %}>
-
-admin/plugins/jQueryUI/jquery-ui.min.js" %}>
-
-admin/components/bootstrap/dist/js/bootstrap.min.js" %}>
-
-admin/components/jquery-slimscroll/jquery.slimscroll.min.js" %}>
-
-admin/components/fastclick/lib/fastclick.js" %}>
-
 admin/dist/js/adminlte.min.js" %}>
  {% if adminlte.demo %}
 admin/dist/js/demo.js" %}>
 {% endif %}
  {% block extrajs %}{% endblock %}
```

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/base_site.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/change_form.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/change_list.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/change_list.html`

 * *Files 9% similar despite different names*

```diff
@@ -55,40 +55,43 @@
                         {% if cl.formset.total_error_count == 1 %}{% trans "Please correct the error below." %}{% else %}{% trans "Please correct the errors below." %}{% endif %}
                     </p>
                     {{ cl.formset.non_form_errors }}
                     {% endif %}
                     <div class="module{% if cl.has_filters %} filtered{% endif %}" id="changelist">
                         <div class="row" style="margin-bottom: 15px;">
                             {% block search %}
-                            <div class="col-md-10 col-sm-12 col-xs-12" id="toolbar">
+                            <div class="col-sm-12 col-xs-12" id="toolbar">
                                 {% search_form cl %}
                             </div>
                             {% endblock %}
-
-                            {% block object-tools %}
-                            <div {% if cl.has_filters or cl.search_fields %}class="col-md-2 col-sm-12 col-xs-12 text-right"{% else %}class="col-md-12 text-right"{% endif %}>
-                                {% block object-tools-items %}
-                                {% change_list_object_tools %}
-                                {% endblock %}
-                            </div>
-                            {% endblock %}
                         </div>
 
                         <div class="row">
                             {% block date_hierarchy %}{% if cl.date_hierarchy %}{% date_hierarchy cl %}{% endif %}{% endblock %}
                         </div>
 
                         <form id="changelist-form" method="post"{% if cl.formset and cl.formset.is_multipart %} enctype="multipart/form-data"{% endif %} novalidate>{% csrf_token %}
                             <div class="dataTables_wrapper form-inline dt-bootstrap">
                             {% if cl.formset %}
                             <div>{{ cl.formset.management_form }}</div>
                             {% endif %}
 
                             {% block result_list %}
-                            {% if action_form and actions_on_top and cl.show_admin_actions %}{% admin_actions %}{% endif %}
+                            <div class="row">
+                                {% if action_form and actions_on_top and cl.show_admin_actions %}
+                                    <div class="col-md-6">{% admin_actions %}</div>
+                                {% endif %}
+                                {% block object-tools %}
+                                    <div {% if action_form and actions_on_top and cl.show_admin_actions %}class="col-md-6 text-right"{% else %}class="col-md-12 text-right"{%endif%}>
+                                        {% block object-tools-items %}
+                                            {% change_list_object_tools %}
+                                        {% endblock %}
+                                    </div>
+                                {% endblock %}
+                            </div>
                             {% result_list cl %}
                             {% if action_form and actions_on_bottom and cl.show_admin_actions %}{% admin_actions %}{% endif %}
                             {% endblock %}
                             {% block pagination %}{% pagination cl %}{% endblock %}
                             </div>
                         </form>
                     </div>
```

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/change_list_results.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/date_hierarchy.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/date_hierarchy.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/delete_confirmation.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/delete_selected_confirmation.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/edit_inline/stacked.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/edit_inline/tabular.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/filter.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/filter.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 {% load i18n %}
 
 <div class="form-group" style="margin-bottom: 5px;">
-    <select id="id_filter_{{ field_name }}" class="form-control search-filter" style="width: 100%;" tabindex="-1" aria-hidden="true">
+    <select id="id_filter_{{ field_name }}" class="form-control search-filter" style="width: 100%; min-width: 200px;" tabindex="-1" aria-hidden="true">
         <option value="">{{ title }}</option>
         <option value="">---------</option>
         {% for choice in choices %}
             {% if choice.name %}
                 <option data-name="{{ choice.name }}" value="{{ choice.value }}" {% if choice.selected %} selected {% endif %}>
                     {{ choice.display }}
                 </option>
             {% endif %}
         {% endfor %}
     </select>
     {% if spec.display_select2 %}
     <script>
         django.jQuery('#id_filter_{{ field_name }}').select2({
-            width: django.jQuery('#id_filter_{{ field_name }}').width() + 26
+            dropdownAutoWidth : true,
+            width: '100%'
         })
+        django.jQuery('#id_filter_{{ field_name }}').parent().find('span.select2-container').css({'min-width': '200px'})
         django.jQuery('#id_filter_{{ field_name }}').on('select2:select', function (e) {
             if (e.params.data.id !=='') {
                 django.jQuery('#id_filter_{{ field_name }}').attr('name', e.params.data.element.dataset.name)
             } else {
                 django.jQuery('#id_filter_{{ field_name }}').removeAttr('name')
             }
         });
```

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/includes/fieldset.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/index.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/invalid_setup.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/invalid_setup.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/login.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/object_history.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/pagination.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/search_form.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/admin/submit_line.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/adminlte/form.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/adminlte/form.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/registration/logged_out.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/registration/password_change_done.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templates/registration/password_change_form.html` & `django-adminlte-ui-2.1.0/adminlteui/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templatetags/adminlte_core.py` & `django-adminlte-ui-2.1.0/adminlteui/templatetags/adminlte_core.py`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templatetags/adminlte_list.py` & `django-adminlte-ui-2.1.0/adminlteui/templatetags/adminlte_list.py`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/adminlteui/templatetags/adminlte_menu.py` & `django-adminlte-ui-2.1.0/adminlteui/templatetags/adminlte_menu.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,30 +26,37 @@
 def render_main_menu(menu):
     if not menu:
         return ''
     html = ''
     for menu_item in menu:
         child = menu_item.get('child', [])
         if child:
+            if menu_item.get('active') is True:
+                treeview_class = 'treeview active menu-open'
+                treeview_menu_class = 'treeview-menu menu-open'
+            else:
+                treeview_class = 'treeview'
+                treeview_menu_class = 'treeview-menu'
             menu_item_html = f'''
-            <li class="treeview">
+            <li class="{treeview_class}">
                 <a href="javascript:void(0)">
                     <i class="fa {menu_item.get('icon')}"></i>
                     <span style="overflow: hidden; display: inline-block; vertical-align:top;">{menu_item.get('name')}</span>
                     <span class="pull-right-container"><i class="fa fa-angle-left pull-right"></i></span>
                 </a>
-                <ul class="treeview-menu">
+                <ul class="{treeview_menu_class}">
                     {render_main_menu(child)}
                 </ul>
             </li>
             '''
         else:
             target_blank = '' if menu_item.get('target_blank') is False else 'target="_blank"'
+            flag = 'active' if menu_item.get('active') is True else ''
             menu_item_html = f'''
-            <li><a {target_blank} href="{menu_item.get('url')}"><i class="fa {menu_item.get('icon')}"></i><span> {menu_item.get('name')}</span></a></li>
+            <li class="{flag}"><a {target_blank} href="{menu_item.get('url')}"><i class="fa {menu_item.get('icon')}"></i><span> {menu_item.get('name')}</span></a></li>
             '''
         html += menu_item_html
     return html
 
 
 def render_top_menu(menu):
     """
@@ -60,28 +67,30 @@
     """
     if not menu:
         return ''
     html = ''
     for menu_item in menu:
         child = menu_item.get('child', [])
         if child:
+            flag = 'active' if menu_item.get('active') is True else ''
             menu_item_html = f'''
-            <li class="dropdown">
+            <li class="dropdown {flag}">
                 <a href="javascript:void(0)" class="dropdown-toggle" data-toggle="dropdown">
                     {menu_item.get('name')} <span class="caret"></span>
                 </a>
                 <ul class="dropdown-menu" role="menu" style="left: 0;">
                     {render_top_menu(child)}
                 </ul>
             </li>
             '''
         else:
             target_blank = '' if menu_item.get('target_blank') is False else 'target="_blank"'
+            flag = 'active' if menu_item.get('active') is True else ''
             menu_item_html = f'''
-            <li><a {target_blank} href="{menu_item.get('url')}"> {menu_item.get('name')}</a></li>
+            <li class="{flag}"><a {target_blank} href="{menu_item.get('url')}"> {menu_item.get('name')}</a></li>
             '''
         html += menu_item_html
     return html
 
 
 @simple_tag(takes_context=True)
 def get_menu(context, request, position: Literal['main', 'top'] = 'main'):
```

### Comparing `django-adminlte-ui-2.0.0/adminlteui/widgets.py` & `django-adminlte-ui-2.1.0/adminlteui/widgets.py`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-2.0.0/django_adminlte_ui.egg-info/PKG-INFO` & `django-adminlte-ui-2.1.0/django_adminlte_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-adminlte-ui
-Version: 2.0.0
+Version: 2.1.0
 Summary: django admin theme base on adminlte
 Home-page: https://github.com/wuyue92tree/django-adminlte-ui
 Author: wuyue
 Author-email: wuyue92tree@163.com
 Maintainer: wuyue
 Maintainer-email: wuyue92tree@163.com
 License: MIT
```

### Comparing `django-adminlte-ui-2.0.0/django_adminlte_ui.egg-info/SOURCES.txt` & `django-adminlte-ui-2.1.0/django_adminlte_ui.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 README.md
 README.rst
 setup.py
 adminlteui/__init__.py
 adminlteui/admin.py
 adminlteui/apps.py
 adminlteui/core.py
+adminlteui/filters.py
 adminlteui/models.py
 adminlteui/tests.py
 adminlteui/views.py
 adminlteui/widgets.py
 adminlteui/__pycache__/__init__.cpython-39.pyc
-adminlteui/locale/zh-Hans/LC_MESSAGES/django.mo
-adminlteui/locale/zh-Hans/LC_MESSAGES/django.po
 adminlteui/locale/zh/LC_MESSAGES/django.mo
 adminlteui/locale/zh/LC_MESSAGES/django.po
+adminlteui/locale/zh_Hans/LC_MESSAGES/django.mo
+adminlteui/locale/zh_Hans/LC_MESSAGES/django.po
 adminlteui/migrations/__init__.py
 adminlteui/static/admin/components/Ionicons/css/ionicons.css
 adminlteui/static/admin/components/Ionicons/css/ionicons.min.css
 adminlteui/static/admin/components/Ionicons/fonts/ionicons.eot
 adminlteui/static/admin/components/Ionicons/fonts/ionicons.svg
 adminlteui/static/admin/components/Ionicons/fonts/ionicons.ttf
 adminlteui/static/admin/components/Ionicons/fonts/ionicons.woff
@@ -145,22 +146,14 @@
 adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.svg
 adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf
 adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff
 adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2
 adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.js
 adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.min.js
 adminlteui/static/admin/components/bootstrap/dist/js/npm.js
-adminlteui/static/admin/components/datatables.net/.bower.json
-adminlteui/static/admin/components/datatables.net/License.txt
-adminlteui/static/admin/components/datatables.net/Readme.md
-adminlteui/static/admin/components/datatables.net/bower.json
-adminlteui/static/admin/components/datatables.net-bs/.bower.json
-adminlteui/static/admin/components/datatables.net-bs/License.txt
-adminlteui/static/admin/components/datatables.net-bs/Readme.md
-adminlteui/static/admin/components/datatables.net-bs/bower.json
 adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.css
 adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.min.css
 adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.js
 adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.min.js
 adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.js
 adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.min.js
 adminlteui/static/admin/components/fastclick/lib/fastclick.js
@@ -182,14 +175,16 @@
 adminlteui/static/admin/components/jquery/dist/jquery.slim.js
 adminlteui/static/admin/components/jquery/dist/jquery.slim.min.js
 adminlteui/static/admin/components/jquery/dist/jquery.slim.min.map
 adminlteui/static/admin/components/jquery/external/sizzle/LICENSE.txt
 adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.js
 adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.js
 adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.map
+adminlteui/static/admin/components/moment/moment-with-locales.js
+adminlteui/static/admin/components/moment/moment-with-locales.min.js
 adminlteui/static/admin/components/select2/dist/css/select2.css
 adminlteui/static/admin/components/select2/dist/css/select2.min.css
 adminlteui/static/admin/components/select2/dist/js/select2.full.js
 adminlteui/static/admin/components/select2/dist/js/select2.full.min.js
 adminlteui/static/admin/components/select2/dist/js/select2.js
 adminlteui/static/admin/components/select2/dist/js/select2.min.js
 adminlteui/static/admin/components/select2/dist/js/i18n/af.js
@@ -471,14 +466,15 @@
 adminlteui/templates/admin/submit_line.html
 adminlteui/templates/admin/auth/user/add_form.html
 adminlteui/templates/admin/auth/user/change_password.html
 adminlteui/templates/admin/edit_inline/stacked.html
 adminlteui/templates/admin/edit_inline/tabular.html
 adminlteui/templates/admin/includes/fieldset.html
 adminlteui/templates/admin/includes/object_delete_summary.html
+adminlteui/templates/adminlte/date_range_filter.html
 adminlteui/templates/adminlte/form.html
 adminlteui/templates/adminlte/widgets/select.html
 adminlteui/templates/registration/logged_out.html
 adminlteui/templates/registration/password_change_done.html
 adminlteui/templates/registration/password_change_form.html
 adminlteui/templatetags/__init__.py
 adminlteui/templatetags/adminlte_core.py
```

### Comparing `django-adminlte-ui-2.0.0/setup.py` & `django-adminlte-ui-2.1.0/setup.py`

 * *Files identical despite different names*

