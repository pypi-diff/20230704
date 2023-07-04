# Comparing `tmp/netbox_celery-0.1.1b5.tar.gz` & `tmp/netbox_celery-0.1.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_celery-0.1.1b5.tar", max compression
+gzip compressed data, was "netbox_celery-0.1.1b6.tar", max compression
```

## Comparing `netbox_celery-0.1.1b5.tar` & `netbox_celery-0.1.1b6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    10172 2023-03-24 10:29:45.705426 netbox_celery-0.1.1b5/LICENSE
--rw-r--r--   0        0        0     1331 2023-04-27 09:02:57.977928 netbox_celery-0.1.1b5/README.md
--rw-r--r--   0        0        0      587 2023-03-24 10:29:45.612506 netbox_celery-0.1.1b5/netbox_celery/__init__.py
--rw-r--r--   0        0        0       25 2023-03-24 10:29:45.678801 netbox_celery-0.1.1b5/netbox_celery/api/__init__.py
--rw-r--r--   0        0        0      563 2023-04-27 08:46:09.004236 netbox_celery-0.1.1b5/netbox_celery/api/serializers.py
--rw-r--r--   0        0        0      296 2023-04-20 09:59:17.598183 netbox_celery-0.1.1b5/netbox_celery/api/urls.py
--rw-r--r--   0        0        0      498 2023-04-27 08:46:09.004529 netbox_celery-0.1.1b5/netbox_celery/api/views.py
--rw-r--r--   0        0        0     1117 2023-03-24 10:29:45.683376 netbox_celery-0.1.1b5/netbox_celery/celery.py
--rw-r--r--   0        0        0     1578 2023-03-24 10:29:45.683648 netbox_celery-0.1.1b5/netbox_celery/choices.py
--rw-r--r--   0        0        0      669 2023-03-24 10:29:45.683923 netbox_celery-0.1.1b5/netbox_celery/filtersets.py
--rw-r--r--   0        0        0     4791 2023-04-27 09:02:57.985880 netbox_celery-0.1.1b5/netbox_celery/forms.py
--rw-r--r--   0        0        0     3888 2023-03-29 09:35:18.274302 netbox_celery-0.1.1b5/netbox_celery/migrations/0001_initial.py
--rw-r--r--   0        0        0      687 2023-03-24 10:29:45.689781 netbox_celery-0.1.1b5/netbox_celery/migrations/0002_rename_data_celeryresult_kwargs_celeryresult_args.py
--rw-r--r--   0        0        0      589 2023-03-24 10:29:45.689962 netbox_celery-0.1.1b5/netbox_celery/migrations/0003_celeryresult_result.py
--rw-r--r--   0        0        0      489 2023-03-29 09:35:18.257345 netbox_celery-0.1.1b5/netbox_celery/migrations/0004_alter_celeryresult_custom_field_data.py
--rw-r--r--   0        0        0        0 2023-03-24 10:29:45.690380 netbox_celery-0.1.1b5/netbox_celery/migrations/__init__.py
--rw-r--r--   0        0        0     5632 2023-04-27 08:46:09.005358 netbox_celery-0.1.1b5/netbox_celery/models.py
--rw-r--r--   0        0        0      284 2023-03-24 10:29:45.693847 netbox_celery-0.1.1b5/netbox_celery/navigation.py
--rw-r--r--   0        0        0     1639 2023-03-29 10:01:44.982974 netbox_celery-0.1.1b5/netbox_celery/schedule.py
--rw-r--r--   0        0        0     1737 2023-03-24 10:29:45.694515 netbox_celery-0.1.1b5/netbox_celery/settings_funcs.py
--rw-r--r--   0        0        0      755 2023-03-24 10:29:45.694890 netbox_celery-0.1.1b5/netbox_celery/tables.py
--rw-r--r--   0        0        0     2431 2023-04-27 09:02:57.986745 netbox_celery-0.1.1b5/netbox_celery/tasks.py
--rw-r--r--   0        0        0     3804 2023-03-24 10:29:45.695656 netbox_celery-0.1.1b5/netbox_celery/templates/netbox_celery/celery_task_form.html
--rw-r--r--   0        0        0     3387 2023-03-24 10:29:45.695921 netbox_celery-0.1.1b5/netbox_celery/templates/netbox_celery/celeryresult.html
--rw-r--r--   0        0        0       29 2023-03-24 10:29:45.696371 netbox_celery-0.1.1b5/netbox_celery/tests/__init__.py
--rw-r--r--   0        0        0     2177 2023-03-24 10:29:45.696652 netbox_celery-0.1.1b5/netbox_celery/tests/test_api.py
--rw-r--r--   0        0        0     1407 2023-03-24 10:29:45.696823 netbox_celery-0.1.1b5/netbox_celery/tests/test_views.py
--rw-r--r--   0        0        0      503 2023-03-24 10:29:45.697069 netbox_celery-0.1.1b5/netbox_celery/urls.py
--rw-r--r--   0        0        0     3621 2023-04-20 09:24:54.605356 netbox_celery-0.1.1b5/netbox_celery/views.py
--rw-r--r--   0        0        0     2049 2023-04-27 09:03:21.890768 netbox_celery-0.1.1b5/pyproject.toml
--rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 netbox_celery-0.1.1b5/PKG-INFO
+-rw-r--r--   0        0        0    10172 2023-03-24 10:29:45.705426 netbox_celery-0.1.1b6/LICENSE
+-rw-r--r--   0        0        0     1331 2023-04-27 09:02:57.977928 netbox_celery-0.1.1b6/README.md
+-rw-r--r--   0        0        0      587 2023-03-24 10:29:45.612506 netbox_celery-0.1.1b6/netbox_celery/__init__.py
+-rw-r--r--   0        0        0       25 2023-03-24 10:29:45.678801 netbox_celery-0.1.1b6/netbox_celery/api/__init__.py
+-rw-r--r--   0        0        0      563 2023-04-27 08:46:09.004236 netbox_celery-0.1.1b6/netbox_celery/api/serializers.py
+-rw-r--r--   0        0        0      296 2023-04-20 09:59:17.598183 netbox_celery-0.1.1b6/netbox_celery/api/urls.py
+-rw-r--r--   0        0        0      498 2023-04-27 08:46:09.004529 netbox_celery-0.1.1b6/netbox_celery/api/views.py
+-rw-r--r--   0        0        0     1117 2023-03-24 10:29:45.683376 netbox_celery-0.1.1b6/netbox_celery/celery.py
+-rw-r--r--   0        0        0     1578 2023-03-24 10:29:45.683648 netbox_celery-0.1.1b6/netbox_celery/choices.py
+-rw-r--r--   0        0        0      669 2023-03-24 10:29:45.683923 netbox_celery-0.1.1b6/netbox_celery/filtersets.py
+-rw-r--r--   0        0        0     4918 2023-07-04 14:47:45.776371 netbox_celery-0.1.1b6/netbox_celery/forms.py
+-rw-r--r--   0        0        0     3888 2023-03-29 09:35:18.274302 netbox_celery-0.1.1b6/netbox_celery/migrations/0001_initial.py
+-rw-r--r--   0        0        0      687 2023-03-24 10:29:45.689781 netbox_celery-0.1.1b6/netbox_celery/migrations/0002_rename_data_celeryresult_kwargs_celeryresult_args.py
+-rw-r--r--   0        0        0      589 2023-03-24 10:29:45.689962 netbox_celery-0.1.1b6/netbox_celery/migrations/0003_celeryresult_result.py
+-rw-r--r--   0        0        0      489 2023-03-29 09:35:18.257345 netbox_celery-0.1.1b6/netbox_celery/migrations/0004_alter_celeryresult_custom_field_data.py
+-rw-r--r--   0        0        0        0 2023-03-24 10:29:45.690380 netbox_celery-0.1.1b6/netbox_celery/migrations/__init__.py
+-rw-r--r--   0        0        0     5632 2023-04-27 08:46:09.005358 netbox_celery-0.1.1b6/netbox_celery/models.py
+-rw-r--r--   0        0        0      284 2023-03-24 10:29:45.693847 netbox_celery-0.1.1b6/netbox_celery/navigation.py
+-rw-r--r--   0        0        0     1639 2023-03-29 10:01:44.982974 netbox_celery-0.1.1b6/netbox_celery/schedule.py
+-rw-r--r--   0        0        0     1737 2023-03-24 10:29:45.694515 netbox_celery-0.1.1b6/netbox_celery/settings_funcs.py
+-rw-r--r--   0        0        0      755 2023-03-24 10:29:45.694890 netbox_celery-0.1.1b6/netbox_celery/tables.py
+-rw-r--r--   0        0        0     2431 2023-04-27 09:02:57.986745 netbox_celery-0.1.1b6/netbox_celery/tasks.py
+-rw-r--r--   0        0        0     3804 2023-03-24 10:29:45.695656 netbox_celery-0.1.1b6/netbox_celery/templates/netbox_celery/celery_task_form.html
+-rw-r--r--   0        0        0     3387 2023-03-24 10:29:45.695921 netbox_celery-0.1.1b6/netbox_celery/templates/netbox_celery/celeryresult.html
+-rw-r--r--   0        0        0       29 2023-03-24 10:29:45.696371 netbox_celery-0.1.1b6/netbox_celery/tests/__init__.py
+-rw-r--r--   0        0        0     2177 2023-03-24 10:29:45.696652 netbox_celery-0.1.1b6/netbox_celery/tests/test_api.py
+-rw-r--r--   0        0        0     1407 2023-03-24 10:29:45.696823 netbox_celery-0.1.1b6/netbox_celery/tests/test_views.py
+-rw-r--r--   0        0        0      503 2023-03-24 10:29:45.697069 netbox_celery-0.1.1b6/netbox_celery/urls.py
+-rw-r--r--   0        0        0     3621 2023-04-20 09:24:54.605356 netbox_celery-0.1.1b6/netbox_celery/views.py
+-rw-r--r--   0        0        0     2049 2023-07-04 14:47:45.776565 netbox_celery-0.1.1b6/pyproject.toml
+-rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 netbox_celery-0.1.1b6/PKG-INFO
```

### Comparing `netbox_celery-0.1.1b5/LICENSE` & `netbox_celery-0.1.1b6/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/README.md` & `netbox_celery-0.1.1b6/README.md`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/__init__.py` & `netbox_celery-0.1.1b6/netbox_celery/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/api/serializers.py` & `netbox_celery-0.1.1b6/netbox_celery/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/celery.py` & `netbox_celery-0.1.1b6/netbox_celery/celery.py`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/choices.py` & `netbox_celery-0.1.1b6/netbox_celery/choices.py`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/filtersets.py` & `netbox_celery-0.1.1b6/netbox_celery/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/forms.py` & `netbox_celery-0.1.1b6/netbox_celery/forms.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,16 @@
 import csv
 
 from celery import current_app
 from django import forms
 from django.core.exceptions import ValidationError
 from django.utils.translation import gettext as _
 from users.models import User
-from utilities.forms import (
-    APISelectMultiple,
-    DateTimePicker,
-    DynamicModelMultipleChoiceField,
-    MultipleChoiceField,
-)
+from utilities.forms.widgets import APISelectMultiple, DateTimePicker
+from utilities.forms.fields import DynamicModelMultipleChoiceField, MultipleChoiceField
 
 from netbox.forms import NetBoxModelFilterSetForm
 from netbox_celery.choices import CeleryResultStatusChoices
 from netbox_celery.models import CeleryResult
 
 
 class CeleryTaskForm(forms.Form):
@@ -23,20 +19,24 @@
 
     class Meta:
         """Meta class for CeleryTaskForm."""
 
         fields = ()
         task_name = None
 
+    def data_to_kwargs(self, data):
+        """Convert the data to kwargs."""
+        return data
+
     def save(self, request):
         """Save the form."""
         return CeleryResult.enqueue_job(
             self.Meta.task_name,
             user=request.user,
-            kwargs=self.cleaned_data,
+            kwargs=self.data_to_kwargs(self.cleaned_data),
         )
 
 
 class CeleryTaskBulkForm(forms.Form):
     """Base form for bulk Celery tasks."""
 
     csv_file = forms.FileField(
@@ -79,15 +79,15 @@
             form = self.Meta.base_form(row)
             if not form.is_valid():
                 return False
         return True
 
     def data_to_kwargs(self, data):
         """Convert the data to kwargs."""
-        raise NotImplementedError
+        return data
 
     def save(self, request):
         """Save the form."""
         if not getattr(self.Meta, "task_name", None):
             raise ValidationError("Please provide a task name in Meta class.")
 
         csv_data = self.read_csv()
```

### Comparing `netbox_celery-0.1.1b5/netbox_celery/migrations/0001_initial.py` & `netbox_celery-0.1.1b6/netbox_celery/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/migrations/0002_rename_data_celeryresult_kwargs_celeryresult_args.py` & `netbox_celery-0.1.1b6/netbox_celery/migrations/0002_rename_data_celeryresult_kwargs_celeryresult_args.py`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/migrations/0003_celeryresult_result.py` & `netbox_celery-0.1.1b6/netbox_celery/migrations/0003_celeryresult_result.py`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/models.py` & `netbox_celery-0.1.1b6/netbox_celery/models.py`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/schedule.py` & `netbox_celery-0.1.1b6/netbox_celery/schedule.py`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/settings_funcs.py` & `netbox_celery-0.1.1b6/netbox_celery/settings_funcs.py`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/tables.py` & `netbox_celery-0.1.1b6/netbox_celery/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/tasks.py` & `netbox_celery-0.1.1b6/netbox_celery/tasks.py`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/templates/netbox_celery/celery_task_form.html` & `netbox_celery-0.1.1b6/netbox_celery/templates/netbox_celery/celery_task_form.html`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/templates/netbox_celery/celeryresult.html` & `netbox_celery-0.1.1b6/netbox_celery/templates/netbox_celery/celeryresult.html`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/tests/test_api.py` & `netbox_celery-0.1.1b6/netbox_celery/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/tests/test_views.py` & `netbox_celery-0.1.1b6/netbox_celery/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/netbox_celery/views.py` & `netbox_celery-0.1.1b6/netbox_celery/views.py`

 * *Files identical despite different names*

### Comparing `netbox_celery-0.1.1b5/pyproject.toml` & `netbox_celery-0.1.1b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netbox-celery"
-version = "0.1.1-beta5"
+version = "0.1.1-beta6"
 description = ""
 authors = ["OpticoreIT <opensource@opticoreit.com>"]
 readme = "README.md"
 packages = [{include = "netbox_celery"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `netbox_celery-0.1.1b5/PKG-INFO` & `netbox_celery-0.1.1b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-celery
-Version: 0.1.1b5
+Version: 0.1.1b6
 Summary: 
 Author: OpticoreIT
 Author-email: opensource@opticoreit.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netbox-celery Version: 0.1.1b5 Summary: Author:
+Metadata-Version: 2.1 Name: netbox-celery Version: 0.1.1b6 Summary: Author:
 OpticoreIT Author-email: opensource@opticoreit.com Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: celery (>=5.2.7,<6.0.0) Requires-
 Dist: django-celery-beat (>=2.3.0,<3.0.0) Description-Content-Type: text/
 markdown # Netbox Celery Plugin
```

