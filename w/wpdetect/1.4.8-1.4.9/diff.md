# Comparing `tmp/wpdetect-1.4.8.tar.gz` & `tmp/wpdetect-1.4.9.tar.gz`

## Comparing `wpdetect-1.4.8.tar` & `wpdetect-1.4.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    15828 2020-02-02 00:00:00.000000 wpdetect-1.4.8/CHANGELOG.md
--rw-r--r--   0        0        0     5224 2020-02-02 00:00:00.000000 wpdetect-1.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 wpdetect-1.4.8/CONTRIBUTING.md
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 wpdetect-1.4.8/SECURITY.md
--rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 wpdetect-1.4.8/generate-changelog.sh
--rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 wpdetect-1.4.8/install-local.sh
--rwxr-xr-x   0        0        0     1089 2020-02-02 00:00:00.000000 wpdetect-1.4.8/release-tag.sh
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 wpdetect-1.4.8/requirements.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wpdetect-1.4.8/sample_urls.txt
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 wpdetect-1.4.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 wpdetect-1.4.8/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wpdetect-1.4.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 wpdetect-1.4.8/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 wpdetect-1.4.8/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 wpdetect-1.4.8/.vscode/settings.json
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 wpdetect-1.4.8/utils/bump_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.4.8/wpdetect/__init__.py
--rw-r--r--   0        0        0     7535 2020-02-02 00:00:00.000000 wpdetect-1.4.8/wpdetect/__main__.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.4.8/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.4.8/LICENSE.txt
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 wpdetect-1.4.8/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 wpdetect-1.4.8/pyproject.toml
--rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 wpdetect-1.4.8/PKG-INFO
+-rw-r--r--   0        0        0    12875 2020-02-02 00:00:00.000000 wpdetect-1.4.9/CHANGELOG.md
+-rw-r--r--   0        0        0     5224 2020-02-02 00:00:00.000000 wpdetect-1.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 wpdetect-1.4.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 wpdetect-1.4.9/SECURITY.md
+-rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 wpdetect-1.4.9/generate-changelog.sh
+-rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 wpdetect-1.4.9/install-local.sh
+-rwxr-xr-x   0        0        0     1118 2020-02-02 00:00:00.000000 wpdetect-1.4.9/release-tag.sh
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 wpdetect-1.4.9/requirements.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wpdetect-1.4.9/sample_urls.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 wpdetect-1.4.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 wpdetect-1.4.9/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wpdetect-1.4.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 wpdetect-1.4.9/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 wpdetect-1.4.9/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 wpdetect-1.4.9/.vscode/settings.json
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 wpdetect-1.4.9/utils/bump_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.4.9/wpdetect/__init__.py
+-rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 wpdetect-1.4.9/wpdetect/__main__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.4.9/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.4.9/LICENSE.txt
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 wpdetect-1.4.9/README.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 wpdetect-1.4.9/pyproject.toml
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 wpdetect-1.4.9/PKG-INFO
```

### Comparing `wpdetect-1.4.8/CODE_OF_CONDUCT.md` & `wpdetect-1.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.8/CONTRIBUTING.md` & `wpdetect-1.4.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.8/release-tag.sh` & `wpdetect-1.4.9/release-tag.sh`

 * *Files 27% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 # Run the version bumping script
 new_version=$($python_executable utils/bump_version.py)
 
 # Commit the updated version
 echo "Committing version $new_version"
 git add pyproject.toml
+git add wpdetect/__main__.py
 git commit -S -m "release $new_version"
 
 
 # Tag the release
 echo "Tagging version $new_version"
 git tag -s "$new_version" -m "release $new_version"
```

### Comparing `wpdetect-1.4.8/.github/ISSUE_TEMPLATE/bug_report.md` & `wpdetect-1.4.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.8/.github/ISSUE_TEMPLATE/feature_request.md` & `wpdetect-1.4.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.8/.github/workflows/pylint.yml` & `wpdetect-1.4.9/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.8/.github/workflows/pypi-publish.yml` & `wpdetect-1.4.9/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.8/utils/bump_version.py` & `wpdetect-1.4.9/utils/bump_version.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,28 @@
     This file increments the version in pyproject.toml.
 """
 
 import os
 import toml
 
 
+def write_changes_to_file(file_location, checker, version):
+    """Writes the changes to the file."""
+
+    with open(file_location, 'r', encoding="utf-8") as file:
+        lines = file.readlines()
+
+    with open(file_location, 'w', encoding="utf-8") as file:
+        for line in lines:
+            if line.startswith(checker):
+                file.write(f'{checker} = "{version}"\n')
+            else:
+                file.write(line)
+
+
 def increment_version():
     """Increments the version in pyproject.toml and returns the new version."""
 
     file_path = os.path.join(os.path.dirname(
         __file__), '..', 'pyproject.toml')
 
     with open(file_path, 'r', encoding="utf-8") as file:
@@ -19,23 +33,18 @@
 
     # Increment the version
     version_parts = current_version.split('.')
     version_parts[-1] = str(int(version_parts[-1]) + 1)
     new_version = '.'.join(version_parts)
 
     # Update the version in pyproject.toml
-    with open(file_path, 'r', encoding="utf-8") as file:
-        lines = file.readlines()
+    write_changes_to_file(file_path, 'version', new_version)
 
-    with open(file_path, 'w', encoding="utf-8") as file:
-        for line in lines:
-            if line.startswith('version'):
-                file.write(f'version = "{new_version}"\n')
-            else:
-                file.write(line)
+    # Update the version in wpdetect/__main__.py
+    write_changes_to_file('wpdetect/__main__.py', 'VERSION', new_version)
 
     return new_version
 
 
 # Call the increment_version() function
 BUMPED_VERSION = increment_version()
 print(f"v{BUMPED_VERSION}")
```

### Comparing `wpdetect-1.4.8/wpdetect/__main__.py` & `wpdetect-1.4.9/wpdetect/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 name: wpdetect
 description: A simple script to detect if a website is running WordPress.
 '''
 
 import sys
 import urllib.request
 from urllib.parse import urlparse
-import toml
 import click
 from pyfiglet import figlet_format
 
 HEADER = "'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3) AppleWebKit/537.75.14" + \
     " (KHTML, like Gecko) Version/7.0.3 Safari/7046A194A'"
+VERSION = "1.4.9"
 
 # Error messages
 ERROR_UNABLE_TO_OPEN_URL = "Couldn't open url," + \
     " please make sure to type a valid and publicly accessible url.\n"
 
 # List to store the found WordPress installations
 wp_domains = []
@@ -28,19 +28,15 @@
     'scan_full': False,  # default value
 }
 
 
 def get_package_version():
     """Returns the version of the package."""
 
-    # using absolute path to open the file because of the issue: #31
-    with open('pyproject.toml', 'r', encoding="utf-8") as pyproject_toml_file:
-        config = toml.load(pyproject_toml_file)
-
-    return config['project']['version']
+    return VERSION
 
 
 def print_verbose(message):
     """Prints the message if verbose is true."""
 
     if cli_options['verbose']:
         print(message)
```

### Comparing `wpdetect-1.4.8/.gitignore` & `wpdetect-1.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.8/LICENSE.txt` & `wpdetect-1.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.8/README.md` & `wpdetect-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.8/pyproject.toml` & `wpdetect-1.4.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wpdetect"
-version = "1.4.8"
+version = "1.4.9"
 dependencies = [
-    "pyfiglet", "requests", "click", "toml"
+    "pyfiglet", "requests", "click"
 ]
 authors = [
   { name="S M Mahmudul Hasan", email="he@smmahmudulhasan.com" },
 ]
 description = "A WordPress detection tool, detects if a website is running WordPress"
 readme = "README.md"
 requires-python = ">=3.4"
```

### Comparing `wpdetect-1.4.8/PKG-INFO` & `wpdetect-1.4.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpdetect
-Version: 1.4.8
+Version: 1.4.9
 Summary: A WordPress detection tool, detects if a website is running WordPress
 Project-URL: Homepage, https://github.com/IamLizu/wpdetect
 Project-URL: Bug Tracker, https://github.com/IamLizu/wpdetect/issues
 Project-URL: Changelog, https://github.com/IamLizu/wpdetect/blob/master/CHANGELOG.md
 Author-email: S M Mahmudul Hasan <he@smmahmudulhasan.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.4
 Requires-Dist: click
 Requires-Dist: pyfiglet
 Requires-Dist: requests
-Requires-Dist: toml
 Description-Content-Type: text/markdown
 
 # WP DETECT
 
 [![Pylint](https://github.com/IamLizu/wpdetect/actions/workflows/pylint.yml/badge.svg?event=push)](https://github.com/IamLizu/wpdetect/actions/workflows/pylint.yml)
 [![Upload Python Package](https://github.com/IamLizu/wpdetect/actions/workflows/pypi-publish.yml/badge.svg?event=release)](https://github.com/IamLizu/wpdetect/actions/workflows/pypi-publish.yml)
```

