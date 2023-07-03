# Comparing `tmp/sphinx-markdown-builder-0.6.1.tar.gz` & `tmp/sphinx-markdown-builder-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-markdown-builder-0.6.1.tar", last modified: Mon Jul  3 22:28:54 2023, max compression
+gzip compressed data, was "sphinx-markdown-builder-0.6.2.tar", last modified: Mon Jul  3 23:22:37 2023, max compression
```

## Comparing `sphinx-markdown-builder-0.6.1.tar` & `sphinx-markdown-builder-0.6.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 22:28:54.782421 sphinx-markdown-builder-0.6.1/
--rw-rw-r--   0 liran     (1000) liran     (1000)     5224 2023-06-22 13:05:55.000000 sphinx-markdown-builder-0.6.1/CODE_OF_CONDUCT.md
--rw-rw-r--   0 liran     (1000) liran     (1000)     2159 2023-06-14 19:10:47.000000 sphinx-markdown-builder-0.6.1/CONTRIBUTING.md
--rw-rw-r--   0 liran     (1000) liran     (1000)     1086 2023-07-03 22:16:52.000000 sphinx-markdown-builder-0.6.1/LICENSE
--rw-rw-r--   0 liran     (1000) liran     (1000)       78 2023-06-22 13:05:55.000000 sphinx-markdown-builder-0.6.1/MANIFEST.in
--rw-rw-r--   0 liran     (1000) liran     (1000)     2802 2023-07-03 22:28:54.782421 sphinx-markdown-builder-0.6.1/PKG-INFO
--rw-rw-r--   0 liran     (1000) liran     (1000)     2089 2023-07-03 22:16:52.000000 sphinx-markdown-builder-0.6.1/README.md
--rw-rw-r--   0 liran     (1000) liran     (1000)     2060 2023-07-03 22:24:28.000000 sphinx-markdown-builder-0.6.1/pyproject.toml
--rw-rw-r--   0 liran     (1000) liran     (1000)       38 2023-07-03 22:28:54.782421 sphinx-markdown-builder-0.6.1/setup.cfg
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 22:28:54.782421 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/
--rw-rw-r--   0 liran     (1000) liran     (1000)      555 2023-07-03 22:16:52.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/__init__.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     2941 2023-07-03 22:00:20.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/builder.py
--rw-rw-r--   0 liran     (1000) liran     (1000)    10540 2023-07-03 22:00:36.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/contexts.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     1786 2023-07-03 22:00:54.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/escape.py
--rw-rw-r--   0 liran     (1000) liran     (1000)    22690 2023-07-03 22:00:09.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/translator.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     1412 2023-07-03 22:00:09.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/writer.py
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 22:28:54.782421 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder.egg-info/
--rw-rw-r--   0 liran     (1000) liran     (1000)     2802 2023-07-03 22:28:54.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder.egg-info/PKG-INFO
--rw-rw-r--   0 liran     (1000) liran     (1000)      567 2023-07-03 22:28:54.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)        1 2023-07-03 22:28:54.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)      111 2023-07-03 22:28:54.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder.egg-info/requires.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)       24 2023-07-03 22:28:54.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder.egg-info/top_level.txt
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 22:28:54.782421 sphinx-markdown-builder-0.6.1/tests/
--rw-rw-r--   0 liran     (1000) liran     (1000)     2598 2023-06-30 11:36:10.000000 sphinx-markdown-builder-0.6.1/tests/test_builder.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     1994 2023-06-30 12:43:08.000000 sphinx-markdown-builder-0.6.1/tests/test_unit.py
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 23:22:37.856375 sphinx-markdown-builder-0.6.2/
+-rw-rw-r--   0 liran     (1000) liran     (1000)     5224 2023-06-22 13:05:55.000000 sphinx-markdown-builder-0.6.2/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2159 2023-06-14 19:10:47.000000 sphinx-markdown-builder-0.6.2/CONTRIBUTING.md
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1086 2023-07-03 23:20:14.000000 sphinx-markdown-builder-0.6.2/LICENSE
+-rw-rw-r--   0 liran     (1000) liran     (1000)       78 2023-06-22 13:05:55.000000 sphinx-markdown-builder-0.6.2/MANIFEST.in
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2802 2023-07-03 23:22:37.856375 sphinx-markdown-builder-0.6.2/PKG-INFO
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2089 2023-07-03 23:20:14.000000 sphinx-markdown-builder-0.6.2/README.md
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2060 2023-07-03 23:20:14.000000 sphinx-markdown-builder-0.6.2/pyproject.toml
+-rw-rw-r--   0 liran     (1000) liran     (1000)       38 2023-07-03 23:22:37.856375 sphinx-markdown-builder-0.6.2/setup.cfg
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 23:22:37.856375 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/
+-rw-rw-r--   0 liran     (1000) liran     (1000)      555 2023-07-03 23:20:14.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/__init__.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2941 2023-07-03 22:00:20.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/builder.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)    10540 2023-07-03 22:00:36.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/contexts.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1786 2023-07-03 22:00:54.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/escape.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)    23049 2023-07-03 23:15:09.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/translator.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1412 2023-07-03 22:00:09.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/writer.py
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 23:22:37.856375 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder.egg-info/
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2802 2023-07-03 23:22:37.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 liran     (1000) liran     (1000)      567 2023-07-03 23:22:37.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)        1 2023-07-03 23:22:37.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)      111 2023-07-03 23:22:37.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder.egg-info/requires.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)       24 2023-07-03 23:22:37.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder.egg-info/top_level.txt
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 23:22:37.856375 sphinx-markdown-builder-0.6.2/tests/
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2598 2023-06-30 11:36:10.000000 sphinx-markdown-builder-0.6.2/tests/test_builder.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1994 2023-06-30 12:43:08.000000 sphinx-markdown-builder-0.6.2/tests/test_unit.py
```

### Comparing `sphinx-markdown-builder-0.6.1/CODE_OF_CONDUCT.md` & `sphinx-markdown-builder-0.6.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.1/CONTRIBUTING.md` & `sphinx-markdown-builder-0.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.1/LICENSE` & `sphinx-markdown-builder-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.1/PKG-INFO` & `sphinx-markdown-builder-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-markdown-builder
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Sphinx extension to add markdown generation support.
 Author-email: Liran Funaro <liran.funaro@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/liran-funaro/sphinx-markdown-builder
 Keywords: sphinx,sphinx-extention,markdown,docs,documentation,builder
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 [![Coverage Status](https://coveralls.io/repos/github/liran-funaro/sphinx-markdown-builder/badge.svg?branch=main)](https://coveralls.io/github/liran-funaro/sphinx-markdown-builder?branch=main)
 
 A Sphinx extension to add markdown generation support.
 
 ## Install
 
 ```sh
-pip3 install sphinx-markdown-builder==0.6.1
+pip3 install sphinx-markdown-builder==0.6.2
 ```
 
 ## Usage
 
 Add the extension to your `conf.py` file:
 ```python
 extensions = [
```

### Comparing `sphinx-markdown-builder-0.6.1/README.md` & `sphinx-markdown-builder-0.6.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![Coverage Status](https://coveralls.io/repos/github/liran-funaro/sphinx-markdown-builder/badge.svg?branch=main)](https://coveralls.io/github/liran-funaro/sphinx-markdown-builder?branch=main)
 
 A Sphinx extension to add markdown generation support.
 
 ## Install
 
 ```sh
-pip3 install sphinx-markdown-builder==0.6.1
+pip3 install sphinx-markdown-builder==0.6.2
 ```
 
 ## Usage
 
 Add the extension to your `conf.py` file:
 ```python
 extensions = [
```

### Comparing `sphinx-markdown-builder-0.6.1/pyproject.toml` & `sphinx-markdown-builder-0.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sphinx-markdown-builder"
-version = "0.6.1"
+version = "0.6.2"
 description = "A Sphinx extension to add markdown generation support."
 readme = "README.md"
 authors = [{ name = "Liran Funaro", email = "liran.funaro@gmail.com" }]
 license = { text = "MIT" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -32,15 +32,15 @@
     "bumpver", "black", "isort", "flake8", "pylint", "pip-tools", "pytest", "pytest-cov", "coveralls",
 ]
 
 [project.urls]
 Homepage = "https://github.com/liran-funaro/sphinx-markdown-builder"
 
 [tool.bumpver]
-current_version = "0.6.1"
+current_version = "0.6.2"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/__init__.py` & `sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 A Sphinx extension to add markdown generation support.
 """
 from sphinx_markdown_builder.builder import MarkdownBuilder
 
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 __docformat__ = "reStructuredText"
 
 
 def setup(app):
     app.add_builder(MarkdownBuilder)
     app.add_config_value("markdown_http_base", "", False)
     app.add_config_value("markdown_uri_doc_suffix", ".md", False)
```

### Comparing `sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/builder.py` & `sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/builder.py`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/contexts.py` & `sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/contexts.py`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/escape.py` & `sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/escape.py`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/translator.py` & `sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,15 +305,21 @@
 
     def depart_comment(self, _node):
         self._pop_context()
         self._pop_status()
 
     @pushing_context
     def visit_paragraph(self, _node):
-        self._push_context(SubContext(SubContextParams(2, 2)))
+        if self.status.list_marker is None:
+            params = SubContextParams(2, 2)
+        else:
+            # Full paragraph spacing inside a list might trigger redundant spacing for some markdown compilers.
+            # So we will add double EOL after the paragraph only if the next element requires it (e.g., code block).
+            params = SubContextParams(2, 1)
+        self._push_context(SubContext(params))
 
     visit_compact_paragraph = visit_paragraph
 
     ################################################################################
     # Line block
     ################################################################################
     # line_block
```

### Comparing `sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/writer.py` & `sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/writer.py`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.1/sphinx_markdown_builder.egg-info/PKG-INFO` & `sphinx-markdown-builder-0.6.2/sphinx_markdown_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-markdown-builder
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Sphinx extension to add markdown generation support.
 Author-email: Liran Funaro <liran.funaro@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/liran-funaro/sphinx-markdown-builder
 Keywords: sphinx,sphinx-extention,markdown,docs,documentation,builder
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 [![Coverage Status](https://coveralls.io/repos/github/liran-funaro/sphinx-markdown-builder/badge.svg?branch=main)](https://coveralls.io/github/liran-funaro/sphinx-markdown-builder?branch=main)
 
 A Sphinx extension to add markdown generation support.
 
 ## Install
 
 ```sh
-pip3 install sphinx-markdown-builder==0.6.1
+pip3 install sphinx-markdown-builder==0.6.2
 ```
 
 ## Usage
 
 Add the extension to your `conf.py` file:
 ```python
 extensions = [
```

### Comparing `sphinx-markdown-builder-0.6.1/sphinx_markdown_builder.egg-info/SOURCES.txt` & `sphinx-markdown-builder-0.6.2/sphinx_markdown_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.1/tests/test_builder.py` & `sphinx-markdown-builder-0.6.2/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.1/tests/test_unit.py` & `sphinx-markdown-builder-0.6.2/tests/test_unit.py`

 * *Files identical despite different names*

