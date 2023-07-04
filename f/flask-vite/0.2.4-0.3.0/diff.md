# Comparing `tmp/flask_vite-0.2.4.tar.gz` & `tmp/flask_vite-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_vite-0.2.4.tar", max compression
+gzip compressed data, was "flask_vite-0.3.0.tar", max compression
```

## Comparing `flask_vite-0.2.4.tar` & `flask_vite-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0     1070 2022-04-08 07:03:12.325318 flask_vite-0.2.4/LICENSE
--rw-r--r--   0        0        0     1395 2022-11-02 07:44:40.948526 flask_vite-0.2.4/README.md
--rw-r--r--   0        0        0     1367 2023-03-29 13:15:37.907340 flask_vite-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       48 2022-09-02 18:03:03.970225 flask_vite-0.2.4/src/flask_vite/__init__.py
--rw-r--r--   0        0        0     1499 2023-03-29 13:14:22.348889 flask_vite-0.2.4/src/flask_vite/cli.py
--rw-r--r--   0        0        0     1512 2023-01-04 10:16:29.839673 flask_vite-0.2.4/src/flask_vite/extension.py
--rw-r--r--   0        0        0      737 2022-11-27 18:02:52.022408 flask_vite-0.2.4/src/flask_vite/npm.py
--rw-r--r--   0        0        0       12 2022-04-08 07:03:12.420495 flask_vite-0.2.4/src/flask_vite/starter/.gitignore
--rw-r--r--   0        0        0      650 2022-04-08 07:03:12.420123 flask_vite-0.2.4/src/flask_vite/starter/bs.config.js
--rw-r--r--   0        0        0     1421 2022-04-08 07:03:12.420695 flask_vite-0.2.4/src/flask_vite/starter/package.json
--rw-r--r--   0        0        0      123 2022-04-08 07:03:12.420844 flask_vite-0.2.4/src/flask_vite/starter/postcss.config.js
--rw-r--r--   0        0        0       59 2022-04-08 07:03:12.421128 flask_vite-0.2.4/src/flask_vite/starter/src/styles.css
--rw-r--r--   0        0        0     1346 2022-04-08 07:03:12.420281 flask_vite-0.2.4/src/flask_vite/starter/tailwind.config.js
--rw-r--r--   0        0        0      902 2023-01-04 10:16:52.879813 flask_vite-0.2.4/src/flask_vite/tags.py
--rw-r--r--   0        0        0       40 2022-04-08 07:28:14.665349 flask_vite-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0      677 2022-04-08 07:28:14.668027 flask_vite-0.2.4/tests/test_flask_vite.py
--rw-r--r--   0        0        0     2213 1970-01-01 00:00:00.000000 flask_vite-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-04-08 07:03:12.325318 flask_vite-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1581 2023-07-04 09:27:06.820368 flask_vite-0.3.0/README.md
+-rw-r--r--   0        0        0     1423 2023-07-04 09:29:58.807372 flask_vite-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       48 2022-09-02 18:03:03.970225 flask_vite-0.3.0/src/flask_vite/__init__.py
+-rw-r--r--   0        0        0     1522 2023-05-15 13:48:16.717305 flask_vite-0.3.0/src/flask_vite/cli.py
+-rw-r--r--   0        0        0     1587 2023-07-04 09:26:28.834945 flask_vite-0.3.0/src/flask_vite/extension.py
+-rw-r--r--   0        0        0      642 2023-07-03 16:44:58.183095 flask_vite-0.3.0/src/flask_vite/npm.py
+-rw-r--r--   0        0        0       50 2023-07-04 09:13:43.637994 flask_vite-0.3.0/src/flask_vite/starter/.gitignore
+-rw-r--r--   0        0        0      650 2022-04-08 07:03:12.420123 flask_vite-0.3.0/src/flask_vite/starter/bs.config.js
+-rw-r--r--   0        0        0      280 2023-07-04 08:57:59.573627 flask_vite-0.3.0/src/flask_vite/starter/index.html
+-rw-r--r--   0        0        0       27 2023-07-04 09:14:53.281846 flask_vite-0.3.0/src/flask_vite/starter/main.js
+-rw-r--r--   0        0        0      359 2023-07-04 09:01:33.300027 flask_vite-0.3.0/src/flask_vite/starter/package.json
+-rw-r--r--   0        0        0       82 2023-07-04 09:05:39.738914 flask_vite-0.3.0/src/flask_vite/starter/postcss.config.js
+-rw-r--r--   0        0        0       59 2023-07-04 08:17:31.233442 flask_vite-0.3.0/src/flask_vite/starter/src/styles.css
+-rw-r--r--   0        0        0      157 2023-07-04 09:03:39.209131 flask_vite-0.3.0/src/flask_vite/starter/tailwind.config.js
+-rw-r--r--   0        0        0      131 2023-07-04 08:17:31.234222 flask_vite-0.3.0/src/flask_vite/starter/vite.config.js
+-rw-r--r--   0        0        0      902 2023-01-04 10:16:52.879813 flask_vite-0.3.0/src/flask_vite/tags.py
+-rw-r--r--   0        0        0       40 2022-04-08 07:28:14.665349 flask_vite-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      677 2022-04-08 07:28:14.668027 flask_vite-0.3.0/tests/test_flask_vite.py
+-rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 flask_vite-0.3.0/PKG-INFO
```

### Comparing `flask_vite-0.2.4/LICENSE` & `flask_vite-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_vite-0.2.4/README.md` & `flask_vite-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Flask-Vite
 
 [![image](https://img.shields.io/pypi/v/flask-tailwind.svg)](https://pypi.python.org/pypi/flask-tailwind)
 
 Plugin to simplify use of Vite from Flask.
 
--   Status: Alpha.
+-   Status: Bêta.
 -   Free software: MIT license
 
 ## Usage
 
 Instantiate the Flask extension as you do for other Flask extensions:
 
 ```python
@@ -41,15 +41,20 @@
 start          Start watching source changes for dev.
 update         Update Vite and its dependencies, if needed.
 ```
 
 ## Features
 
 - Manages a `vite` directory where you put your front-end source code.
-- Auto-injects vite-generated assets into your HTML pages.
+- Auto-injects vite-generated assets into your HTML pages (if `VITE_AUTO_INSERT` is set in the Flask config).
+- Use `{{ vite_tags() }}` in your Jinja templates otherwise.
+
+## Demo
+
+See the `demo/` directory for a working demo using TailwindCSS.
 
 ## Credits
 
 This project is inspired by the
 [Django-Tailwind](https://github.com/timonweb/django-tailwind) project.
 
 This package was created with
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flask_vite-0.2.4/pyproject.toml` & `flask_vite-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask-vite"
-version = "0.2.4"
+version = "0.3.0"
 homepage = "https://github.com/abilian/flask-vite"
 description = "Flask+Vite integration."
 authors = ["Abilian SAS <contact@abilian.com>"]
 readme = "README.md"
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
@@ -27,14 +27,17 @@
 flask = "^2"
 
 [tool.poetry.dev-dependencies]
 abilian-devtools = "*"
 devtools = "*"
 pyanalyze = "*"
 
+[tool.poetry.group.dev.dependencies]
+honcho = "^1.1.0"
+
 [tool.isort]
 profile = "black"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `flask_vite-0.2.4/src/flask_vite/cli.py` & `flask_vite-0.3.0/src/flask_vite/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,15 +27,18 @@
     source_dir = Path(__file__).parent / "starter"
     dest_dir = Path("vite")
     if dest_dir.exists():
         secho(f"Target directory '{dest_dir}' exists, aborting.", fg="red")
         sys.exit(1)
 
     shutil.copytree(source_dir, dest_dir)
-    secho(f"Vite source directory and starter content installed in '{dest_dir}'.", fg="green")
+    secho(
+        f"Vite source directory and starter content installed in '{dest_dir}'.",
+        fg="green",
+    )
 
 
 @command()
 @with_appcontext
 def install():
     """Install the dependencies using npm."""
     npm_run("install")
```

### Comparing `flask_vite-0.2.4/src/flask_vite/extension.py` & `flask_vite-0.3.0/src/flask_vite/extension.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,17 +22,20 @@
         if "vite" in app.extensions:
             raise RuntimeError(
                 "This extension is already registered on this Flask app."
             )
 
         app.extensions["vite"] = self
 
-        app.after_request(self.after_request)
+        config = app.config
+        if config.get("VITE_AUTO_INSERT", True):
+            app.after_request(self.after_request)
+
         app.route("/_vite/<path:filename>")(self.vite_static)
-        app.template_global("vite_header_tags")(make_tag)
+        app.template_global("vite_tags")(make_tag)
 
     def after_request(self, response: Response):
         if response.status_code != 200:
             return response
 
         mimetype = response.mimetype or ""
         if not mimetype.startswith("text/html"):
```

### Comparing `flask_vite-0.2.4/src/flask_vite/npm.py` & `flask_vite-0.3.0/src/flask_vite/npm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 import subprocess
+from dataclasses import dataclass
 from textwrap import dedent
 
 # Assume npm is in the path for now.
 NPM_BIN_PATH = "npm"
 
 
 class NPMError(Exception):
     pass
 
 
+@dataclass
 class NPM:
-    cwd: str
+    cwd: str = ""
     npm_bin_path: str = NPM_BIN_PATH
 
-    def __init__(self, cwd="", npm_bin_path=None):
-        if npm_bin_path:
-            self.npm_bin_path = npm_bin_path
-        self.cwd = cwd
-
     def run(self, *args):
         try:
             subprocess.run([self.npm_bin_path] + list(args), cwd=self.cwd)
         except OSError:
             msg = """
             It looks like node.js and/or npm is not installed or cannot be found.
             Visit https://nodejs.org to download and install node.js for your system.
```

### Comparing `flask_vite-0.2.4/src/flask_vite/starter/bs.config.js` & `flask_vite-0.3.0/src/flask_vite/starter/bs.config.js`

 * *Files identical despite different names*

### Comparing `flask_vite-0.2.4/src/flask_vite/tags.py` & `flask_vite-0.3.0/src/flask_vite/tags.py`

 * *Files identical despite different names*

### Comparing `flask_vite-0.2.4/tests/test_flask_vite.py` & `flask_vite-0.3.0/tests/test_flask_vite.py`

 * *Files identical despite different names*

### Comparing `flask_vite-0.2.4/PKG-INFO` & `flask_vite-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 Metadata-Version: 2.1
 Name: flask-vite
-Version: 0.2.4
+Version: 0.3.0
 Summary: Flask+Vite integration.
 Home-page: https://github.com/abilian/flask-vite
 Author: Abilian SAS
 Author-email: contact@abilian.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: flask (>=2,<3)
 Description-Content-Type: text/markdown
 
 # Flask-Vite
 
 [![image](https://img.shields.io/pypi/v/flask-tailwind.svg)](https://pypi.python.org/pypi/flask-tailwind)
 
 Plugin to simplify use of Vite from Flask.
 
--   Status: Alpha.
+-   Status: Bêta.
 -   Free software: MIT license
 
 ## Usage
 
 Instantiate the Flask extension as you do for other Flask extensions:
 
 ```python
@@ -63,15 +59,20 @@
 start          Start watching source changes for dev.
 update         Update Vite and its dependencies, if needed.
 ```
 
 ## Features
 
 - Manages a `vite` directory where you put your front-end source code.
-- Auto-injects vite-generated assets into your HTML pages.
+- Auto-injects vite-generated assets into your HTML pages (if `VITE_AUTO_INSERT` is set in the Flask config).
+- Use `{{ vite_tags() }}` in your Jinja templates otherwise.
+
+## Demo
+
+See the `demo/` directory for a working demo using TailwindCSS.
 
 ## Credits
 
 This project is inspired by the
 [Django-Tailwind](https://github.com/timonweb/django-tailwind) project.
 
 This package was created with
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

