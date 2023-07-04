# Comparing `tmp/meringue-0.4.0.post1.tar.gz` & `tmp/meringue-1.0.0.tar.gz`

## Comparing `meringue-0.4.0.post1.tar` & `meringue-1.0.0.tar`

### file list

```diff
@@ -1,50 +1,24 @@
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/__init__.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/fields.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/forms.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/middleware.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/widgets.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/admin/__init__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/admin/apps.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/admin/static/css/inline-gallery.css
--rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/admin/static/images/noise.png
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/admin/static/images/none.gif
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/admin/templates/admin/filter.html
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/conf/__init__.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/conf/default_settings.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/__init__.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/apps.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/decorators.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/errors.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/managers.py
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/models.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/options.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/query.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/translation.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/upload_handlers.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/views.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/static/css/inline-gallery.css
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/static/css/reset.css
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/static/css/reset.min.css
--rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/static/images/noise.png
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/static/images/none.gif
--rw-r--r--   0        0        0    83615 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/static/js/jquery-2.1.0.min.js
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/templates/404.html
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/templates/500.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/templates/robots.txt
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/templates/meringue/edit_inline/gallery.html
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/templates/rest_framework/base.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/templatetags/__init__.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/templatetags/meringue_base.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/templatetags/meringue_thumbnails.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/utils/__init__.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/utils/paginator.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/utils/unify.py
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/utils/thumbnails/__init__.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/utils/thumbnails/methods.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/utils/thumbnails/properties.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/AUTHORS
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/LICENSE
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/README.md
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/pyproject.toml
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/PKG-INFO
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/__init__.py
+-rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/conf/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/conf/default_settings.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/apps.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/managers.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/options.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/query.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/translation.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/upload_handlers.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/views.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/templatetags/__init__.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/templatetags/meringue_base.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/utils/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/utils/datetime.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.0.0/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-1.0.0/AUTHORS
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.0.0/LICENSE
+-rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 meringue-1.0.0/README.md
+-rw-r--r--   0        0        0     7990 2020-02-02 00:00:00.000000 meringue-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 meringue-1.0.0/PKG-INFO
```

### Comparing `meringue-0.4.0.post1/LICENSE` & `meringue-1.0.0/LICENSE`

 * *Files identical despite different names*

