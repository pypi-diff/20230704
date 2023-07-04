# Comparing `tmp/django-tomselect-0.4.2.tar.gz` & `tmp/django-tomselect-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tomselect-0.4.2.tar", last modified: Mon Jul  3 22:07:54 2023, max compression
+gzip compressed data, was "django-tomselect-0.4.3.tar", last modified: Tue Jul  4 05:54:35 2023, max compression
```

## Comparing `django-tomselect-0.4.2.tar` & `django-tomselect-0.4.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/
--rw-rw-r--   0 watervize  (1000) watervize  (1000)     1094 2023-07-03 19:44:33.000000 django-tomselect-0.4.2/LICENSE
--rw-rw-r--   0 watervize  (1000) watervize  (1000)    14181 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/PKG-INFO
--rw-rw-r--   0 watervize  (1000) watervize  (1000)    13740 2023-07-03 21:32:27.000000 django-tomselect-0.4.2/README.md
--rw-rw-r--   0 watervize  (1000) watervize  (1000)     1661 2023-07-03 22:01:14.000000 django-tomselect-0.4.2/pyproject.toml
--rw-rw-r--   0 watervize  (1000) watervize  (1000)       38 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/setup.cfg
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.265442 django-tomselect-0.4.2/src/
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/src/django_tomselect/
--rw-rw-r--   0 watervize  (1000) watervize  (1000)      122 2023-07-02 22:08:10.000000 django-tomselect-0.4.2/src/django_tomselect/__init__.py
--rw-rw-r--   0 watervize  (1000) watervize  (1000)      123 2023-07-03 21:29:51.000000 django-tomselect-0.4.2/src/django_tomselect/settings.py
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.265442 django-tomselect-0.4.2/src/django_tomselect/static/
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.265442 django-tomselect-0.4.2/src/django_tomselect/static/django_tomselect/
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/src/django_tomselect/static/django_tomselect/css/
--rw-rw-r--   0 watervize  (1000) watervize  (1000)      430 2023-06-30 11:53:27.000000 django-tomselect-0.4.2/src/django_tomselect/static/django_tomselect/css/django-tomselect.css
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/src/django_tomselect/static/django_tomselect/js/
--rw-r--r--   0 watervize  (1000) watervize  (1000)   148483 2023-07-03 22:07:52.000000 django-tomselect-0.4.2/src/django_tomselect/static/django_tomselect/js/django-tomselect.js
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.265442 django-tomselect-0.4.2/src/django_tomselect/static/vendor/
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.265442 django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/css/
--rw-rw-r--   0 watervize  (1000) watervize  (1000)    13682 2023-07-03 20:47:05.000000 django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap4.css
--rw-rw-r--   0 watervize  (1000) watervize  (1000)    18762 2023-07-03 20:47:07.000000 django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap4.css.map
--rw-rw-r--   0 watervize  (1000) watervize  (1000)    17697 2023-06-30 11:53:27.000000 django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css
--rw-rw-r--   0 watervize  (1000) watervize  (1000)    23112 2023-06-30 11:53:27.000000 django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map
--rw-rw-r--   0 watervize  (1000) watervize  (1000)     4678 2023-07-02 22:08:10.000000 django-tomselect-0.4.2/src/django_tomselect/views.py
--rw-rw-r--   0 watervize  (1000) watervize  (1000)     7652 2023-07-03 21:59:43.000000 django-tomselect-0.4.2/src/django_tomselect/widgets.py
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/src/django_tomselect.egg-info/
--rw-rw-r--   0 watervize  (1000) watervize  (1000)    14181 2023-07-03 22:07:54.000000 django-tomselect-0.4.2/src/django_tomselect.egg-info/PKG-INFO
--rw-rw-r--   0 watervize  (1000) watervize  (1000)      889 2023-07-03 22:07:54.000000 django-tomselect-0.4.2/src/django_tomselect.egg-info/SOURCES.txt
--rw-rw-r--   0 watervize  (1000) watervize  (1000)        1 2023-07-03 22:07:54.000000 django-tomselect-0.4.2/src/django_tomselect.egg-info/dependency_links.txt
--rw-rw-r--   0 watervize  (1000) watervize  (1000)        7 2023-07-03 22:07:54.000000 django-tomselect-0.4.2/src/django_tomselect.egg-info/requires.txt
--rw-rw-r--   0 watervize  (1000) watervize  (1000)       17 2023-07-03 22:07:54.000000 django-tomselect-0.4.2/src/django_tomselect.egg-info/top_level.txt
-drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-03 22:07:54.269441 django-tomselect-0.4.2/tests/
--rw-rw-r--   0 watervize  (1000) watervize  (1000)    16617 2023-07-02 22:16:57.000000 django-tomselect-0.4.2/tests/test_e2e.py
--rw-rw-r--   0 watervize  (1000) watervize  (1000)    16131 2023-07-02 21:58:43.000000 django-tomselect-0.4.2/tests/test_views.py
--rw-rw-r--   0 watervize  (1000) watervize  (1000)     5142 2023-07-02 22:37:18.000000 django-tomselect-0.4.2/tests/test_widgets.py
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-04 05:54:35.352424 django-tomselect-0.4.3/
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)     1094 2023-07-03 19:44:33.000000 django-tomselect-0.4.3/LICENSE
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    14852 2023-07-04 05:54:35.348423 django-tomselect-0.4.3/PKG-INFO
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    14411 2023-07-04 05:53:30.000000 django-tomselect-0.4.3/README.md
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)     1661 2023-07-04 05:42:14.000000 django-tomselect-0.4.3/pyproject.toml
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)       38 2023-07-04 05:54:35.352424 django-tomselect-0.4.3/setup.cfg
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-04 05:54:35.348423 django-tomselect-0.4.3/src/
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-04 05:54:35.348423 django-tomselect-0.4.3/src/django_tomselect/
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)      122 2023-07-02 22:08:10.000000 django-tomselect-0.4.3/src/django_tomselect/__init__.py
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)      123 2023-07-03 21:29:51.000000 django-tomselect-0.4.3/src/django_tomselect/settings.py
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-04 05:54:35.348423 django-tomselect-0.4.3/src/django_tomselect/static/
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-04 05:54:35.348423 django-tomselect-0.4.3/src/django_tomselect/static/django_tomselect/
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-04 05:54:35.348423 django-tomselect-0.4.3/src/django_tomselect/static/django_tomselect/css/
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)      430 2023-06-30 11:53:27.000000 django-tomselect-0.4.3/src/django_tomselect/static/django_tomselect/css/django-tomselect.css
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-04 05:54:35.348423 django-tomselect-0.4.3/src/django_tomselect/static/django_tomselect/js/
+-rw-r--r--   0 watervize  (1000) watervize  (1000)   148996 2023-07-04 05:54:33.000000 django-tomselect-0.4.3/src/django_tomselect/static/django_tomselect/js/django-tomselect.js
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-04 05:54:35.348423 django-tomselect-0.4.3/src/django_tomselect/static/django_tomselect/vendor/
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-04 05:54:35.348423 django-tomselect-0.4.3/src/django_tomselect/static/django_tomselect/vendor/tom-select/
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-04 05:54:35.348423 django-tomselect-0.4.3/src/django_tomselect/static/django_tomselect/vendor/tom-select/css/
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    13682 2023-07-03 20:47:05.000000 django-tomselect-0.4.3/src/django_tomselect/static/django_tomselect/vendor/tom-select/css/tom-select.bootstrap4.css
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    18762 2023-07-03 20:47:07.000000 django-tomselect-0.4.3/src/django_tomselect/static/django_tomselect/vendor/tom-select/css/tom-select.bootstrap4.css.map
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    17697 2023-06-30 11:53:27.000000 django-tomselect-0.4.3/src/django_tomselect/static/django_tomselect/vendor/tom-select/css/tom-select.bootstrap5.css
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    23112 2023-06-30 11:53:27.000000 django-tomselect-0.4.3/src/django_tomselect/static/django_tomselect/vendor/tom-select/css/tom-select.bootstrap5.css.map
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)     4678 2023-07-02 22:08:10.000000 django-tomselect-0.4.3/src/django_tomselect/views.py
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)     7686 2023-07-04 02:42:28.000000 django-tomselect-0.4.3/src/django_tomselect/widgets.py
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-04 05:54:35.348423 django-tomselect-0.4.3/src/django_tomselect.egg-info/
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    14852 2023-07-04 05:54:35.000000 django-tomselect-0.4.3/src/django_tomselect.egg-info/PKG-INFO
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)      957 2023-07-04 05:54:35.000000 django-tomselect-0.4.3/src/django_tomselect.egg-info/SOURCES.txt
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)        1 2023-07-04 05:54:35.000000 django-tomselect-0.4.3/src/django_tomselect.egg-info/dependency_links.txt
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)        7 2023-07-04 05:54:35.000000 django-tomselect-0.4.3/src/django_tomselect.egg-info/requires.txt
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)       17 2023-07-04 05:54:35.000000 django-tomselect-0.4.3/src/django_tomselect.egg-info/top_level.txt
+drwxrwxr-x   0 watervize  (1000) watervize  (1000)        0 2023-07-04 05:54:35.348423 django-tomselect-0.4.3/tests/
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    16617 2023-07-02 22:16:57.000000 django-tomselect-0.4.3/tests/test_e2e.py
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)    16131 2023-07-02 21:58:43.000000 django-tomselect-0.4.3/tests/test_views.py
+-rw-rw-r--   0 watervize  (1000) watervize  (1000)     5142 2023-07-02 22:37:18.000000 django-tomselect-0.4.3/tests/test_widgets.py
```

### Comparing `django-tomselect-0.4.2/LICENSE` & `django-tomselect-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tomselect-0.4.2/PKG-INFO` & `django-tomselect-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tomselect
-Version: 0.4.2
+Version: 0.4.3
 Summary: Django autocomplete widgets and views using Tom Select
 Author-email: Jack Linke <jacklinke@gmail.com>, Philip Becker <yummytea1@gmail.com>
 Project-URL: Source, https://github.com/jacklinke/django-tomselect
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -36,14 +36,15 @@
   * [Function & Features](#function--features)
     * [Modifying the initial QuerySet](#modifying-the-initial-queryset)
     * [Searching](#searching)
     * [Option creation](#option-creation)
       * [AJAX request](#ajax-request)
     * [List View link](#list-view-link)
     * [Chained Dropdown Filtering](#chained-dropdown-filtering)
+  * [Manually Initializing Tom Select Fields](#manually-initializing-tom-select-fields)
   * [Development & Demo](#development--demo)
 <!-- TOC -->
 
 ----
 
 ## Installation
 
@@ -366,14 +367,36 @@
 NOTE: When using `filter_by`, the declaring element now **requires** that the 
 other field provides a value, since its choices are dependent on the other 
 field. If the other field does not have a value, the search will not return any 
 results.
 
 ----
 
+## Manually Initializing Tom Select Fields
+
+If a form is added dynamically after the page loads (e.g.: with htmx), the new form 
+fields will not be initialized as django-tomselect fields. In order to manually 
+initialize them, dispatch a `triggerTomSelect` event, providing the id of the 
+form field as a value in `detail` as follows.
+
+```javascript
+<script>
+  document.addEventListener("DOMContentLoaded", (event) => {
+    window.dispatchEvent(new CustomEvent('triggerTomSelect', {
+      detail: {
+        elemID: 'id_tomselect_tabular'
+      }
+    }))
+  });
+</script>
+
+````
+
+----
+
 ## Development & Demo
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
 make init
 ```
```

### Comparing `django-tomselect-0.4.2/README.md` & `django-tomselect-0.4.3/src/django_tomselect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: django-tomselect
+Version: 0.4.3
+Summary: Django autocomplete widgets and views using Tom Select
+Author-email: Jack Linke <jacklinke@gmail.com>, Philip Becker <yummytea1@gmail.com>
+Project-URL: Source, https://github.com/jacklinke/django-tomselect
+Classifier: Framework :: Django
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Tom Select for Django
 
 Django autocomplete widgets and views using [Tom Select](https://tom-select.js.org/).
 
 This package provides a Django autocomplete widget and view that can be used
 together to provide a user interface for selecting a model instance from a
 database table.
@@ -24,14 +36,15 @@
   * [Function & Features](#function--features)
     * [Modifying the initial QuerySet](#modifying-the-initial-queryset)
     * [Searching](#searching)
     * [Option creation](#option-creation)
       * [AJAX request](#ajax-request)
     * [List View link](#list-view-link)
     * [Chained Dropdown Filtering](#chained-dropdown-filtering)
+  * [Manually Initializing Tom Select Fields](#manually-initializing-tom-select-fields)
   * [Development & Demo](#development--demo)
 <!-- TOC -->
 
 ----
 
 ## Installation
 
@@ -354,14 +367,36 @@
 NOTE: When using `filter_by`, the declaring element now **requires** that the 
 other field provides a value, since its choices are dependent on the other 
 field. If the other field does not have a value, the search will not return any 
 results.
 
 ----
 
+## Manually Initializing Tom Select Fields
+
+If a form is added dynamically after the page loads (e.g.: with htmx), the new form 
+fields will not be initialized as django-tomselect fields. In order to manually 
+initialize them, dispatch a `triggerTomSelect` event, providing the id of the 
+form field as a value in `detail` as follows.
+
+```javascript
+<script>
+  document.addEventListener("DOMContentLoaded", (event) => {
+    window.dispatchEvent(new CustomEvent('triggerTomSelect', {
+      detail: {
+        elemID: 'id_tomselect_tabular'
+      }
+    }))
+  });
+</script>
+
+````
+
+----
+
 ## Development & Demo
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
 make init
 ```
```

### Comparing `django-tomselect-0.4.2/pyproject.toml` & `django-tomselect-0.4.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-tomselect"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
   { name="Jack Linke", email="jacklinke@gmail.com" },
   { name="Philip Becker", email="yummytea1@gmail.com" },
 ]
 description = "Django autocomplete widgets and views using Tom Select"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `django-tomselect-0.4.2/src/django_tomselect/static/django_tomselect/js/django-tomselect.js` & `django-tomselect-0.4.3/src/django_tomselect/static/django_tomselect/js/django-tomselect.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -4583,32 +4583,52 @@
                 ts.on("blur", () => {
                     listviewLink.href = listviewURL;
                 });
             }
             ts.dropdown.appendChild(footer);
         }
     }
-    document.addEventListener("DOMContentLoaded", (event) => {
-        document.querySelectorAll("[is-tomselect]").forEach((elem) => {
-            const ts = new TomSelect(elem, getSettings2(elem));
-            attachFooter(ts, elem);
-            ts.on("type", (query) => {
-                if (!query) {
-                    ts.load("");
-                    ts.refreshOptions();
-                }
-            });
-            if (elem.filterByElem) {
-                elem.filterByElem.addEventListener("change", () => {
-                    ts.getUrl(null);
-                    ts.clearOptions();
-                    ts.wrapper.classList.remove("preloaded");
-                });
+
+    function attachTomSelectToElem(elem = null) {
+        const ts = new TomSelect(elem, getSettings2(elem));
+        attachFooter(ts, elem);
+        ts.on("type", (query) => {
+            if (!query) {
+                ts.load("");
+                ts.refreshOptions();
             }
         });
+        if (elem.filterByElem) {
+            elem.filterByElem.addEventListener("change", () => {
+                ts.getUrl(null);
+                ts.clearOptions();
+                ts.wrapper.classList.remove("preloaded");
+            });
+        }
+    }
+
+    function processElementsForTomSelect(elemID = null) {
+        if (elemID) {
+            const elem = document.querySelector(`[id="${elemID}"]`);
+            if (!elem) {
+                console.error(`No element with name "${elemID}" found.`);
+                return;
+            }
+            attachTomSelectToElem(elem);
+        } else {
+            document.querySelectorAll("[is-tomselect]").forEach((elem) => {
+                attachTomSelectToElem(elem);
+            });
+        }
+    }
+    document.addEventListener("DOMContentLoaded", (event) => {
+        processElementsForTomSelect();
+    });
+    window.addEventListener("triggerTomSelect", (e) => {
+        processElementsForTomSelect(e.detail.elemID);
     });
 })();
 /*! Bundled license information:
 
 @orchidjs/sifter/dist/umd/sifter.js:
   (*! sifter.js | https://github.com/orchidjs/sifter.js | Apache License (v2) *)
   (*! @orchidjs/unicode-variants | https://github.com/orchidjs/unicode-variants | Apache License (v2) *)
```

### Comparing `django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap4.css` & `django-tomselect-0.4.3/src/django_tomselect/static/django_tomselect/vendor/tom-select/css/tom-select.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap4.css.map` & `django-tomselect-0.4.3/src/django_tomselect/static/django_tomselect/vendor/tom-select/css/tom-select.bootstrap4.css.map`

 * *Files identical despite different names*

### Comparing `django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css` & `django-tomselect-0.4.3/src/django_tomselect/static/django_tomselect/vendor/tom-select/css/tom-select.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `django-tomselect-0.4.2/src/django_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map` & `django-tomselect-0.4.3/src/django_tomselect/static/django_tomselect/vendor/tom-select/css/tom-select.bootstrap5.css.map`

 * *Files identical despite different names*

### Comparing `django-tomselect-0.4.2/src/django_tomselect/views.py` & `django-tomselect-0.4.3/src/django_tomselect/views.py`

 * *Files identical despite different names*

### Comparing `django-tomselect-0.4.2/src/django_tomselect/widgets.py` & `django-tomselect-0.4.3/src/django_tomselect/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,25 +115,25 @@
 
     @property
     def media(self):
         if self.bootstrap_version == 4:
             return forms.Media(
                 css={
                     "all": [
-                        "vendor/tom-select/css/tom-select.bootstrap4.css",
+                        "django_tomselect/vendor/tom-select/css/tom-select.bootstrap4.css",
                         "django_tomselect/css/django-tomselect.css",
                     ],
                 },
                 js=["django_tomselect/js/django-tomselect.js"],
             )
         else:
             return forms.Media(
                 css={
                     "all": [
-                        "vendor/tom-select/css/tom-select.bootstrap5.css",
+                        "django_tomselect/vendor/tom-select/css/tom-select.bootstrap5.css",
                         "django_tomselect/css/django-tomselect.css",
                     ],
                 },
                 js=["django_tomselect/js/django-tomselect.js"],
             )
```

### Comparing `django-tomselect-0.4.2/src/django_tomselect.egg-info/PKG-INFO` & `django-tomselect-0.4.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: django-tomselect
-Version: 0.4.2
-Summary: Django autocomplete widgets and views using Tom Select
-Author-email: Jack Linke <jacklinke@gmail.com>, Philip Becker <yummytea1@gmail.com>
-Project-URL: Source, https://github.com/jacklinke/django-tomselect
-Classifier: Framework :: Django
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Tom Select for Django
 
 Django autocomplete widgets and views using [Tom Select](https://tom-select.js.org/).
 
 This package provides a Django autocomplete widget and view that can be used
 together to provide a user interface for selecting a model instance from a
 database table.
@@ -36,14 +24,15 @@
   * [Function & Features](#function--features)
     * [Modifying the initial QuerySet](#modifying-the-initial-queryset)
     * [Searching](#searching)
     * [Option creation](#option-creation)
       * [AJAX request](#ajax-request)
     * [List View link](#list-view-link)
     * [Chained Dropdown Filtering](#chained-dropdown-filtering)
+  * [Manually Initializing Tom Select Fields](#manually-initializing-tom-select-fields)
   * [Development & Demo](#development--demo)
 <!-- TOC -->
 
 ----
 
 ## Installation
 
@@ -366,14 +355,36 @@
 NOTE: When using `filter_by`, the declaring element now **requires** that the 
 other field provides a value, since its choices are dependent on the other 
 field. If the other field does not have a value, the search will not return any 
 results.
 
 ----
 
+## Manually Initializing Tom Select Fields
+
+If a form is added dynamically after the page loads (e.g.: with htmx), the new form 
+fields will not be initialized as django-tomselect fields. In order to manually 
+initialize them, dispatch a `triggerTomSelect` event, providing the id of the 
+form field as a value in `detail` as follows.
+
+```javascript
+<script>
+  document.addEventListener("DOMContentLoaded", (event) => {
+    window.dispatchEvent(new CustomEvent('triggerTomSelect', {
+      detail: {
+        elemID: 'id_tomselect_tabular'
+      }
+    }))
+  });
+</script>
+
+````
+
+----
+
 ## Development & Demo
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
 make init
 ```
```

### Comparing `django-tomselect-0.4.2/tests/test_e2e.py` & `django-tomselect-0.4.3/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `django-tomselect-0.4.2/tests/test_views.py` & `django-tomselect-0.4.3/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-tomselect-0.4.2/tests/test_widgets.py` & `django-tomselect-0.4.3/tests/test_widgets.py`

 * *Files identical despite different names*

