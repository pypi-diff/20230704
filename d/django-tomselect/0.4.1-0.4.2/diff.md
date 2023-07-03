# Comparing `tmp/django-tomselect-0.4.1.tar.gz` & `tmp/django-tomselect-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tomselect-0.4.1.tar", last modified: Mon Jul  3 19:46:46 2023, max compression
+gzip compressed data, was "django-tomselect-0.4.2.tar", last modified: Mon Jul  3 22:07:54 2023, max compression
```

## Comparing `django-tomselect-0.4.1.tar` & `django-tomselect-0.4.2.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 19:46:46.234637 django-tomselect-0.4.1/
--rw-rw-r--   0 watervize  (1000) watervize  (1000)     1094 2023-07-03 19:44:33.000000 django-tomselect-0.4.1/LICENSE
--rw-rw-r--   0 watervize  (1000) watervize  (1000)    14480 2023-07-03 19:46:46.234637 django-tomselect-0.4.1/PKG-INFO
--rw-rw-r--   0 watervize  (1000) watervize  (1000)    14039 2023-07-03 19:12:21.000000 django-tomselect-0.4.1/README.md
--rw-rw-r--   0 watervize  (1000) watervize  (1000)     1661 2023-07-03 19:43:15.000000 django-tomselect-0.4.1/pyproject.toml
--rw-rw-r--   0 watervize  (1000) watervize  (1000)       38 2023-07-03 19:46:46.234637 django-tomselect-0.4.1/setup.cfg
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 19:46:46.230637 django-tomselect-0.4.1/src/
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 19:46:46.230637 django-tomselect-0.4.1/src/django_tomselect/
--rw-rw-r--   0 watervize  (1000) watervize  (1000)      122 2023-07-02 22:08:10.000000 django-tomselect-0.4.1/src/django_tomselect/__init__.py
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 19:46:46.230637 django-tomselect-0.4.1/src/django_tomselect/static/
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 19:46:46.230637 django-tomselect-0.4.1/src/django_tomselect/static/django_tomselect/
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 19:46:46.230637 django-tomselect-0.4.1/src/django_tomselect/static/django_tomselect/css/
--rw-rw-r--   0 watervize  (1000) watervize  (1000)      430 2023-06-30 11:53:27.000000 django-tomselect-0.4.1/src/django_tomselect/static/django_tomselect/css/django-tomselect.css
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 19:46:46.230637 django-tomselect-0.4.1/src/django_tomselect/static/django_tomselect/js/
--rw-r--r--   0 watervize  (1000) watervize  (1000)   146409 2023-07-03 19:46:43.000000 django-tomselect-0.4.1/src/django_tomselect/static/django_tomselect/js/django-tomselect.js
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 19:46:46.230637 django-tomselect-0.4.1/src/django_tomselect/static/vendor/
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 19:46:46.230637 django-tomselect-0.4.1/src/django_tomselect/static/vendor/tom-select/
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 19:46:46.230637 django-tomselect-0.4.1/src/django_tomselect/static/vendor/tom-select/css/
--rw-rw-r--   0 watervize  (1000) watervize  (1000)    17697 2023-06-30 11:53:27.000000 django-tomselect-0.4.1/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css
--rw-rw-r--   0 watervize  (1000) watervize  (1000)    23112 2023-06-30 11:53:27.000000 django-tomselect-0.4.1/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map
--rw-rw-r--   0 watervize  (1000) watervize  (1000)     4678 2023-07-02 22:08:10.000000 django-tomselect-0.4.1/src/django_tomselect/views.py
--rw-rw-r--   0 watervize  (1000) watervize  (1000)     6711 2023-07-02 22:38:40.000000 django-tomselect-0.4.1/src/django_tomselect/widgets.py
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 19:46:46.230637 django-tomselect-0.4.1/src/django_tomselect.egg-info/
--rw-rw-r--   0 watervize  (1000) watervize  (1000)    14480 2023-07-03 19:46:46.000000 django-tomselect-0.4.1/src/django_tomselect.egg-info/PKG-INFO
--rw-rw-r--   0 watervize  (1000) watervize  (1000)      700 2023-07-03 19:46:46.000000 django-tomselect-0.4.1/src/django_tomselect.egg-info/SOURCES.txt
--rw-rw-r--   0 watervize  (1000) watervize  (1000)        1 2023-07-03 19:46:46.000000 django-tomselect-0.4.1/src/django_tomselect.egg-info/dependency_links.txt
--rw-rw-r--   0 watervize  (1000) watervize  (1000)        7 2023-07-03 19:46:46.000000 django-tomselect-0.4.1/src/django_tomselect.egg-info/requires.txt
--rw-rw-r--   0 watervize  (1000) watervize  (1000)       17 2023-07-03 19:46:46.000000 django-tomselect-0.4.1/src/django_tomselect.egg-info/top_level.txt
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 19:46:46.230637 django-tomselect-0.4.1/tests/
--rw-rw-r--   0 watervize  (1000) watervize  (1000)    16617 2023-07-02 22:16:57.000000 django-tomselect-0.4.1/tests/test_e2e.py
--rw-rw-r--   0 watervize  (1000) watervize  (1000)    16131 2023-07-02 21:58:43.000000 django-tomselect-0.4.1/tests/test_views.py
--rw-rw-r--   0 watervize  (1000) watervize  (1000)     5142 2023-07-02 22:37:18.000000 django-tomselect-0.4.1/tests/test_widgets.py
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)     1094 2023-07-03 19:44:33.000000 django-tomselect-0.4.2/LICENSE
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    14181 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/PKG-INFO
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    13740 2023-07-03 21:32:27.000000 django-tomselect-0.4.2/README.md
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)     1661 2023-07-03 22:01:14.000000 django-tomselect-0.4.2/pyproject.toml
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)       38 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/setup.cfg
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.265442 django-tomselect-0.4.2/src/
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/src/django_tomselect/
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)      122 2023-07-02 22:08:10.000000 django-tomselect-0.4.2/src/django_tomselect/__init__.py
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)      123 2023-07-03 21:29:51.000000 django-tomselect-0.4.2/src/django_tomselect/settings.py
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.265442 django-tomselect-0.4.2/src/django_tomselect/static/
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.265442 django-tomselect-0.4.2/src/django_tomselect/static/django_tomselect/
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/src/django_tomselect/static/django_tomselect/css/
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)      430 2023-06-30 11:53:27.000000 django-tomselect-0.4.2/src/django_tomselect/static/django_tomselect/css/django-tomselect.css
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/src/django_tomselect/static/django_tomselect/js/
+-rw-r--r--   0 watervize  (1000) watervize  (1000)   148483 2023-07-03 22:07:52.000000 django-tomselect-0.4.2/src/django_tomselect/static/django_tomselect/js/django-tomselect.js
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.265442 django-tomselect-0.4.2/src/django_tomselect/static/vendor/
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.265442 django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/css/
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    13682 2023-07-03 20:47:05.000000 django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap4.css
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    18762 2023-07-03 20:47:07.000000 django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap4.css.map
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    17697 2023-06-30 11:53:27.000000 django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    23112 2023-06-30 11:53:27.000000 django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)     4678 2023-07-02 22:08:10.000000 django-tomselect-0.4.2/src/django_tomselect/views.py
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)     7652 2023-07-03 21:59:43.000000 django-tomselect-0.4.2/src/django_tomselect/widgets.py
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/src/django_tomselect.egg-info/
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    14181 2023-07-03 22:07:54.000000 django-tomselect-0.4.2/src/django_tomselect.egg-info/PKG-INFO
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)      889 2023-07-03 22:07:54.000000 django-tomselect-0.4.2/src/django_tomselect.egg-info/SOURCES.txt
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)        1 2023-07-03 22:07:54.000000 django-tomselect-0.4.2/src/django_tomselect.egg-info/dependency_links.txt
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)        7 2023-07-03 22:07:54.000000 django-tomselect-0.4.2/src/django_tomselect.egg-info/requires.txt
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)       17 2023-07-03 22:07:54.000000 django-tomselect-0.4.2/src/django_tomselect.egg-info/top_level.txt
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/tests/
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    16617 2023-07-02 22:16:57.000000 django-tomselect-0.4.2/tests/test_e2e.py
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    16131 2023-07-02 21:58:43.000000 django-tomselect-0.4.2/tests/test_views.py
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)     5142 2023-07-02 22:37:18.000000 django-tomselect-0.4.2/tests/test_widgets.py
```

### Comparing `django-tomselect-0.4.1/LICENSE` & `django-tomselect-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tomselect-0.4.1/PKG-INFO` & `django-tomselect-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tomselect
-Version: 0.4.1
+Version: 0.4.2
 Summary: Django autocomplete widgets and views using Tom Select
 Author-email: Jack Linke <jacklinke@gmail.com>, Philip Becker <yummytea1@gmail.com>
 Project-URL: Source, https://github.com/jacklinke/django-tomselect
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -27,15 +27,18 @@
 * [Tom Select for Django](#tom-select-for-django)
   * [Installation](#installation)
   * [Usage](#usage)
   * [Widgets](#widgets)
     * [TomSelectWidget](#tomselectwidget)
     * [TomSelectTabularWidget](#tomselecttabularwidget)
       * [Adding more columns](#adding-more-columns-)
+  * [Settings](#settings)
+    * [TOMSELECT_BOOTSTRAP_VERSION](#tomselectbootstrapversion)
   * [Function & Features](#function--features)
+    * [Modifying the initial QuerySet](#modifying-the-initial-queryset)
     * [Searching](#searching)
     * [Option creation](#option-creation)
       * [AJAX request](#ajax-request)
     * [List View link](#list-view-link)
     * [Chained Dropdown Filtering](#chained-dropdown-filtering)
   * [Development & Demo](#development--demo)
 <!-- TOC -->
@@ -141,27 +144,27 @@
 HTML element via the dataset property. The Tom Select element is then initialized
 from the attributes in the dataset property.
 
 ### TomSelectWidget
 
 Base autocomplete widget. The arguments of TomSelectWidget are:
 
-| Argument       | Default value                                                                                                                                   | Description                                                                                    |
-|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------|
-| model          | **required**                                                                                                                                    | the model class that provides the choices                                                      |
-| url            | `"autocomplete"`                                                                                                                                | URL pattern name of the autocomplete view                                                      |
-| value_field    | `f"{model._meta.pk.name}"`                                                                                                                      | model field that provides the value of an option                                               |
-| label_field    | `getattr(model, "name_field", "name")`                                                                                                          | model field that provides the label of an option                                               |
-| search_lookups | <code>[<br/>&nbsp;&nbsp;&nbsp;&nbsp;f"{self.value_field}__icontains",<br/>&nbsp;&nbsp;&nbsp;&nbsp;f"{self.label_field}__icontains",<br/>]<code> | the list of lookups to use when filtering the results                                          |
-| create_field   |                                                                                                                                                 | model field to create new objects with ([see below](#ajax-request))                            |
-| multiple       | False                                                                                                                                           | if True, allow selecting multiple options                                                      |
-| listview_url   |                                                                                                                                                 | URL name of the list view for this model ([see below](#list-view-link))                        |
-| add_url        |                                                                                                                                                 | URL name of the add view for this model([see below](#option-creation))                         |
-| filter_by      |                                                                                                                                                 | a 2-tuple defining an additional filter ([see below](#chained-dropdown-filtering)) |
-
+| Argument          | Default value                                                           | Description                                                                        |
+|-------------------|-------------------------------------------------------------------------|------------------------------------------------------------------------------------|
+| model             | **required**                                                            | the model class that provides the choices                                          |
+| url               | `"autocomplete"`                                                        | URL pattern name of the autocomplete view                                          |
+| value_field       | `f"{model._meta.pk.name}"`                                              | model field that provides the value of an option                                   |
+| label_field       | `getattr(model, "name_field", "name")`                                  | model field that provides the label of an option                                   |
+| search_lookups    | `[f"{self.value_field}__icontains", f"{self.label_field}__icontains"]`  | the list of lookups to use when filtering the results                              |
+| create_field      | ""                                                                      | model field to create new objects with ([see below](#ajax-request))                |
+| multiple          | False                                                                   | if True, allow selecting multiple options                                          |
+| listview_url      | ""                                                                      | URL name of the list view for this model ([see below](#list-view-link))            |
+| add_url           | ""                                                                      | URL name of the add view for this model([see below](#option-creation))             |
+| filter_by         | ()                                                                      | a 2-tuple defining an additional filter ([see below](#chained-dropdown-filtering)) |
+| bootstrap_version | 5                                                                       | the bootstrap version to use, either `4` or `5`                                    |
 
 ### TomSelectTabularWidget
 
 This widget displays the results in tabular form. A table header will be added
 to the dropdown. By default, the table contains two columns: one column for the choice 
 value (commonly the "ID" of the option) and one column for the choice label (the 
 human-readable part of the choice).
@@ -210,14 +213,26 @@
 or property with that name or the column will remain empty. 
 The results for Tom Select are created by the view calling `values()` on the 
 result queryset, so you must make sure that the attribute name is available
 on the view's root queryset as either a model field or as an annotation.
 
 ----
 
+## Settings
+
+### TOMSELECT_BOOTSTRAP_VERSION
+
+The bootstrap version to use. Either `4` or `5`. Defaults to `5`.
+
+This sets the project-wide default for the `bootstrap_version` argument of the
+widgets. You can overwrite the default for a specific widget by passing the
+`bootstrap_version` argument to the widget.
+
+----
+
 ## Function & Features
 
 ### Modifying the initial QuerySet
 
 If you want to modify all autocomplete queries for a subclassed AutocompleteView, you can use `super()` with the `get_queryset()` method.
 
 ```python
```

### Comparing `django-tomselect-0.4.1/README.md` & `django-tomselect-0.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 * [Tom Select for Django](#tom-select-for-django)
   * [Installation](#installation)
   * [Usage](#usage)
   * [Widgets](#widgets)
     * [TomSelectWidget](#tomselectwidget)
     * [TomSelectTabularWidget](#tomselecttabularwidget)
       * [Adding more columns](#adding-more-columns-)
+  * [Settings](#settings)
+    * [TOMSELECT_BOOTSTRAP_VERSION](#tomselectbootstrapversion)
   * [Function & Features](#function--features)
+    * [Modifying the initial QuerySet](#modifying-the-initial-queryset)
     * [Searching](#searching)
     * [Option creation](#option-creation)
       * [AJAX request](#ajax-request)
     * [List View link](#list-view-link)
     * [Chained Dropdown Filtering](#chained-dropdown-filtering)
   * [Development & Demo](#development--demo)
 <!-- TOC -->
@@ -129,27 +132,27 @@
 HTML element via the dataset property. The Tom Select element is then initialized
 from the attributes in the dataset property.
 
 ### TomSelectWidget
 
 Base autocomplete widget. The arguments of TomSelectWidget are:
 
-| Argument       | Default value                                                                                                                                   | Description                                                                                    |
-|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------|
-| model          | **required**                                                                                                                                    | the model class that provides the choices                                                      |
-| url            | `"autocomplete"`                                                                                                                                | URL pattern name of the autocomplete view                                                      |
-| value_field    | `f"{model._meta.pk.name}"`                                                                                                                      | model field that provides the value of an option                                               |
-| label_field    | `getattr(model, "name_field", "name")`                                                                                                          | model field that provides the label of an option                                               |
-| search_lookups | <code>[<br/>&nbsp;&nbsp;&nbsp;&nbsp;f"{self.value_field}__icontains",<br/>&nbsp;&nbsp;&nbsp;&nbsp;f"{self.label_field}__icontains",<br/>]<code> | the list of lookups to use when filtering the results                                          |
-| create_field   |                                                                                                                                                 | model field to create new objects with ([see below](#ajax-request))                            |
-| multiple       | False                                                                                                                                           | if True, allow selecting multiple options                                                      |
-| listview_url   |                                                                                                                                                 | URL name of the list view for this model ([see below](#list-view-link))                        |
-| add_url        |                                                                                                                                                 | URL name of the add view for this model([see below](#option-creation))                         |
-| filter_by      |                                                                                                                                                 | a 2-tuple defining an additional filter ([see below](#chained-dropdown-filtering)) |
-
+| Argument          | Default value                                                           | Description                                                                        |
+|-------------------|-------------------------------------------------------------------------|------------------------------------------------------------------------------------|
+| model             | **required**                                                            | the model class that provides the choices                                          |
+| url               | `"autocomplete"`                                                        | URL pattern name of the autocomplete view                                          |
+| value_field       | `f"{model._meta.pk.name}"`                                              | model field that provides the value of an option                                   |
+| label_field       | `getattr(model, "name_field", "name")`                                  | model field that provides the label of an option                                   |
+| search_lookups    | `[f"{self.value_field}__icontains", f"{self.label_field}__icontains"]`  | the list of lookups to use when filtering the results                              |
+| create_field      | ""                                                                      | model field to create new objects with ([see below](#ajax-request))                |
+| multiple          | False                                                                   | if True, allow selecting multiple options                                          |
+| listview_url      | ""                                                                      | URL name of the list view for this model ([see below](#list-view-link))            |
+| add_url           | ""                                                                      | URL name of the add view for this model([see below](#option-creation))             |
+| filter_by         | ()                                                                      | a 2-tuple defining an additional filter ([see below](#chained-dropdown-filtering)) |
+| bootstrap_version | 5                                                                       | the bootstrap version to use, either `4` or `5`                                    |
 
 ### TomSelectTabularWidget
 
 This widget displays the results in tabular form. A table header will be added
 to the dropdown. By default, the table contains two columns: one column for the choice 
 value (commonly the "ID" of the option) and one column for the choice label (the 
 human-readable part of the choice).
@@ -198,14 +201,26 @@
 or property with that name or the column will remain empty. 
 The results for Tom Select are created by the view calling `values()` on the 
 result queryset, so you must make sure that the attribute name is available
 on the view's root queryset as either a model field or as an annotation.
 
 ----
 
+## Settings
+
+### TOMSELECT_BOOTSTRAP_VERSION
+
+The bootstrap version to use. Either `4` or `5`. Defaults to `5`.
+
+This sets the project-wide default for the `bootstrap_version` argument of the
+widgets. You can overwrite the default for a specific widget by passing the
+`bootstrap_version` argument to the widget.
+
+----
+
 ## Function & Features
 
 ### Modifying the initial QuerySet
 
 If you want to modify all autocomplete queries for a subclassed AutocompleteView, you can use `super()` with the `get_queryset()` method.
 
 ```python
```

### Comparing `django-tomselect-0.4.1/pyproject.toml` & `django-tomselect-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-tomselect"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="Jack Linke", email="jacklinke@gmail.com" },
   { name="Philip Becker", email="yummytea1@gmail.com" },
 ]
 description = "Django autocomplete widgets and views using Tom Select"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `django-tomselect-0.4.1/src/django_tomselect/static/django_tomselect/js/django-tomselect.js` & `django-tomselect-0.4.2/src/django_tomselect/static/django_tomselect/js/django-tomselect.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3997,16 +3997,76 @@
                     result = orig_method.apply(self2, arguments);
                 }
                 return result;
             };
         }
     };
 
+    // node_modules/tom-select/src/plugins/checkbox_options/plugin.ts
+    function plugin_default() {
+        var self2 = this;
+        var orig_onOptionSelect = self2.onOptionSelect;
+        self2.settings.hideSelected = false;
+        var UpdateCheckbox = function(option) {
+            setTimeout(() => {
+                var checkbox = option.querySelector("input");
+                if (checkbox instanceof HTMLInputElement) {
+                    if (option.classList.contains("selected")) {
+                        checkbox.checked = true;
+                    } else {
+                        checkbox.checked = false;
+                    }
+                }
+            }, 1);
+        };
+        self2.hook("after", "setupTemplates", () => {
+            var orig_render_option = self2.settings.render.option;
+            self2.settings.render.option = (data, escape_html2) => {
+                var rendered = getDom(orig_render_option.call(self2, data, escape_html2));
+                var checkbox = document.createElement("input");
+                checkbox.addEventListener("click", function(evt) {
+                    preventDefault(evt);
+                });
+                checkbox.type = "checkbox";
+                const hashed = hash_key(data[self2.settings.valueField]);
+                if (hashed && self2.items.indexOf(hashed) > -1) {
+                    checkbox.checked = true;
+                }
+                rendered.prepend(checkbox);
+                return rendered;
+            };
+        });
+        self2.on("item_remove", (value) => {
+            var option = self2.getOption(value);
+            if (option) {
+                option.classList.remove("selected");
+                UpdateCheckbox(option);
+            }
+        });
+        self2.on("item_add", (value) => {
+            var option = self2.getOption(value);
+            if (option) {
+                UpdateCheckbox(option);
+            }
+        });
+        self2.hook("instead", "onOptionSelect", (evt, option) => {
+            if (option.classList.contains("selected")) {
+                option.classList.remove("selected");
+                self2.removeItem(option.dataset.value);
+                self2.refreshOptions();
+                preventDefault(evt, true);
+                return;
+            }
+            orig_onOptionSelect.call(self2, evt, option);
+            UpdateCheckbox(option);
+        });
+    }
+
     // node_modules/tom-select/src/plugins/clear_button/plugin.ts
-    function plugin_default(userOptions) {
+    function plugin_default2(userOptions) {
         const self2 = this;
         const options = Object.assign({
             className: "clear-button",
             title: "Clear All",
             html: (data) => {
                 return `<div class="${data.className}" title="${data.title}">&#10799;</div>`;
             }
@@ -4025,15 +4085,15 @@
                 evt.stopPropagation();
             });
             self2.control.appendChild(button);
         });
     }
 
     // node_modules/tom-select/src/plugins/dropdown_header/plugin.ts
-    function plugin_default2(userOptions) {
+    function plugin_default3(userOptions) {
         const self2 = this;
         const options = Object.assign({
             title: "Untitled",
             headerClass: "dropdown-header",
             titleRowClass: "dropdown-header-title",
             labelClass: "dropdown-header-label",
             closeClass: "dropdown-header-close",
@@ -4051,15 +4111,15 @@
                 });
             }
             self2.dropdown.insertBefore(header, self2.dropdown.firstChild);
         });
     }
 
     // node_modules/tom-select/src/plugins/dropdown_input/plugin.ts
-    function plugin_default3() {
+    function plugin_default4() {
         const self2 = this;
         self2.settings.shouldOpen = true;
         self2.hook("before", "setup", () => {
             self2.focus_node = self2.control;
             addClasses(self2.control_input, "dropdown-input");
             const div = getDom('<div class="dropdown-input-wrap">');
             div.append(self2.control_input);
@@ -4104,15 +4164,15 @@
                     preventScroll: true
                 });
             });
         });
     }
 
     // node_modules/tom-select/src/plugins/remove_button/plugin.ts
-    function plugin_default4(userOptions) {
+    function plugin_default5(userOptions) {
         const options = Object.assign({
             label: "&times;",
             title: "Remove",
             className: "remove",
             append: true
         }, userOptions);
         var self2 = this;
@@ -4141,15 +4201,15 @@
                 });
                 return item;
             };
         });
     }
 
     // node_modules/tom-select/src/plugins/virtual_scroll/plugin.ts
-    function plugin_default5() {
+    function plugin_default6() {
         const self2 = this;
         const orig_canLoad = self2.canLoad;
         const orig_clearActiveOption = self2.clearActiveOption;
         const orig_loadCallback = self2.loadCallback;
         var pagination = {};
         var dropdown_content;
         var loading_more = false;
@@ -4274,19 +4334,20 @@
                 loading_more = true;
                 self2.load.call(self2, self2.lastValue);
             });
         });
     }
 
     // client/django-tomselect.js
-    TomSelect.define("clear_button", plugin_default);
-    TomSelect.define("dropdown_header", plugin_default2);
-    TomSelect.define("dropdown_input", plugin_default3);
-    TomSelect.define("remove_button", plugin_default4);
-    TomSelect.define("virtual_scroll", plugin_default5);
+    TomSelect.define("checkbox_options", plugin_default);
+    TomSelect.define("clear_button", plugin_default2);
+    TomSelect.define("dropdown_header", plugin_default3);
+    TomSelect.define("dropdown_input", plugin_default4);
+    TomSelect.define("remove_button", plugin_default5);
+    TomSelect.define("virtual_scroll", plugin_default6);
 
     function getFormPrefix(elem) {
         const parts = elem.getAttribute("name").split("-").slice(0, -1);
         if (parts.length) {
             return parts.join("-") + "-";
         }
         return "";
```

### Comparing `django-tomselect-0.4.1/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css` & `django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `django-tomselect-0.4.1/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map` & `django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map`

 * *Files identical despite different names*

### Comparing `django-tomselect-0.4.1/src/django_tomselect/views.py` & `django-tomselect-0.4.2/src/django_tomselect/views.py`

 * *Files identical despite different names*

### Comparing `django-tomselect-0.4.1/src/django_tomselect/widgets.py` & `django-tomselect-0.4.2/src/django_tomselect/widgets.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import json
 
 from django import forms
 from django.urls import reverse
 
+from .settings import DJANGO_TOMSELECT_BOOTSTRAP_VERSION
+
 
 class TomSelectWidget(forms.Select):
     """
     A Tom Select widget with model object choices.
 
     The Tom Select element will be configured using custom data attributes on
     the select element, which are provided by the widget's `build_attrs` method.
@@ -14,20 +16,21 @@
 
     def __init__(
         self,
         model,
         url="autocomplete",
         value_field="",
         label_field="",
-        search_lookups="",
+        search_lookups=(),
         create_field="",
         multiple=False,
         listview_url="",
         add_url="",
         filter_by=(),
+        bootstrap_version=DJANGO_TOMSELECT_BOOTSTRAP_VERSION,
         **kwargs,
     ):
         """
         Instantiate a TomSelectWidget widget.
 
         Args:
             model: the django model that the choices are derived from
@@ -47,14 +50,17 @@
             multiple: if True, allow selecting multiple options
             listview_url: URL name of the listview view for this model
             add_url: URL name of the add view for this model
             filter_by: a 2-tuple (form_field_name, field_lookup) to filter the
               results against the value of the form field using the given
               Django field lookup. For example:
                ('foo', 'bar__id') => results.filter(bar__id=data['foo'])
+            bootstrap_version: the Bootstrap version to use for the widget. Can
+                be set project-wide via settings.TOMSELECT_BOOTSTRAP_VERSION,
+                or per-widget instance. Defaults to 5.
             kwargs: additional keyword arguments passed to forms.Select
         """
         self.model = model
         self.url = url
         self.value_field = value_field or self.model._meta.pk.name
         self.label_field = label_field or getattr(self.model, "name_field", "name")
         self.search_lookups = search_lookups or [
@@ -62,14 +68,15 @@
             f"{self.label_field}__icontains",
         ]
         self.create_field = create_field
         self.multiple = multiple
         self.listview_url = listview_url
         self.add_url = add_url
         self.filter_by = filter_by
+        self.bootstrap_version = bootstrap_version if bootstrap_version in (4, 5) else 5
         super().__init__(**kwargs)
 
     def optgroups(self, name, value, attrs=None):
         return []  # Never provide any options; let the view serve the options.
 
     def get_url(self):
         """Hook to specify the autocomplete URL."""
@@ -102,22 +109,36 @@
                 "data-listview-url": self.get_listview_url() or "",
                 "data-add-url": self.get_add_url() or "",
                 "data-filter-by": json.dumps(list(self.filter_by)),
             }
         )
         return attrs
 
-    class Media:
-        css = {
-            "all": [
-                "vendor/tom-select/css/tom-select.bootstrap5.css",
-                "django_tomselect/css/django-tomselect.css",
-            ],
-        }
-        js = ["django_tomselect/js/django-tomselect.js"]
+    @property
+    def media(self):
+        if self.bootstrap_version == 4:
+            return forms.Media(
+                css={
+                    "all": [
+                        "vendor/tom-select/css/tom-select.bootstrap4.css",
+                        "django_tomselect/css/django-tomselect.css",
+                    ],
+                },
+                js=["django_tomselect/js/django-tomselect.js"],
+            )
+        else:
+            return forms.Media(
+                css={
+                    "all": [
+                        "vendor/tom-select/css/tom-select.bootstrap5.css",
+                        "django_tomselect/css/django-tomselect.css",
+                    ],
+                },
+                js=["django_tomselect/js/django-tomselect.js"],
+            )
 
 
 class TomSelectTabularWidget(TomSelectWidget):
     """TomSelectWidget widget that displays results in a table with header."""
 
     def __init__(
         self,
```

### Comparing `django-tomselect-0.4.1/src/django_tomselect.egg-info/PKG-INFO` & `django-tomselect-0.4.2/src/django_tomselect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tomselect
-Version: 0.4.1
+Version: 0.4.2
 Summary: Django autocomplete widgets and views using Tom Select
 Author-email: Jack Linke <jacklinke@gmail.com>, Philip Becker <yummytea1@gmail.com>
 Project-URL: Source, https://github.com/jacklinke/django-tomselect
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -27,15 +27,18 @@
 * [Tom Select for Django](#tom-select-for-django)
   * [Installation](#installation)
   * [Usage](#usage)
   * [Widgets](#widgets)
     * [TomSelectWidget](#tomselectwidget)
     * [TomSelectTabularWidget](#tomselecttabularwidget)
       * [Adding more columns](#adding-more-columns-)
+  * [Settings](#settings)
+    * [TOMSELECT_BOOTSTRAP_VERSION](#tomselectbootstrapversion)
   * [Function & Features](#function--features)
+    * [Modifying the initial QuerySet](#modifying-the-initial-queryset)
     * [Searching](#searching)
     * [Option creation](#option-creation)
       * [AJAX request](#ajax-request)
     * [List View link](#list-view-link)
     * [Chained Dropdown Filtering](#chained-dropdown-filtering)
   * [Development & Demo](#development--demo)
 <!-- TOC -->
@@ -141,27 +144,27 @@
 HTML element via the dataset property. The Tom Select element is then initialized
 from the attributes in the dataset property.
 
 ### TomSelectWidget
 
 Base autocomplete widget. The arguments of TomSelectWidget are:
 
-| Argument       | Default value                                                                                                                                   | Description                                                                                    |
-|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------|
-| model          | **required**                                                                                                                                    | the model class that provides the choices                                                      |
-| url            | `"autocomplete"`                                                                                                                                | URL pattern name of the autocomplete view                                                      |
-| value_field    | `f"{model._meta.pk.name}"`                                                                                                                      | model field that provides the value of an option                                               |
-| label_field    | `getattr(model, "name_field", "name")`                                                                                                          | model field that provides the label of an option                                               |
-| search_lookups | <code>[<br/>&nbsp;&nbsp;&nbsp;&nbsp;f"{self.value_field}__icontains",<br/>&nbsp;&nbsp;&nbsp;&nbsp;f"{self.label_field}__icontains",<br/>]<code> | the list of lookups to use when filtering the results                                          |
-| create_field   |                                                                                                                                                 | model field to create new objects with ([see below](#ajax-request))                            |
-| multiple       | False                                                                                                                                           | if True, allow selecting multiple options                                                      |
-| listview_url   |                                                                                                                                                 | URL name of the list view for this model ([see below](#list-view-link))                        |
-| add_url        |                                                                                                                                                 | URL name of the add view for this model([see below](#option-creation))                         |
-| filter_by      |                                                                                                                                                 | a 2-tuple defining an additional filter ([see below](#chained-dropdown-filtering)) |
-
+| Argument          | Default value                                                           | Description                                                                        |
+|-------------------|-------------------------------------------------------------------------|------------------------------------------------------------------------------------|
+| model             | **required**                                                            | the model class that provides the choices                                          |
+| url               | `"autocomplete"`                                                        | URL pattern name of the autocomplete view                                          |
+| value_field       | `f"{model._meta.pk.name}"`                                              | model field that provides the value of an option                                   |
+| label_field       | `getattr(model, "name_field", "name")`                                  | model field that provides the label of an option                                   |
+| search_lookups    | `[f"{self.value_field}__icontains", f"{self.label_field}__icontains"]`  | the list of lookups to use when filtering the results                              |
+| create_field      | ""                                                                      | model field to create new objects with ([see below](#ajax-request))                |
+| multiple          | False                                                                   | if True, allow selecting multiple options                                          |
+| listview_url      | ""                                                                      | URL name of the list view for this model ([see below](#list-view-link))            |
+| add_url           | ""                                                                      | URL name of the add view for this model([see below](#option-creation))             |
+| filter_by         | ()                                                                      | a 2-tuple defining an additional filter ([see below](#chained-dropdown-filtering)) |
+| bootstrap_version | 5                                                                       | the bootstrap version to use, either `4` or `5`                                    |
 
 ### TomSelectTabularWidget
 
 This widget displays the results in tabular form. A table header will be added
 to the dropdown. By default, the table contains two columns: one column for the choice 
 value (commonly the "ID" of the option) and one column for the choice label (the 
 human-readable part of the choice).
@@ -210,14 +213,26 @@
 or property with that name or the column will remain empty. 
 The results for Tom Select are created by the view calling `values()` on the 
 result queryset, so you must make sure that the attribute name is available
 on the view's root queryset as either a model field or as an annotation.
 
 ----
 
+## Settings
+
+### TOMSELECT_BOOTSTRAP_VERSION
+
+The bootstrap version to use. Either `4` or `5`. Defaults to `5`.
+
+This sets the project-wide default for the `bootstrap_version` argument of the
+widgets. You can overwrite the default for a specific widget by passing the
+`bootstrap_version` argument to the widget.
+
+----
+
 ## Function & Features
 
 ### Modifying the initial QuerySet
 
 If you want to modify all autocomplete queries for a subclassed AutocompleteView, you can use `super()` with the `get_queryset()` method.
 
 ```python
```

### Comparing `django-tomselect-0.4.1/src/django_tomselect.egg-info/SOURCES.txt` & `django-tomselect-0.4.2/src/django_tomselect.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
 src/django_tomselect/__init__.py
+src/django_tomselect/settings.py
 src/django_tomselect/views.py
 src/django_tomselect/widgets.py
 src/django_tomselect.egg-info/PKG-INFO
 src/django_tomselect.egg-info/SOURCES.txt
 src/django_tomselect.egg-info/dependency_links.txt
 src/django_tomselect.egg-info/requires.txt
 src/django_tomselect.egg-info/top_level.txt
 src/django_tomselect/static/django_tomselect/css/django-tomselect.css
 src/django_tomselect/static/django_tomselect/js/django-tomselect.js
+src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap4.css
+src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap4.css.map
 src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css
 src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map
 tests/test_e2e.py
 tests/test_views.py
 tests/test_widgets.py
```

### Comparing `django-tomselect-0.4.1/tests/test_e2e.py` & `django-tomselect-0.4.2/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `django-tomselect-0.4.1/tests/test_views.py` & `django-tomselect-0.4.2/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-tomselect-0.4.1/tests/test_widgets.py` & `django-tomselect-0.4.2/tests/test_widgets.py`

 * *Files identical despite different names*

