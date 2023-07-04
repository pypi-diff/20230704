# Comparing `tmp/django-content-blocks-1.3.5.tar.gz` & `tmp/django-content-blocks-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-content-blocks-1.3.5.tar", last modified: Thu Jun 15 12:59:12 2023, max compression
+gzip compressed data, was "django-content-blocks-1.3.6.tar", last modified: Tue Jul  4 10:59:24 2023, max compression
```

## Comparing `django-content-blocks-1.3.5.tar` & `django-content-blocks-1.3.6.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.728030 django-content-blocks-1.3.5/
--rw-r--r--   0 quantra    (501) staff       (20)     1076 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/LICENSE
--rw-r--r--   0 quantra    (501) staff       (20)      147 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/MANIFEST.in
--rw-r--r--   0 quantra    (501) staff       (20)     7611 2023-06-15 12:59:12.728117 django-content-blocks-1.3.5/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)     6072 2023-06-10 15:19:48.000000 django-content-blocks-1.3.5/README.rst
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.697072 django-content-blocks-1.3.5/content_blocks/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.5/content_blocks/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)      850 2023-05-23 18:04:22.000000 django-content-blocks-1.3.5/content_blocks/abstract_models.py
--rw-r--r--   0 quantra    (501) staff       (20)    11969 2023-06-06 15:28:11.000000 django-content-blocks-1.3.5/content_blocks/admin.py
--rw-r--r--   0 quantra    (501) staff       (20)     5301 2023-06-06 15:28:11.000000 django-content-blocks-1.3.5/content_blocks/admin_forms.py
--rw-r--r--   0 quantra    (501) staff       (20)      952 2023-06-04 20:53:17.000000 django-content-blocks-1.3.5/content_blocks/apps.py
--rw-r--r--   0 quantra    (501) staff       (20)     1591 2023-06-03 20:41:24.000000 django-content-blocks-1.3.5/content_blocks/conf.py
--rw-r--r--   0 quantra    (501) staff       (20)     1685 2023-05-03 13:23:45.000000 django-content-blocks-1.3.5/content_blocks/fields.py
--rw-r--r--   0 quantra    (501) staff       (20)     8031 2023-05-24 23:15:33.000000 django-content-blocks-1.3.5/content_blocks/forms.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.697524 django-content-blocks-1.3.5/content_blocks/management/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2022-09-05 20:58:44.000000 django-content-blocks-1.3.5/content_blocks/management/__init__.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.698851 django-content-blocks-1.3.5/content_blocks/management/commands/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2022-09-05 20:59:01.000000 django-content-blocks-1.3.5/content_blocks/management/commands/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)      420 2023-05-23 18:04:22.000000 django-content-blocks-1.3.5/content_blocks/management/commands/clear_content_blocks_cache.py
--rw-r--r--   0 quantra    (501) staff       (20)      542 2023-05-23 18:04:22.000000 django-content-blocks-1.3.5/content_blocks/management/commands/export_content_block_templates.py
--rw-r--r--   0 quantra    (501) staff       (20)     1461 2023-05-24 11:55:23.000000 django-content-blocks-1.3.5/content_blocks/management/commands/import_content_block_templates.py
--rw-r--r--   0 quantra    (501) staff       (20)      415 2023-05-23 18:04:22.000000 django-content-blocks-1.3.5/content_blocks/management/commands/set_content_blocks_cache.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.699918 django-content-blocks-1.3.5/content_blocks/migrations/
--rw-r--r--   0 quantra    (501) staff       (20)    12063 2023-03-17 11:59:08.000000 django-content-blocks-1.3.5/content_blocks/migrations/0001_initial.py
--rw-r--r--   0 quantra    (501) staff       (20)     1784 2023-04-14 09:38:36.000000 django-content-blocks-1.3.5/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py
--rw-r--r--   0 quantra    (501) staff       (20)     1154 2023-05-01 12:02:10.000000 django-content-blocks-1.3.5/content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py
--rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.5/content_blocks/migrations/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)    23959 2023-06-15 12:30:46.000000 django-content-blocks-1.3.5/content_blocks/models.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.700942 django-content-blocks-1.3.5/content_blocks/services/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-05-23 18:56:52.000000 django-content-blocks-1.3.5/content_blocks/services/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)    12089 2023-06-15 12:57:28.000000 django-content-blocks-1.3.5/content_blocks/services/content_block.py
--rw-r--r--   0 quantra    (501) staff       (20)     1141 2023-05-23 18:04:22.000000 django-content-blocks-1.3.5/content_blocks/services/content_block_parent.py
--rw-r--r--   0 quantra    (501) staff       (20)     5283 2023-05-24 11:55:40.000000 django-content-blocks-1.3.5/content_blocks/services/content_block_template.py
--rw-r--r--   0 quantra    (501) staff       (20)     3312 2023-06-04 21:01:31.000000 django-content-blocks-1.3.5/content_blocks/signals.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.679715 django-content-blocks-1.3.5/content_blocks/static/
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.701292 django-content-blocks-1.3.5/content_blocks/static/content_blocks/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-28 23:45:54.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/.DS_Store
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.702820 django-content-blocks-1.3.5/content_blocks/static/content_blocks/css/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2022-12-22 00:43:03.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/css/.DS_Store
--rw-r--r--   0 quantra    (501) staff       (20)     1114 2023-06-06 15:28:11.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/css/content_block_template_admin.css
--rw-r--r--   0 quantra    (501) staff       (20)    10043 2023-06-14 16:14:32.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/css/content_blocks.css
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.680400 django-content-blocks-1.3.5/content_blocks/static/content_blocks/fontawesome/
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.704969 django-content-blocks-1.3.5/content_blocks/static/content_blocks/fontawesome/css/
--rw-r--r--   0 quantra    (501) staff       (20)    95481 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css
--rw-r--r--   0 quantra    (501) staff       (20)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/fontawesome/css/light.min.css
--rw-r--r--   0 quantra    (501) staff       (20)      747 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css
--rw-r--r--   0 quantra    (501) staff       (20)      573 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/fontawesome/css/solid.min.css
--rw-r--r--   0 quantra    (501) staff       (20)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/fontawesome/css/thin.min.css
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.706586 django-content-blocks-1.3.5/content_blocks/static/content_blocks/fontawesome/webfonts/
--rw-r--r--   0 quantra    (501) staff       (20)   394832 2023-05-02 13:45:50.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 quantra    (501) staff       (20)   149908 2023-05-02 13:45:50.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.707770 django-content-blocks-1.3.5/content_blocks/static/content_blocks/iframeresizer/
--rw-r--r--   0 quantra    (501) staff       (20)    34811 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js
--rw-r--r--   0 quantra    (501) staff       (20)    37781 2023-05-02 13:45:50.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.708442 django-content-blocks-1.3.5/content_blocks/static/content_blocks/jqueryform/
--rw-r--r--   0 quantra    (501) staff       (20)    17094 2023-05-02 13:45:50.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js
--rw-r--r--   0 quantra    (501) staff       (20)    22565 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.709052 django-content-blocks-1.3.5/content_blocks/static/content_blocks/jqueryui/
--rw-r--r--   0 quantra    (501) staff       (20)    30802 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css
--rw-r--r--   0 quantra    (501) staff       (20)   255080 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.712994 django-content-blocks-1.3.5/content_blocks/static/content_blocks/js/
--rw-r--r--   0 quantra    (501) staff       (20)     1894 2023-06-14 16:14:32.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/js/admin_choices_widget.js
--rw-r--r--   0 quantra    (501) staff       (20)      980 2023-06-14 16:14:32.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/js/ajax_setup.js
--rw-r--r--   0 quantra    (501) staff       (20)    19428 2023-06-14 16:14:32.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/js/content_block_editor.js
--rw-r--r--   0 quantra    (501) staff       (20)     2015 2023-06-14 16:14:32.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/js/content_block_template_admin.js
--rw-r--r--   0 quantra    (501) staff       (20)     2201 2023-06-14 16:14:32.000000 django-content-blocks-1.3.5/content_blocks/static/content_blocks/js/popup.js
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.714442 django-content-blocks-1.3.5/content_blocks/templates/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-03-16 15:09:32.000000 django-content-blocks-1.3.5/content_blocks/templates/.DS_Store
--rw-r--r--   0 quantra    (501) staff       (20)      137 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/templates/base.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.716092 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-07 23:05:50.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/.DS_Store
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.717107 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/admin/
--rw-r--r--   0 quantra    (501) staff       (20)      317 2023-06-04 15:21:52.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/admin/content_block_template_change_list.html
--rw-r--r--   0 quantra    (501) staff       (20)      197 2023-06-06 15:28:11.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/admin/content_block_template_field_delete_checkbox.html
--rw-r--r--   0 quantra    (501) staff       (20)     1366 2023-05-03 12:36:26.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/admin/content_block_template_import_form.html
--rw-r--r--   0 quantra    (501) staff       (20)      305 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/content_block_collection.html
--rw-r--r--   0 quantra    (501) staff       (20)      494 2023-05-23 18:04:22.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/content_block_preview.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.718477 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/editor/
--rw-r--r--   0 quantra    (501) staff       (20)     1997 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/editor/base.html
--rw-r--r--   0 quantra    (501) staff       (20)     2656 2023-06-14 16:14:32.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/editor/content_block_form.html
--rw-r--r--   0 quantra    (501) staff       (20)     4886 2023-06-14 16:14:32.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html
--rw-r--r--   0 quantra    (501) staff       (20)      439 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/editor/content_block_forms.html
--rw-r--r--   0 quantra    (501) staff       (20)     4886 2023-06-14 16:14:32.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/editor/editor.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.719477 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/partials/
--rw-r--r--   0 quantra    (501) staff       (20)      187 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/partials/delete_popup.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.720033 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/partials/fields/
--rw-r--r--   0 quantra    (501) staff       (20)      149 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/partials/fields/checkbox.html
--rw-r--r--   0 quantra    (501) staff       (20)      497 2023-06-14 16:14:32.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/partials/fields/default.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.721218 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/partials/fields/previews/
--rw-r--r--   0 quantra    (501) staff       (20)      144 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/partials/fields/previews/base.html
--rw-r--r--   0 quantra    (501) staff       (20)      464 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/partials/fields/previews/embedded_video.html
--rw-r--r--   0 quantra    (501) staff       (20)      286 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/partials/fields/previews/image.html
--rw-r--r--   0 quantra    (501) staff       (20)      389 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/partials/fields/previews/video.html
--rw-r--r--   0 quantra    (501) staff       (20)      442 2023-06-14 16:14:32.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/partials/loader.html
--rw-r--r--   0 quantra    (501) staff       (20)      499 2023-06-14 16:14:32.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/partials/popup.html
--rw-r--r--   0 quantra    (501) staff       (20)      221 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/partials/reset_popup.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.722113 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/widgets/
--rw-r--r--   0 quantra    (501) staff       (20)      499 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/widgets/choices.html
--rw-r--r--   0 quantra    (501) staff       (20)      574 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/widgets/clearable_file.html
--rw-r--r--   0 quantra    (501) staff       (20)      207 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/content_blocks/templates/content_blocks/widgets/filename_autocomplete.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.723731 django-content-blocks-1.3.5/content_blocks/templatetags/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-26 15:01:37.000000 django-content-blocks-1.3.5/content_blocks/templatetags/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)      514 2023-03-03 23:30:41.000000 django-content-blocks-1.3.5/content_blocks/templatetags/content_block_admin.py
--rw-r--r--   0 quantra    (501) staff       (20)     1555 2023-05-23 18:04:22.000000 django-content-blocks-1.3.5/content_blocks/templatetags/content_blocks.py
--rw-r--r--   0 quantra    (501) staff       (20)      699 2023-05-02 18:54:11.000000 django-content-blocks-1.3.5/content_blocks/urls.py
--rw-r--r--   0 quantra    (501) staff       (20)    12326 2023-05-23 18:04:22.000000 django-content-blocks-1.3.5/content_blocks/views.py
--rw-r--r--   0 quantra    (501) staff       (20)     2078 2023-06-06 15:28:11.000000 django-content-blocks-1.3.5/content_blocks/widgets.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-15 12:59:12.727891 django-content-blocks-1.3.5/django_content_blocks.egg-info/
--rw-r--r--   0 quantra    (501) staff       (20)     7611 2023-06-15 12:59:12.000000 django-content-blocks-1.3.5/django_content_blocks.egg-info/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)     4749 2023-06-15 12:59:12.000000 django-content-blocks-1.3.5/django_content_blocks.egg-info/SOURCES.txt
--rw-r--r--   0 quantra    (501) staff       (20)       40 2023-06-15 12:59:12.000000 django-content-blocks-1.3.5/django_content_blocks.egg-info/dependency_links.txt
--rw-r--r--   0 quantra    (501) staff       (20)       55 2023-06-15 12:59:12.000000 django-content-blocks-1.3.5/django_content_blocks.egg-info/requires.txt
--rw-r--r--   0 quantra    (501) staff       (20)       23 2023-06-15 12:59:12.000000 django-content-blocks-1.3.5/django_content_blocks.egg-info/top_level.txt
--rw-r--r--   0 quantra    (501) staff       (20)       89 2023-05-02 22:05:05.000000 django-content-blocks-1.3.5/pyproject.toml
--rw-r--r--   0 quantra    (501) staff       (20)     1977 2023-06-15 12:59:12.736594 django-content-blocks-1.3.5/setup.cfg
--rw-r--r--   0 quantra    (501) staff       (20)       38 2022-12-21 13:27:13.000000 django-content-blocks-1.3.5/setup.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.638172 django-content-blocks-1.3.6/
+-rw-r--r--   0 quantra    (501) staff       (20)     1076 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/LICENSE
+-rw-r--r--   0 quantra    (501) staff       (20)      147 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/MANIFEST.in
+-rw-r--r--   0 quantra    (501) staff       (20)     7611 2023-07-04 10:59:24.638292 django-content-blocks-1.3.6/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)     6072 2023-06-10 15:19:48.000000 django-content-blocks-1.3.6/README.rst
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.538364 django-content-blocks-1.3.6/content_blocks/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.6/content_blocks/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)      850 2023-05-23 18:04:22.000000 django-content-blocks-1.3.6/content_blocks/abstract_models.py
+-rw-r--r--   0 quantra    (501) staff       (20)    11988 2023-07-04 10:53:38.000000 django-content-blocks-1.3.6/content_blocks/admin.py
+-rw-r--r--   0 quantra    (501) staff       (20)     5301 2023-06-06 15:28:11.000000 django-content-blocks-1.3.6/content_blocks/admin_forms.py
+-rw-r--r--   0 quantra    (501) staff       (20)      952 2023-06-04 20:53:17.000000 django-content-blocks-1.3.6/content_blocks/apps.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1591 2023-06-03 20:41:24.000000 django-content-blocks-1.3.6/content_blocks/conf.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1653 2023-06-30 12:40:59.000000 django-content-blocks-1.3.6/content_blocks/fields.py
+-rw-r--r--   0 quantra    (501) staff       (20)     8031 2023-05-24 23:15:33.000000 django-content-blocks-1.3.6/content_blocks/forms.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.539126 django-content-blocks-1.3.6/content_blocks/management/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2022-09-05 20:58:44.000000 django-content-blocks-1.3.6/content_blocks/management/__init__.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.540899 django-content-blocks-1.3.6/content_blocks/management/commands/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2022-09-05 20:59:01.000000 django-content-blocks-1.3.6/content_blocks/management/commands/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)      420 2023-05-23 18:04:22.000000 django-content-blocks-1.3.6/content_blocks/management/commands/clear_content_blocks_cache.py
+-rw-r--r--   0 quantra    (501) staff       (20)      635 2023-07-04 00:00:43.000000 django-content-blocks-1.3.6/content_blocks/management/commands/export_content_block_templates.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1461 2023-05-24 11:55:23.000000 django-content-blocks-1.3.6/content_blocks/management/commands/import_content_block_templates.py
+-rw-r--r--   0 quantra    (501) staff       (20)      415 2023-05-23 18:04:22.000000 django-content-blocks-1.3.6/content_blocks/management/commands/set_content_blocks_cache.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.542369 django-content-blocks-1.3.6/content_blocks/migrations/
+-rw-r--r--   0 quantra    (501) staff       (20)    12063 2023-03-17 11:59:08.000000 django-content-blocks-1.3.6/content_blocks/migrations/0001_initial.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1784 2023-04-14 09:38:36.000000 django-content-blocks-1.3.6/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1154 2023-05-01 12:02:10.000000 django-content-blocks-1.3.6/content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.6/content_blocks/migrations/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)    24015 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/models.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.544223 django-content-blocks-1.3.6/content_blocks/services/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-05-23 18:56:52.000000 django-content-blocks-1.3.6/content_blocks/services/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)    12089 2023-06-30 12:40:59.000000 django-content-blocks-1.3.6/content_blocks/services/content_block.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1141 2023-05-23 18:04:22.000000 django-content-blocks-1.3.6/content_blocks/services/content_block_parent.py
+-rw-r--r--   0 quantra    (501) staff       (20)     5283 2023-05-24 11:55:40.000000 django-content-blocks-1.3.6/content_blocks/services/content_block_template.py
+-rw-r--r--   0 quantra    (501) staff       (20)     3312 2023-06-04 21:01:31.000000 django-content-blocks-1.3.6/content_blocks/signals.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.525410 django-content-blocks-1.3.6/content_blocks/static/
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.547015 django-content-blocks-1.3.6/content_blocks/static/content_blocks/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-28 23:45:54.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/.DS_Store
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.557104 django-content-blocks-1.3.6/content_blocks/static/content_blocks/css/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2022-12-22 00:43:03.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/css/.DS_Store
+-rw-r--r--   0 quantra    (501) staff       (20)     1114 2023-06-06 15:28:11.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/css/content_block_template_admin.css
+-rw-r--r--   0 quantra    (501) staff       (20)    10043 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/css/content_blocks.css
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.526131 django-content-blocks-1.3.6/content_blocks/static/content_blocks/fontawesome/
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.575217 django-content-blocks-1.3.6/content_blocks/static/content_blocks/fontawesome/css/
+-rw-r--r--   0 quantra    (501) staff       (20)    95481 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css
+-rw-r--r--   0 quantra    (501) staff       (20)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/fontawesome/css/light.min.css
+-rw-r--r--   0 quantra    (501) staff       (20)      747 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css
+-rw-r--r--   0 quantra    (501) staff       (20)      573 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/fontawesome/css/solid.min.css
+-rw-r--r--   0 quantra    (501) staff       (20)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/fontawesome/css/thin.min.css
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.582099 django-content-blocks-1.3.6/content_blocks/static/content_blocks/fontawesome/webfonts/
+-rw-r--r--   0 quantra    (501) staff       (20)   394832 2023-05-02 13:45:50.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 quantra    (501) staff       (20)   149908 2023-05-02 13:45:50.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.595657 django-content-blocks-1.3.6/content_blocks/static/content_blocks/iframeresizer/
+-rw-r--r--   0 quantra    (501) staff       (20)    34811 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js
+-rw-r--r--   0 quantra    (501) staff       (20)    37781 2023-05-02 13:45:50.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.604735 django-content-blocks-1.3.6/content_blocks/static/content_blocks/jqueryform/
+-rw-r--r--   0 quantra    (501) staff       (20)    17094 2023-05-02 13:45:50.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js
+-rw-r--r--   0 quantra    (501) staff       (20)    22565 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.614365 django-content-blocks-1.3.6/content_blocks/static/content_blocks/jqueryui/
+-rw-r--r--   0 quantra    (501) staff       (20)    30802 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css
+-rw-r--r--   0 quantra    (501) staff       (20)   255080 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.615738 django-content-blocks-1.3.6/content_blocks/static/content_blocks/js/
+-rw-r--r--   0 quantra    (501) staff       (20)     1894 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/js/admin_choices_widget.js
+-rw-r--r--   0 quantra    (501) staff       (20)      980 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/js/ajax_setup.js
+-rw-r--r--   0 quantra    (501) staff       (20)    19428 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/js/content_block_editor.js
+-rw-r--r--   0 quantra    (501) staff       (20)     2015 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/js/content_block_template_admin.js
+-rw-r--r--   0 quantra    (501) staff       (20)     2201 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/static/content_blocks/js/popup.js
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.621179 django-content-blocks-1.3.6/content_blocks/templates/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-03-16 15:09:32.000000 django-content-blocks-1.3.6/content_blocks/templates/.DS_Store
+-rw-r--r--   0 quantra    (501) staff       (20)      137 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/content_blocks/templates/base.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.623568 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-07 23:05:50.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/.DS_Store
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.624561 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/admin/
+-rw-r--r--   0 quantra    (501) staff       (20)      317 2023-06-04 15:21:52.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/admin/content_block_template_change_list.html
+-rw-r--r--   0 quantra    (501) staff       (20)      197 2023-06-06 15:28:11.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/admin/content_block_template_field_delete_checkbox.html
+-rw-r--r--   0 quantra    (501) staff       (20)     1366 2023-05-03 12:36:26.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/admin/content_block_template_import_form.html
+-rw-r--r--   0 quantra    (501) staff       (20)      305 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/content_block_collection.html
+-rw-r--r--   0 quantra    (501) staff       (20)      494 2023-05-23 18:04:22.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/content_block_preview.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.625983 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/editor/
+-rw-r--r--   0 quantra    (501) staff       (20)     1997 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/editor/base.html
+-rw-r--r--   0 quantra    (501) staff       (20)     2656 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/editor/content_block_form.html
+-rw-r--r--   0 quantra    (501) staff       (20)     4886 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html
+-rw-r--r--   0 quantra    (501) staff       (20)      439 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/editor/content_block_forms.html
+-rw-r--r--   0 quantra    (501) staff       (20)     4886 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/editor/editor.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.627072 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/partials/
+-rw-r--r--   0 quantra    (501) staff       (20)      187 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/partials/delete_popup.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.627712 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/partials/fields/
+-rw-r--r--   0 quantra    (501) staff       (20)      149 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/partials/fields/checkbox.html
+-rw-r--r--   0 quantra    (501) staff       (20)      497 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/partials/fields/default.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.628908 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/partials/fields/previews/
+-rw-r--r--   0 quantra    (501) staff       (20)      144 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/partials/fields/previews/base.html
+-rw-r--r--   0 quantra    (501) staff       (20)      464 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/partials/fields/previews/embedded_video.html
+-rw-r--r--   0 quantra    (501) staff       (20)      286 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/partials/fields/previews/image.html
+-rw-r--r--   0 quantra    (501) staff       (20)      389 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/partials/fields/previews/video.html
+-rw-r--r--   0 quantra    (501) staff       (20)      442 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/partials/loader.html
+-rw-r--r--   0 quantra    (501) staff       (20)      499 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/partials/popup.html
+-rw-r--r--   0 quantra    (501) staff       (20)      221 2023-07-04 00:10:28.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/partials/reset_popup.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.631389 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/widgets/
+-rw-r--r--   0 quantra    (501) staff       (20)      499 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/widgets/choices.html
+-rw-r--r--   0 quantra    (501) staff       (20)      574 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/widgets/clearable_file.html
+-rw-r--r--   0 quantra    (501) staff       (20)      207 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/content_blocks/templates/content_blocks/widgets/filename_autocomplete.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.632720 django-content-blocks-1.3.6/content_blocks/templatetags/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-26 15:01:37.000000 django-content-blocks-1.3.6/content_blocks/templatetags/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)      514 2023-03-03 23:30:41.000000 django-content-blocks-1.3.6/content_blocks/templatetags/content_block_admin.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1555 2023-05-23 18:04:22.000000 django-content-blocks-1.3.6/content_blocks/templatetags/content_blocks.py
+-rw-r--r--   0 quantra    (501) staff       (20)      699 2023-05-02 18:54:11.000000 django-content-blocks-1.3.6/content_blocks/urls.py
+-rw-r--r--   0 quantra    (501) staff       (20)    12326 2023-05-23 18:04:22.000000 django-content-blocks-1.3.6/content_blocks/views.py
+-rw-r--r--   0 quantra    (501) staff       (20)     2078 2023-06-06 15:28:11.000000 django-content-blocks-1.3.6/content_blocks/widgets.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-04 10:59:24.637976 django-content-blocks-1.3.6/django_content_blocks.egg-info/
+-rw-r--r--   0 quantra    (501) staff       (20)     7611 2023-07-04 10:59:24.000000 django-content-blocks-1.3.6/django_content_blocks.egg-info/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)     4749 2023-07-04 10:59:24.000000 django-content-blocks-1.3.6/django_content_blocks.egg-info/SOURCES.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       40 2023-07-04 10:59:24.000000 django-content-blocks-1.3.6/django_content_blocks.egg-info/dependency_links.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       55 2023-07-04 10:59:24.000000 django-content-blocks-1.3.6/django_content_blocks.egg-info/requires.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       23 2023-07-04 10:59:24.000000 django-content-blocks-1.3.6/django_content_blocks.egg-info/top_level.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       89 2023-05-02 22:05:05.000000 django-content-blocks-1.3.6/pyproject.toml
+-rw-r--r--   0 quantra    (501) staff       (20)     1977 2023-07-04 10:59:24.641391 django-content-blocks-1.3.6/setup.cfg
+-rw-r--r--   0 quantra    (501) staff       (20)       38 2022-12-21 13:27:13.000000 django-content-blocks-1.3.6/setup.py
```

### Comparing `django-content-blocks-1.3.5/LICENSE` & `django-content-blocks-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/PKG-INFO` & `django-content-blocks-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-content-blocks
-Version: 1.3.5
+Version: 1.3.6
 Summary: HTML content blocks for Django.
 Home-page: https://github.com/Quantra/django-content-blocks
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Documentation, https://django-content-blocks.readthedocs.io
 Project-URL: Source, https://github.com/Quantra/django-content-blocks
```

### Comparing `django-content-blocks-1.3.5/README.rst` & `django-content-blocks-1.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/abstract_models.py` & `django-content-blocks-1.3.6/content_blocks/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/admin.py` & `django-content-blocks-1.3.6/content_blocks/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     list_editable = ("visible",)
     list_filter = AUTO_DATE_FIELDS + ["visible"]
     search_fields = ("name", "template_filename")
 
     readonly_fields = AUTO_DATE_FIELDS
     inlines = [ContentBlockTemplateFieldInline]
     actions = ["export_content_block_templates"]
+    save_as = True
 
     class Media:
         css = {"all": ["content_blocks/css/content_block_template_admin.css"]}
         js = (
             "content_blocks/js/content_block_template_admin.js",
             "content_blocks/js/admin_choices_widget.js",
         )
```

### Comparing `django-content-blocks-1.3.5/content_blocks/admin_forms.py` & `django-content-blocks-1.3.6/content_blocks/admin_forms.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/apps.py` & `django-content-blocks-1.3.6/content_blocks/apps.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/conf.py` & `django-content-blocks-1.3.6/content_blocks/conf.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/fields.py` & `django-content-blocks-1.3.6/content_blocks/fields.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from django import forms
 from django.core.exceptions import ValidationError
 from django.core.validators import (
     FileExtensionValidator,
     get_available_image_extensions,
 )
 from django.db import models
-from django.db.models import FileField
 from django.db.models.fields.files import FieldFile
 
 
 def validate_svg(f):
     f.seek(0)
     tag = None
     try:
@@ -55,15 +54,15 @@
 
 class FieldVideo(FieldFile):
     @property
     def file_extension(self):
         return Path(self.name).suffix[1:]
 
 
-class VideoField(FileField):
+class VideoField(models.FileField):
     attr_class = FieldVideo
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.validators.append(
             FileExtensionValidator(allowed_extensions=["mp4", "webm", "ogg"])
         )
```

### Comparing `django-content-blocks-1.3.5/content_blocks/forms.py` & `django-content-blocks-1.3.6/content_blocks/forms.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/management/commands/export_content_block_templates.py` & `django-content-blocks-1.3.6/content_blocks/management/commands/export_content_block_templates.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from io import StringIO
+
 from django.core.management import BaseCommand
 
 from content_blocks.services.content_block_template import ImportExportServices
 
 
 class Command(BaseCommand):
     help = "Export content block templates to json."
 
     def handle(self, *args, **options):
         """
         Export ContentBlockTemplate and associated ContentBlockTemplateField to json via stdout.
         The output can be used for import_content_block_templates management command.
         """
-        ImportExportServices.export_content_block_templates(file_like=self.stdout)
+        buffer = StringIO()
+        ImportExportServices.export_content_block_templates(file_like=buffer)
+        self.stdout.write(buffer.getvalue())
```

### Comparing `django-content-blocks-1.3.5/content_blocks/management/commands/import_content_block_templates.py` & `django-content-blocks-1.3.6/content_blocks/management/commands/import_content_block_templates.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/migrations/0001_initial.py` & `django-content-blocks-1.3.6/content_blocks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py` & `django-content-blocks-1.3.6/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py` & `django-content-blocks-1.3.6/content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/models.py` & `django-content-blocks-1.3.6/content_blocks/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,14 +256,15 @@
         )
         # noinspection PyTypeChecker
         return forms.CharField(
             initial=self.text,
             required=self.template_field.required,
             help_text=self.template_field.help_text,
             widget=widget,
+            max_length=256,
         )
 
 
 class ContentField(ContentBlockField):
     class Meta:
         proxy = True
 
@@ -413,14 +414,15 @@
     @property
     def form_field(self):
         # noinspection PyTypeChecker
         return forms.CharField(
             initial=self.embedded_video,
             required=self.template_field.required,
             help_text=self.template_field.help_text,
+            max_length=256,
         )
 
 
 class ChoiceField(ContentBlockField):
     class Meta:
         proxy = True
```

### Comparing `django-content-blocks-1.3.5/content_blocks/services/content_block.py` & `django-content-blocks-1.3.6/content_blocks/services/content_block.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/services/content_block_parent.py` & `django-content-blocks-1.3.6/content_blocks/services/content_block_parent.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/services/content_block_template.py` & `django-content-blocks-1.3.6/content_blocks/services/content_block_template.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/signals.py` & `django-content-blocks-1.3.6/content_blocks/signals.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/.DS_Store` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/css/.DS_Store` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/css/content_block_template_admin.css` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/css/content_block_template_admin.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/css/content_blocks.css` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/css/content_blocks.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/fontawesome/css/solid.min.css` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/fontawesome/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/js/admin_choices_widget.js` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/js/admin_choices_widget.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/js/ajax_setup.js` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/js/ajax_setup.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/js/content_block_editor.js` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/js/content_block_editor.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/js/content_block_template_admin.js` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/js/content_block_template_admin.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/static/content_blocks/js/popup.js` & `django-content-blocks-1.3.6/content_blocks/static/content_blocks/js/popup.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/templates/.DS_Store` & `django-content-blocks-1.3.6/content_blocks/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/templates/content_blocks/.DS_Store` & `django-content-blocks-1.3.6/content_blocks/templates/content_blocks/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/templates/content_blocks/admin/content_block_template_import_form.html` & `django-content-blocks-1.3.6/content_blocks/templates/content_blocks/admin/content_block_template_import_form.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/templates/content_blocks/editor/base.html` & `django-content-blocks-1.3.6/content_blocks/templates/content_blocks/editor/base.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/templates/content_blocks/editor/content_block_form.html` & `django-content-blocks-1.3.6/content_blocks/templates/content_blocks/editor/content_block_form.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html` & `django-content-blocks-1.3.6/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/templates/content_blocks/editor/editor.html` & `django-content-blocks-1.3.6/content_blocks/templates/content_blocks/editor/editor.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/templates/content_blocks/widgets/clearable_file.html` & `django-content-blocks-1.3.6/content_blocks/templates/content_blocks/widgets/clearable_file.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/templatetags/content_block_admin.py` & `django-content-blocks-1.3.6/content_blocks/templatetags/content_block_admin.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/templatetags/content_blocks.py` & `django-content-blocks-1.3.6/content_blocks/templatetags/content_blocks.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/urls.py` & `django-content-blocks-1.3.6/content_blocks/urls.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/views.py` & `django-content-blocks-1.3.6/content_blocks/views.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/content_blocks/widgets.py` & `django-content-blocks-1.3.6/content_blocks/widgets.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/django_content_blocks.egg-info/PKG-INFO` & `django-content-blocks-1.3.6/django_content_blocks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-content-blocks
-Version: 1.3.5
+Version: 1.3.6
 Summary: HTML content blocks for Django.
 Home-page: https://github.com/Quantra/django-content-blocks
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Documentation, https://django-content-blocks.readthedocs.io
 Project-URL: Source, https://github.com/Quantra/django-content-blocks
```

### Comparing `django-content-blocks-1.3.5/django_content_blocks.egg-info/SOURCES.txt` & `django-content-blocks-1.3.6/django_content_blocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.5/setup.cfg` & `django-content-blocks-1.3.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-content-blocks
-version = 1.3.5
+version = 1.3.6
 description = HTML content blocks for Django.
 long_description = file:README.rst
 url = https://github.com/Quantra/django-content-blocks
 author = Vince Coleman
 author_email = vince@shystudios.co.uk
 license = MIT
 classifiers =
```

