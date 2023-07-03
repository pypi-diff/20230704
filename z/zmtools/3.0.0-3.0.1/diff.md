# Comparing `tmp/zmtools-3.0.0.tar.gz` & `tmp/zmtools-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zmtools-3.0.0.tar", max compression
+gzip compressed data, was "zmtools-3.0.1.tar", max compression
```

## Comparing `zmtools-3.0.0.tar` & `zmtools-3.0.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-04-30 02:48:27.000000 zmtools-3.0.0/LICENSE
--rw-r--r--   0        0        0      145 2023-04-30 02:48:27.000000 zmtools-3.0.0/README.md
--rw-r--r--   0        0        0     1674 2023-04-30 02:49:14.929633 zmtools-3.0.0/pyproject.toml
--rw-r--r--   0        0        0       42 2023-04-30 02:49:14.930633 zmtools-3.0.0/zmtools/__init__.py
--rw-r--r--   0        0        0     5808 2023-04-30 02:48:27.000000 zmtools-3.0.0/zmtools/api.py
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 zmtools-3.0.0/setup.py
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 zmtools-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-30 02:33:58.655410 zmtools-3.0.1/LICENSE
+-rw-r--r--   0        0        0      145 2023-04-30 02:33:58.655567 zmtools-3.0.1/README.md
+-rw-r--r--   0        0        0     1691 2023-07-03 22:30:28.591102 zmtools-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-07-03 22:30:28.593482 zmtools-3.0.1/zmtools/__init__.py
+-rw-r--r--   0        0        0     5863 2023-05-07 13:05:53.198605 zmtools-3.0.1/zmtools/api.py
+-rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 zmtools-3.0.1/PKG-INFO
```

### Comparing `zmtools-3.0.0/LICENSE` & `zmtools-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zmtools-3.0.0/pyproject.toml` & `zmtools-3.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "zmtools"
-version = "3.0.0"
+version = "3.0.1"
 description = "Various tools used across Zeke Marffy's programs"
 authors = ["Zeke Marffy <zmarffy@yahoo.com>"]
 packages = [{ include = "zmtools" }]
 readme = "README.md"
 repository = "https://github.com/zmarffy/zmtools"
 homepage = "https://github.com/zmarffy/zmtools"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
+click = "^8.1.3"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-datafiles = "^3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
```

### Comparing `zmtools-3.0.0/zmtools/api.py` & `zmtools-3.0.1/zmtools/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,15 +137,17 @@
         package_name (str): The package name.
 
     Returns:
         str: The version of the package.
     """
     return re.findall(
         r"(?<=Version: ).+",
-        subprocess.check_output(["dpkg", "-s", package_name]).decode(),
+        subprocess.run(
+            ["dpkg", "-s", package_name], check=True, capture_output=True, text=True
+        ).stdout,
     )[0]
 
 
 def picker(items: list, item_name: str = "choice") -> Any:
     """Display a picker for a list of items, asking the user to select one. Return the selection.
 
     Args:
```

### Comparing `zmtools-3.0.0/PKG-INFO` & `zmtools-3.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: zmtools
-Version: 3.0.0
+Version: 3.0.1
 Summary: Various tools used across Zeke Marffy's programs
 Home-page: https://github.com/zmarffy/zmtools
 License: MIT
 Author: Zeke Marffy
 Author-email: zmarffy@yahoo.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
 Project-URL: Repository, https://github.com/zmarffy/zmtools
 Description-Content-Type: text/markdown
 
 # zmtools
 
 A conglomeration of functions reused in my programs; maybe they can help you too. The docstrings should explain all you need to know.
```

