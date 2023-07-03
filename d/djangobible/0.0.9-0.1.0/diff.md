# Comparing `tmp/djangobible-0.0.9.tar.gz` & `tmp/djangobible-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangobible-0.0.9.tar", last modified: Wed Oct 28 02:01:19 2020, max compression
+gzip compressed data, was "djangobible-0.1.0.tar", last modified: Mon Jul  3 22:47:22 2023, max compression
```

## Comparing `djangobible-0.0.9.tar` & `djangobible-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,52 @@
--rw-r--r--   0        0        0     2262 2020-10-27 18:00:12.441457 djangobible-0.0.9/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      715 2020-10-27 17:48:39.342953 djangobible-0.0.9/.github/workflows/django.yml
--rw-r--r--   0        0        0     1971 2020-10-09 03:33:01.891952 djangobible-0.0.9/.gitignore
--rw-r--r--   0        0        0     1091 2020-10-09 03:33:01.895945 djangobible-0.0.9/LICENSE
--rw-r--r--   0        0        0     1552 2020-10-28 01:59:23.247054 djangobible-0.0.9/README.md
--rw-r--r--   0        0        0       45 2020-10-18 23:43:36.419870 djangobible-0.0.9/__init__.py
--rw-r--r--   0        0        0      206 2020-10-28 02:00:26.421394 djangobible-0.0.9/djangobible/__init__.py
--rw-r--r--   0        0        0      102 2020-10-10 02:15:26.841191 djangobible-0.0.9/djangobible/apps.py
--rw-r--r--   0        0        0     1207 2020-10-10 02:15:26.901189 djangobible-0.0.9/djangobible/migrations/0001_initial.py
--rw-r--r--   0        0        0       58 2020-10-18 23:25:04.976566 djangobible-0.0.9/djangobible/migrations/__init__.py
--rw-r--r--   0        0        0     2155 2020-10-18 23:44:20.371406 djangobible-0.0.9/djangobible/models.py
--rw-r--r--   0        0        0      697 2020-10-18 23:44:20.327402 djangobible-0.0.9/manage.py
--rw-r--r--   0        0        0      659 2020-10-28 01:59:53.459453 djangobible-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      177 2020-10-10 02:09:17.806309 djangobible-0.0.9/pytest.ini
--rw-r--r--   0        0        0       36 2020-10-18 23:36:32.169986 djangobible-0.0.9/requirements.txt
--rw-r--r--   0        0        0       58 2020-10-12 15:35:46.348106 djangobible-0.0.9/test_django_app/__init__.py
--rw-r--r--   0        0        0      108 2020-10-10 02:15:31.876139 djangobible-0.0.9/test_django_app/apps.py
--rw-r--r--   0        0        0      766 2020-10-10 02:15:31.924137 djangobible-0.0.9/test_django_app/migrations/0001_initial.py
--rw-r--r--   0        0        0       63 2020-10-18 23:25:04.958460 djangobible-0.0.9/test_django_app/migrations/__init__.py
--rw-r--r--   0        0        0      332 2020-10-18 23:37:19.553224 djangobible-0.0.9/test_django_app/models.py
--rw-r--r--   0        0        0       49 2020-10-18 23:26:36.754738 djangobible-0.0.9/test_django_app/tests/__init__.py
--rw-r--r--   0        0        0     2261 2020-10-10 20:06:34.269947 djangobible-0.0.9/test_django_app/tests/conftest.py
--rw-r--r--   0        0        0     2533 2020-10-12 15:15:27.198297 djangobible-0.0.9/test_django_app/tests/test_models.py
--rw-r--r--   0        0        0      823 2020-10-10 20:06:34.221952 djangobible-0.0.9/test_django_app/tests/test_search.py
--rw-r--r--   0        0        0       62 2020-10-18 23:21:06.336139 djangobible-0.0.9/test_django_project/__init__.py
--rw-r--r--   0        0        0      431 2020-10-18 23:32:52.973212 djangobible-0.0.9/test_django_project/asgi.py
--rw-r--r--   0        0        0     3333 2020-10-18 23:32:46.749700 djangobible-0.0.9/test_django_project/settings.py
--rw-r--r--   0        0        0      784 2020-10-18 23:31:50.265596 djangobible-0.0.9/test_django_project/urls.py
--rw-r--r--   0        0        0      431 2020-10-10 02:15:38.198787 djangobible-0.0.9/test_django_project/wsgi.py
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 djangobible-0.0.9/setup.py
--rw-r--r--   0        0        0      201 1970-01-01 00:00:00.000000 djangobible-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0       75 2022-07-15 23:13:41.269564 djangobible-0.1.0/.coveragerc
+-rw-r--r--   0        0        0      282 2023-07-01 01:36:16.431867 djangobible-0.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2196 2023-07-01 02:24:51.433180 djangobible-0.1.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1052 2023-07-03 20:11:12.045217 djangobible-0.1.0/.github/workflows/django.yml
+-rw-r--r--   0        0        0     1837 2021-06-22 14:59:30.263767 djangobible-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1089 2023-05-27 20:57:45.007175 djangobible-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       34 2023-07-03 22:46:58.648769 djangobible-0.1.0/.sourcery.yaml
+-rw-r--r--   0        0        0      557 2023-07-03 22:46:58.649082 djangobible-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3357 2021-06-22 14:59:30.263836 djangobible-0.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1429 2022-07-15 23:13:41.270254 djangobible-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1070 2021-06-22 14:59:30.263955 djangobible-0.1.0/LICENSE
+-rw-r--r--   0        0        0     9129 2023-07-03 20:11:12.045960 djangobible-0.1.0/README.md
+-rw-r--r--   0        0        0      231 2023-07-03 22:46:58.649273 djangobible-0.1.0/djangobible/__init__.py
+-rw-r--r--   0        0        0      244 2022-07-15 23:13:41.270891 djangobible-0.1.0/djangobible/apps.py
+-rw-r--r--   0        0        0     3025 2023-07-03 22:46:58.649476 djangobible-0.1.0/djangobible/fields.py
+-rw-r--r--   0        0        0     1200 2023-05-27 20:57:45.008392 djangobible-0.1.0/djangobible/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-07-15 23:13:41.271368 djangobible-0.1.0/djangobible/migrations/__init__.py
+-rw-r--r--   0        0        0     3028 2022-07-15 23:13:41.271640 djangobible-0.1.0/djangobible/models.py
+-rw-r--r--   0        0        0        0 2021-06-22 14:59:30.264482 djangobible-0.1.0/djangobible/templatetags/__init__.py
+-rw-r--r--   0        0        0     1728 2023-07-03 22:46:58.649784 djangobible-0.1.0/djangobible/templatetags/verse_tags.py
+-rw-r--r--   0        0        0      853 2022-07-15 23:13:41.271921 djangobible-0.1.0/djangobible/validators.py
+-rw-r--r--   0        0        0      711 2022-07-15 23:13:41.272212 djangobible-0.1.0/manage.py
+-rw-r--r--   0        0        0      716 2023-07-03 22:46:58.649924 djangobible-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       11 2022-07-15 23:13:41.272553 djangobible-0.1.0/requirements-dev.txt
+-rw-r--r--   0        0        0       32 2022-07-15 23:13:41.272687 djangobible-0.1.0/requirements-test.txt
+-rw-r--r--   0        0        0       34 2023-07-03 20:11:12.046069 djangobible-0.1.0/requirements.txt
+-rw-r--r--   0        0        0     1499 2023-07-03 22:46:58.650070 djangobible-0.1.0/setup.cfg
+-rw-r--r--   0        0        0        0 2022-07-15 23:13:41.273090 djangobible-0.1.0/test_django_app/__init__.py
+-rw-r--r--   0        0        0      285 2022-07-15 23:13:41.273280 djangobible-0.1.0/test_django_app/admin.py
+-rw-r--r--   0        0        0      229 2022-07-15 23:13:41.273461 djangobible-0.1.0/test_django_app/apps.py
+-rw-r--r--   0        0        0      770 2023-05-27 20:57:45.008715 djangobible-0.1.0/test_django_app/migrations/0001_initial.py
+-rw-r--r--   0        0        0      826 2023-05-27 20:57:45.008828 djangobible-0.1.0/test_django_app/migrations/0002_testsingleverseobject.py
+-rw-r--r--   0        0        0      486 2023-05-27 20:57:45.008956 djangobible-0.1.0/test_django_app/migrations/0003_alter_testsingleverseobject_verse.py
+-rw-r--r--   0        0        0        0 2022-07-15 23:13:41.274052 djangobible-0.1.0/test_django_app/migrations/__init__.py
+-rw-r--r--   0        0        0      962 2022-07-15 23:13:41.274250 djangobible-0.1.0/test_django_app/models.py
+-rw-r--r--   0        0        0      443 2023-05-27 21:02:17.828564 djangobible-0.1.0/test_django_app/templates/verse_tags.html
+-rw-r--r--   0        0        0        0 2022-07-15 23:13:41.274479 djangobible-0.1.0/test_django_app/tests/__init__.py
+-rw-r--r--   0        0        0     1028 2022-07-15 23:13:41.275405 djangobible-0.1.0/test_django_app/tests/factories.py
+-rw-r--r--   0        0        0     2491 2022-07-15 23:13:41.275604 djangobible-0.1.0/test_django_app/tests/test_admin.py
+-rw-r--r--   0        0        0    11108 2022-07-15 23:13:41.275914 djangobible-0.1.0/test_django_app/tests/test_models.py
+-rw-r--r--   0        0        0     1861 2022-07-15 23:13:41.276255 djangobible-0.1.0/test_django_app/tests/test_search.py
+-rw-r--r--   0        0        0     4398 2023-05-27 21:01:27.797730 djangobible-0.1.0/test_django_app/tests/test_tags.py
+-rw-r--r--   0        0        0     1535 2023-05-27 21:02:43.291610 djangobible-0.1.0/test_django_app/tests/test_tags_functional.py
+-rw-r--r--   0        0        0      964 2022-07-15 23:13:41.276899 djangobible-0.1.0/test_django_app/tests/test_validators.py
+-rw-r--r--   0        0        0      357 2023-05-27 21:02:17.826182 djangobible-0.1.0/test_django_app/views.py
+-rw-r--r--   0        0        0        0 2022-07-15 23:13:41.277131 djangobible-0.1.0/test_django_project/__init__.py
+-rw-r--r--   0        0        0      451 2022-07-15 23:13:41.277293 djangobible-0.1.0/test_django_project/asgi.py
+-rw-r--r--   0        0        0     3499 2022-07-15 23:13:41.277464 djangobible-0.1.0/test_django_project/settings.py
+-rw-r--r--   0        0        0      247 2022-07-15 23:13:41.277617 djangobible-0.1.0/test_django_project/urls.py
+-rw-r--r--   0        0        0      451 2022-07-15 23:13:41.277770 djangobible-0.1.0/test_django_project/wsgi.py
+-rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 djangobible-0.1.0/setup.py
+-rw-r--r--   0        0        0      199 1970-01-01 00:00:00.000000 djangobible-0.1.0/PKG-INFO
```

### Comparing `djangobible-0.0.9/manage.py` & `djangobible-0.1.0/manage.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-#!/usr/bin/env python
-"""Django's command-line utility for administrative tasks."""
-import os
-import sys
-
-
-def main():
-    """Run administrative tasks."""
-    os.environ.setdefault("DJANGO_SETTINGS_MODULE", "test_django_project.settings")
-    try:
-        from django.core.management import execute_from_command_line
-    except ImportError as exc:
-        raise ImportError(
-            "Couldn't import Django. Are you sure it's installed and "
-            "available on your PYTHONPATH environment variable? Did you "
-            "forget to activate a virtual environment?"
-        ) from exc
-    execute_from_command_line(sys.argv)
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python
+"""Django's command-line utility for administrative tasks."""
+from __future__ import annotations
+
+import os
+import sys
+
+
+def main():
+    """Run administrative tasks."""
+    os.environ.setdefault("DJANGO_SETTINGS_MODULE", "test_django_project.settings")
+    try:
+        from django.core.management import execute_from_command_line
+    except ImportError as exc:
+        raise ImportError(
+            "Couldn't import Django. Are you sure it's installed and "
+            "available on your PYTHONPATH environment variable? Did you "
+            "forget to activate a virtual environment?"
+        ) from exc
+    execute_from_command_line(sys.argv)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `djangobible-0.0.9/setup.py` & `djangobible-0.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #!/usr/bin/env python
 # setup.py generated by flit for tools that don't yet use PEP 517
 
 from distutils.core import setup
 
 packages = \
-['djangobible', 'djangobible.migrations']
+['djangobible', 'djangobible.migrations', 'djangobible.templatetags']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Django >=3.0.0', 'pythonbible >=0.1.3']
+['Django >=3.2.0', 'pythonbible >=0.10.0']
 
 extras_require = \
-{'all': ['defusedxml >=0.6.0'],
- 'dev': ['bandit >=1.6.2', 'black >=20.8b1', 'prospector >=1.3.0'],
- 'test': ['pytest-django >=3.10.0']}
+{'all': ['defusedxml >=0.7.1'],
+ 'dev': ['pre-commit >=2.20.0'],
+ 'test': ['coverage >=6.4.2', 'factory-boy >=3.2.1', 'playwright >=1.23.1']}
 
 setup(name='djangobible',
-      version='0.0.9',
-      description='django-bible python library.',
+      version='0.1.0',
+      description='djangobible python library.',
       author='Nathan Patton',
       author_email='npatton@gmail.com',
-      url='https://github.com/avendesora/django-bible',
+      url='https://github.com/avendesora/djangobible',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
       extras_require=extras_require,
-      python_requires='>=3.6',
+      python_requires='>=3.8',
      )
```

