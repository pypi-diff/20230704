# Comparing `tmp/sphinx-markdown-builder-0.6.0.tar.gz` & `tmp/sphinx-markdown-builder-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-markdown-builder-0.6.0.tar", last modified: Sun Jun 25 12:09:52 2023, max compression
+gzip compressed data, was "sphinx-markdown-builder-0.6.1.tar", last modified: Mon Jul  3 22:28:54 2023, max compression
```

## Comparing `sphinx-markdown-builder-0.6.0.tar` & `sphinx-markdown-builder-0.6.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-06-25 12:09:52.125374 sphinx-markdown-builder-0.6.0/
--rw-rw-r--   0 liran     (1000) liran     (1000)     5224 2023-06-22 13:05:55.000000 sphinx-markdown-builder-0.6.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 liran     (1000) liran     (1000)     2159 2023-06-14 19:10:47.000000 sphinx-markdown-builder-0.6.0/CONTRIBUTING.md
--rw-rw-r--   0 liran     (1000) liran     (1000)     1086 2023-06-25 12:07:13.000000 sphinx-markdown-builder-0.6.0/LICENSE
--rw-rw-r--   0 liran     (1000) liran     (1000)       78 2023-06-22 13:05:55.000000 sphinx-markdown-builder-0.6.0/MANIFEST.in
--rw-rw-r--   0 liran     (1000) liran     (1000)     2670 2023-06-25 12:09:52.125374 sphinx-markdown-builder-0.6.0/PKG-INFO
--rw-rw-r--   0 liran     (1000) liran     (1000)     1961 2023-06-25 12:07:13.000000 sphinx-markdown-builder-0.6.0/README.md
--rw-rw-r--   0 liran     (1000) liran     (1000)     1865 2023-06-25 12:07:13.000000 sphinx-markdown-builder-0.6.0/pyproject.toml
--rw-rw-r--   0 liran     (1000) liran     (1000)       38 2023-06-25 12:09:52.125374 sphinx-markdown-builder-0.6.0/setup.cfg
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-06-25 12:09:52.125374 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder/
--rw-rw-r--   0 liran     (1000) liran     (1000)      484 2023-06-25 12:07:13.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder/__init__.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     2813 2023-06-25 11:47:26.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder/builder.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     5547 2023-06-25 11:53:29.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder/contexts.py
--rw-rw-r--   0 liran     (1000) liran     (1000)    23402 2023-06-25 11:56:31.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder/translator.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     1421 2023-06-22 13:05:55.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder/writer.py
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-06-25 12:09:52.125374 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder.egg-info/
--rw-rw-r--   0 liran     (1000) liran     (1000)     2670 2023-06-25 12:09:52.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder.egg-info/PKG-INFO
--rw-rw-r--   0 liran     (1000) liran     (1000)      514 2023-06-25 12:09:52.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)        1 2023-06-25 12:09:52.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)      111 2023-06-25 12:09:52.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder.egg-info/requires.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)       24 2023-06-25 12:09:52.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder.egg-info/top_level.txt
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-06-25 12:09:52.125374 sphinx-markdown-builder-0.6.0/tests/
--rw-rw-r--   0 liran     (1000) liran     (1000)     1345 2023-06-25 11:01:32.000000 sphinx-markdown-builder-0.6.0/tests/test_builder.py
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 22:28:54.782421 sphinx-markdown-builder-0.6.1/
+-rw-rw-r--   0 liran     (1000) liran     (1000)     5224 2023-06-22 13:05:55.000000 sphinx-markdown-builder-0.6.1/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2159 2023-06-14 19:10:47.000000 sphinx-markdown-builder-0.6.1/CONTRIBUTING.md
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1086 2023-07-03 22:16:52.000000 sphinx-markdown-builder-0.6.1/LICENSE
+-rw-rw-r--   0 liran     (1000) liran     (1000)       78 2023-06-22 13:05:55.000000 sphinx-markdown-builder-0.6.1/MANIFEST.in
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2802 2023-07-03 22:28:54.782421 sphinx-markdown-builder-0.6.1/PKG-INFO
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2089 2023-07-03 22:16:52.000000 sphinx-markdown-builder-0.6.1/README.md
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2060 2023-07-03 22:24:28.000000 sphinx-markdown-builder-0.6.1/pyproject.toml
+-rw-rw-r--   0 liran     (1000) liran     (1000)       38 2023-07-03 22:28:54.782421 sphinx-markdown-builder-0.6.1/setup.cfg
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 22:28:54.782421 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/
+-rw-rw-r--   0 liran     (1000) liran     (1000)      555 2023-07-03 22:16:52.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/__init__.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2941 2023-07-03 22:00:20.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/builder.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)    10540 2023-07-03 22:00:36.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/contexts.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1786 2023-07-03 22:00:54.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/escape.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)    22690 2023-07-03 22:00:09.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/translator.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1412 2023-07-03 22:00:09.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/writer.py
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 22:28:54.782421 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder.egg-info/
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2802 2023-07-03 22:28:54.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 liran     (1000) liran     (1000)      567 2023-07-03 22:28:54.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)        1 2023-07-03 22:28:54.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)      111 2023-07-03 22:28:54.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder.egg-info/requires.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)       24 2023-07-03 22:28:54.000000 sphinx-markdown-builder-0.6.1/sphinx_markdown_builder.egg-info/top_level.txt
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 22:28:54.782421 sphinx-markdown-builder-0.6.1/tests/
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2598 2023-06-30 11:36:10.000000 sphinx-markdown-builder-0.6.1/tests/test_builder.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1994 2023-06-30 12:43:08.000000 sphinx-markdown-builder-0.6.1/tests/test_unit.py
```

### Comparing `sphinx-markdown-builder-0.6.0/CODE_OF_CONDUCT.md` & `sphinx-markdown-builder-0.6.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.0/CONTRIBUTING.md` & `sphinx-markdown-builder-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.0/LICENSE` & `sphinx-markdown-builder-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.0/PKG-INFO` & `sphinx-markdown-builder-0.6.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,19 @@
-Metadata-Version: 2.1
-Name: sphinx-markdown-builder
-Version: 0.6.0
-Summary: Sphinx builder that generates markdown files from reStructuredText.
-Author-email: Liran Funaro <liran.funaro@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/liran-funaro/sphinx-markdown-builder
-Keywords: sphinx,markdown,docs,documentation,builder
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # sphinx-markdown-builder
 
 [![Coverage Status](https://coveralls.io/repos/github/liran-funaro/sphinx-markdown-builder/badge.svg?branch=main)](https://coveralls.io/github/liran-funaro/sphinx-markdown-builder?branch=main)
 
-Sphinx builder that generates markdown files from reStructuredText.
+A Sphinx extension to add markdown generation support.
 
 ## Install
 
 ```sh
-pip3 install sphinx-markdown-builder==0.6.0
+pip3 install sphinx-markdown-builder==0.6.1
 ```
 
-
 ## Usage
 
 Add the extension to your `conf.py` file:
 ```python
 extensions = [
     ...,
     "sphinx_markdown_builder",
@@ -45,29 +26,38 @@
 sphinx-build -M markdown ./docs ./build
 ```
 
 ## Configurations
 
 You can add the following configurations to your `conf.py` file:
 
+* `markdown_anchor_sections`/`markdown_anchor_signatures`: If set to `True`, 
+  then anchors will be added before each section/function/class signature. 
+  This allows references to a specific anchor in the document.
+* `markdown_docinfo`: Adds metadata to the top of each document containing author, copyright, and version.
 * `markdown_http_base`: If set, all references will link to this prefix address
 * `markdown_uri_doc_suffix`: If set, all references will link to documents with this suffix.
-* `markdown_anchor_sections`/`markdown_anchor_signatures`: If set to `True`, then anchors will be added before each section/function/class signature. 
- This allows references to a specific anchor in the document.
 
 For example, if your `conf.py` file have the following configuration:
+
 ```python
 markdown_http_base = "https://your-domain.com/docs"
 markdown_uri_doc_suffix = ".html"
 ```
 
 Then a reference to `your-doc-name#your-header` will be substituted with `https://your-domain.com/docs/your-doc-name.html#your-header`. 
 
 ## Credits
-This project forked from [
-sphinx-markdown-builder](https://github.com/clayrisser/sphinx-markdown-builder), which was developed by [Clay Risser](https://github.com/clayrisser) under the [MIT](https://github.com/clayrisser/sphinx-markdown-builder/blob/master/LICENSE) license.
+This project forked from [clayrisser/sphinx-markdown-builder], which was developed by [Clay Risser] under the [MIT] license.
 
-The original implementation was based on [doctree2md](https://github.com/matthew-brett/nb2plots/blob/master/nb2plots/doctree2md.py) by [Matthew Brett](https://github.com/matthew-brett) under the [BSD-2](https://github.com/matthew-brett/nb2plots/blob/main/LICENSE) license.
+The original implementation was based on [doctree2md] by [Matthew Brett] under the [BSD-2] license.
 
 ## License
 
-[MIT](LICENSE)
+[MIT]
+
+[clayrisser/sphinx-markdown-builder]: https://github.com/clayrisser/sphinx-markdown-builder
+[Clay Risser]: https://github.com/clayrisser
+[doctree2md]: https://github.com/matthew-brett/nb2plots/blob/master/nb2plots/doctree2md.py
+[Matthew Brett]: https://github.com/matthew-brett
+[MIT]: LICENSE
+[BSD-2]: https://github.com/matthew-brett/nb2plots/blob/main/LICENSE
```

### Comparing `sphinx-markdown-builder-0.6.0/pyproject.toml` & `sphinx-markdown-builder-0.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sphinx-markdown-builder"
-version = "0.6.0"
-description = "Sphinx builder that generates markdown files from reStructuredText."
+version = "0.6.1"
+description = "A Sphinx extension to add markdown generation support."
 readme = "README.md"
 authors = [{ name = "Liran Funaro", email = "liran.funaro@gmail.com" }]
 license = { text = "MIT" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
-keywords = ["sphinx", "markdown", "docs", "documentation", "builder"]
+keywords = ["sphinx", "sphinx-extention", "markdown", "docs", "documentation", "builder"]
 dependencies = ["sphinx>=2.2.0", "tabulate", "docutils"]
 requires-python = ">=3.7"
 
 [tool.poetry.plugins] # Optional super table
 
 [tool.poetry.plugins."sphinx.builders"]
 "markdown" = "sphinx_markdown_builder"
@@ -32,15 +32,15 @@
     "bumpver", "black", "isort", "flake8", "pylint", "pip-tools", "pytest", "pytest-cov", "coveralls",
 ]
 
 [project.urls]
 Homepage = "https://github.com/liran-funaro/sphinx-markdown-builder"
 
 [tool.bumpver]
-current_version = "0.6.0"
+current_version = "0.6.1"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
@@ -57,14 +57,18 @@
 "sphinx_markdown_builder/__init__.py" = [
     "^__version__ = \"{version}\"$",
 ]
 "tests/source/conf.py" = [
     "^version = \"{version}\"$",
     "Copyright (c) 2023-YYYY, Liran Funaro.",
 ]
+"tests/expected/overrides-auto-summery.md" = [
+    "<meta name=\"version\" content=\"{version}\"/>",
+    "<meta name=\"copyright\" content=\"Copyright (c) 2023-YYYY, Liran Funaro.\"/>",
+]
 
 [tool.black]
 line-length = 120
 
 [tool.pylint.format]
 max-line-length = 120
 max-args = 6
```

### Comparing `sphinx-markdown-builder-0.6.0/sphinx_markdown_builder/builder.py` & `sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
-docutils XML to markdown translator.
+Custom docutils builder for markdown.
 """
 import os
+from contextlib import contextmanager
 from typing import Set
 
 from docutils import nodes
 from docutils.io import StringOutput
 from sphinx.application import Sphinx
 from sphinx.builders import Builder
 from sphinx.environment import BuildEnvironment
@@ -15,20 +16,25 @@
 
 from sphinx_markdown_builder.translator import MarkdownTranslator
 from sphinx_markdown_builder.writer import MarkdownWriter
 
 logger = logging.getLogger(__name__)
 
 
-def get_mod_time_if_exists(file_path):
+@contextmanager
+def io_handler(file_path: str):
     try:
+        yield
+    except (IOError, OSError) as err:
+        logger.warning(__("error accessing file %s: %s"), file_path, err)
+
+
+def get_mod_time_if_exists(file_path):
+    with io_handler(file_path):
         return os.path.getmtime(file_path)
-    except OSError as err:
-        logger.warning(__("error reading file %s: %s"), file_path, err)
-        return 0
 
 
 class MarkdownBuilder(Builder):
     name = "markdown"
     format = "markdown"
     epilog = __("The markdown files are in %(outdir)s.")
 
@@ -48,17 +54,18 @@
 
     def get_outdated_docs(self):
         for doc_name in self.env.found_docs:
             if doc_name not in self.env.all_docs:
                 yield doc_name
                 continue
             target_name = os.path.join(self.outdir, doc_name + self.out_suffix)
+            source_name = self.env.doc2path(doc_name)
             target_mtime = get_mod_time_if_exists(target_name)
-            src_mtime = get_mod_time_if_exists(self.env.doc2path(doc_name))
-            if src_mtime > target_mtime:
+            source_mtime = get_mod_time_if_exists(source_name)
+            if source_mtime is None or target_mtime is None or source_mtime > target_mtime:
                 yield doc_name
 
     def get_target_uri(self, docname: str, typ: str = None):
         """
         Returns the target file name.
         By default, we link to the currently generated markdown files.
         But, we also support linking to external document (e.g., an html web page).
@@ -72,12 +79,10 @@
         self.current_doc_name = docname
         self.sec_numbers = self.env.toc_secnumbers.get(docname, {})
         destination = StringOutput(encoding="utf-8")
         self.writer.write(doctree, destination)
         out_filename = os.path.join(self.outdir, f"{os_path(docname)}{self.out_suffix}")
         ensuredir(os.path.dirname(out_filename))
 
-        try:
+        with io_handler(out_filename):
             with open(out_filename, "w", encoding="utf-8") as file:
                 file.write(self.writer.output)
-        except (IOError, OSError) as err:
-            logger.warning(__("error writing file %s: %s"), out_filename, err)
```

### Comparing `sphinx-markdown-builder-0.6.0/sphinx_markdown_builder/translator.py` & `sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/translator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,96 +1,82 @@
 """
-docutils XML to markdown translator.
+Custom docutils translator for markdown.
+
+See Also
+========
+The Docutils Document Tree:
+https://docutils.sourceforge.io/docs/ref/doctree.html
+
+reStructuredText Markup Specification/Directives:
+https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html
+https://docutils.sourceforge.net/docs/ref/rst/directives.html
+
+Doctree node classes added by Sphinx:
+https://www.sphinx-doc.org/en/master/extdev/nodes.html
+
+reStructuredText Primer:
+https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html
+
+HTML5 translator (example):
+https://github.com/sphinx-doc/sphinx/blob/master/sphinx/writers/html5.py
+
+Base HTML5 translator (example):
+https://github.com/docutils/docutils/blob/master/docutils/docutils/writers/html5_polyglot/__init__.py
 """
-import os
+import dataclasses
 import posixpath
 import re
-from textwrap import dedent
-from typing import List, Dict, Union, TYPE_CHECKING
+from typing import TYPE_CHECKING, Callable, Dict, List, Optional, Union
 
 from docutils import languages, nodes
 from sphinx.util.docutils import SphinxTranslator
 
 from sphinx_markdown_builder.contexts import (
-    WrappedContext,
+    CommaSeparatedContext,
+    ContextStatus,
+    DocInfoContext,
     IndentContext,
+    ItalicContext,
+    ListMarker,
+    MetaContext,
+    PushContext,
+    StrongContext,
     SubContext,
+    SubContextParams,
+    SubscriptContext,
     TableContext,
+    TitleContext,
     UniqueString,
-    CommaSeparatedContext,
+    WrappedContext,
 )
+from sphinx_markdown_builder.escape import escape_html_quote, escape_markdown_chars
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from sphinx_markdown_builder import MarkdownBuilder
 
-# Characters that should be escaped in Markdown:
-# ----------------------------------------------
-# Emphasis chars: * and _
-#   Emphasis char prefix/postfix should have a non-space char to its right/left.
-#   _ prefix/postfix must have a space char to its left/right (or beginning/end of the text).
-#   We cannot make the destination between prefix/postfix in regular expression, so we will enforce both for all.
-# Quote/Title: > and #
-#   Should only precede by space chars in the line.
-# Block char: `
-#   One ` only requires not to have double line break in between
-#   Double `` seems to be ignored
-#   Three ``` must be at the beginning of the line
-# Title: ----
-#   A line that only have - or =
-#   No spaces between them
-# Horizontal line: ----
-#   A line that only have 3 consecutive -, _, or * or more.
-#   Precedes an empty line or beginng of text.
-# Links: [text](link)
-# Images: ![alt](link)
-# Lists: +, -, *, 1.
-# Tables: |
-# Anything starting with 4 spaces is considered a block.
-#   Should add force spaces (\ ) to avoid it.
-# Escape char: \
-#   Should be followed by:
-#   Character Name
-#   \         backslash
-#   `         backtick (see also escaping backticks in code)
-#   *         asterisk
-#   _         underscore
-#   { }       curly braces
-#   [ ]       brackets
-#   < >       angle brackets
-#   ( )       parentheses
-#   #         pound sign
-#   +         plus sign
-#   -         minus sign (hyphen)
-#   .         dot
-#   !         exclamation mark
-#   |         pipe (see also escaping pipe in tables)
-ESCAPE_RE = re.compile(r"([\\*`]|(?:^|(?<=\s|_))_)", re.M)
-
-DOC_SECTION_ORDER = "head", "body", "foot"
-
 VISIT_DEPART_PATTERN = re.compile("(visit|depart)_(.+)")
-
-
-def escape_chars(txt: str):
-    # Escape (some) characters with special meaning for Markdown
-    return ESCAPE_RE.sub(r"\\\1", txt)
-
-
 SKIP = UniqueString("skip")
 
-PREDEFINED_ELEMENTS = dict(  # pylint: disable=use-dict-literal
+DOC_INFO_FIELDS = "author", "contact", "copyright", "date", "organization", "revision", "status", "version"
+
+PREDEFINED_ELEMENTS: Dict[str, Union[PushContext, SKIP, None]] = dict(  # pylint: disable=use-dict-literal
     # Doctree elements for which Markdown element is <prefix><content><suffix>
-    emphasis=(WrappedContext, "*"),  # _ is more restrictive
-    strong=(WrappedContext, "**"),  # _ is more restrictive
-    subscript=(WrappedContext, "<sub>", "</sub>"),
-    superscript=(WrappedContext, "<sup>", "</sup>"),
-    desc_annotation=(WrappedContext, "*"),  # _ is more restrictive
-    field_name=(WrappedContext, "**"),  # e.g 'returns', 'parameters'
-    literal_strong=(WrappedContext, "**"),
-    literal_emphasis=(WrappedContext, "*"),
+    emphasis=ItalicContext,
+    strong=StrongContext,
+    subscript=SubscriptContext,
+    superscript=SubscriptContext,
+    desc_annotation=ItalicContext,
+    literal_strong=StrongContext,
+    literal_emphasis=ItalicContext,
+    field_name=StrongContext,  # e.g 'returns', 'parameters'
+    # Doc info elements
+    docinfo=DocInfoContext,
+    docinfo_item=DocInfoContext,
+    **dict.fromkeys(DOC_INFO_FIELDS, DocInfoContext),
+    authors=None,  # not used: visit_author is called anyway for each author.
     # Doctree elements to skip subtree
     autosummary_toc=SKIP,
     nbplot_epilogue=SKIP,
     nbplot_not_rendered=SKIP,
     nbplot_container=SKIP,
     code_links=SKIP,
     index=SKIP,
@@ -103,360 +89,356 @@
     definition_list=None,
     definition_list_item=None,
     term=None,
     field_list_item=None,
     mpl_hint=None,
     pending_xref=None,
     compound=None,
-    line=None,
-    line_block=None,
     desc_addname=None,  # module pre-roll for class/method
     desc_content=None,  # the description of the class/method
     desc_name=None,  # name of the class/method
     title_reference=None,
     autosummary_table=None,  # Sphinx autosummary
     # See https://www.sphinx-doc.org/en/master/usage/extensions/autosummary.html.
     # Ignored table elements
     raw=None,
     tabular_col_spec=None,
     colspec=None,
     tgroup=None,
 )
 
 
-class MarkdownTranslator(SphinxTranslator):  # pylint: disable=too-many-instance-attributes,too-many-public-methods
+def pushing_context(method):
+    """Marks method as pushing context"""
+    match = VISIT_DEPART_PATTERN.fullmatch(method.__name__)
+    assert match is not None
+    state, _ = match.groups()
+    assert state == "visit"
+    setattr(method, "__pushing_context__", True)
+    return method
+
+
+class MarkdownTranslator(SphinxTranslator):  # pylint: disable=too-many-public-methods
     def __init__(self, document: nodes.document, builder: "MarkdownBuilder"):
         super().__init__(document, builder)
         self.builder: "MarkdownBuilder" = builder
+        # noinspection PyUnresolvedReferences
         self.language = languages.get_language(self.settings.language_code, document.reporter)
         # Warn only once per writer about unsupported elements
         self._warned = set()
-        # Lookup table to get section list from name (default is ordered dict)
-        # FIFO Sub context allow us to handle unique cases when post-processing is required.
-        self._sections: Dict[str, List[SubContext]] = dict.fromkeys(DOC_SECTION_ORDER, None)
-
-        # Current section heading level during writing
-        self.section_level = 0
-
-        # Flag indicating we are processing docinfo items
-        self._in_docinfo = False
-
-        # Flag for whether to escape characters
-        self._escape_text = True
 
-        self.list_context: List[Union[str, int]] = []
+        # FIFO Sub context allow us to handle unique cases when post-processing is required
+        self._ctx_queue: List[SubContext] = [SubContext()]
+        self._doc_info: SubContext = SubContext()
+        self._status_queue: List[ContextStatus] = [ContextStatus()]
+
+        if self.config.markdown_docinfo:
+            self._add_doc_info_from_config()
+
+    def _add_doc_info_from_config(self):
+        for key in DOC_INFO_FIELDS:
+            value = getattr(self.config, key, "")
+            if isinstance(value, str):
+                self._push_context(MetaContext(key))
+                self.ctx.add(value)
+                self._pop_context()
+
+    @property
+    def ctx(self) -> SubContext:
+        return self._ctx_queue[-1]
 
-        # Saves the current descriptor type
-        self.desc_context: List[str] = []
+    def _push_context(self, ctx: SubContext):
+        self._ctx_queue.append(ctx)
 
-        # Reset attributes modified by reading
-        self.reset()
-
-    def reset(self):
-        """Initialize object for fresh read."""
-        for k in DOC_SECTION_ORDER:
-            self._sections[k] = [SubContext()]
-
-        self.section_level = 0
-        self._in_docinfo = False
-        self._escape_text = True
-        self.list_context = []
-        self.desc_context = []
+    def _pop_context(self, _node=None, count=1):
+        for _ in range(count):
+            if len(self._ctx_queue) <= 1:
+                break
 
-    def ctx(self, section="body") -> SubContext:
-        return self._sections[section][-1]
+            last_ctx = self._ctx_queue.pop()
+            ctx = self.ctx if last_ctx.params.target == "body" else self._doc_info
+            ctx.add(last_ctx.make(), last_ctx.params.prefix_eol, last_ctx.params.suffix_eol)
+
+    def _push_box(self, title: str):
+        self.add(f"#### {title}", prefix_eol=2)
+        self._push_context(SubContext(SubContextParams(1, 2)))
+
+    @property
+    def status(self) -> ContextStatus:
+        return self._status_queue[-1]
+
+    def _push_status(self, **changes):
+        cur_status = self.status
+        self._status_queue.append(dataclasses.replace(cur_status, **changes))
+
+    def _pop_status(self, _node=None, count=1):
+        count = min(len(self._status_queue) - 1, count)
+        self._status_queue = self._status_queue[:-count]
 
     def astext(self):
         """Return the final formatted document as a string."""
-        for section in self._sections:
-            self._pop_context(count=2**31, section=section)
-
-        parts = (self.ctx(section).make().strip() for section in DOC_SECTION_ORDER)
-        return "\n\n".join(parts).strip() + "\n"
+        self._pop_context(count=2**31)
+        assert len(self._ctx_queue) == 1
 
-    def add(self, value: str, section="body"):
-        """
-        Add `value` to `section`.
+        ctx = SubContext()
+        for sub_ctx in (self._doc_info, self._ctx_queue[0]):
+            ctx.add(sub_ctx.make().strip(), prefix_eol=2, suffix_eol=1)
+        ctx.force_eol(1)
+        return ctx.make()
+
+    def add(self, value: str, prefix_eol: int = 0, suffix_eol: int = 0):
+        """See `SubContext.add()`"""
+        self.ctx.add(value, prefix_eol, suffix_eol)
 
-        Parameters
-        ----------
-        value : str
-            String to add to output document
-        section : {'body', 'head', 'foot'}, optional
-            Section of document that generated text should be appended to.
-        """
-        self.ctx(section).add(value)
-
-    def ensure_eol(self, count=1, section="body"):
+    def ensure_eol(self, count=1):
         """Ensure the last line in current base is terminated by X new lines."""
-        self.ctx(section).ensure_eol(count)
-
-    def _push_context(self, ctx: SubContext, section="body"):
-        self._sections[section].append(ctx)
-
-    def _pop_context(self, _node=None, count=1, section="body"):
-        for _ in range(count):
-            if len(self._sections[section]) <= 1:
-                break
-            content = self._sections[section].pop().make()
-            self.add(content)
-
-    def _start_level(self, prefix: str):
-        """Create a new IndentLevel with `prefix` and `first_prefix`"""
-        self._push_context(IndentContext(prefix))
-
-    _finish_level = _pop_context
+        self.ctx.ensure_eol(count)
 
     def _pass(self, _node=None):
         pass
 
     def _skip(self, _node=None):
         raise nodes.SkipNode
 
     def _has_attr(self, item):
         try:
             super().__getattribute__(item)
             return True
         except AttributeError:
             return False
 
+    def _get_attr(self, item, default=None):
+        try:
+            return super().__getattribute__(item)
+        except AttributeError:
+            return default
+
     def __getattribute__(self, item):
-        # First try to get an existing attribute
+        """Uses some predefined rules to reduce the visit/depart method clutter in the class"""
         try:
+            # First try to get an existing attribute
             return super().__getattribute__(item)
         except AttributeError as ex:
-            exp = ex
+            predefined_method = self._find_predefined_method(item)
+            if predefined_method is not None:
+                return predefined_method
+            raise ex
 
+    def _find_predefined_method(self, item) -> Optional[Callable]:  # pylint: disable=too-many-return-statements
         match = VISIT_DEPART_PATTERN.fullmatch(item)
         if match is None:
-            raise exp
-
+            # We only care about visit/depart methods
+            return None
         state, element = match.groups()
-        if element in PREDEFINED_ELEMENTS:
-            action = PREDEFINED_ELEMENTS[element]
-            if action is None:
-                return self._pass
-            if action is SKIP:
-                return self._skip
-            if isinstance(action, (list, tuple)) and isinstance(action[0], type) and issubclass(action[0], SubContext):
-                if state == "visit":
-                    sub_context, *args = action
-                    return lambda _node: self._push_context(sub_context(*args))
+
+        action = PREDEFINED_ELEMENTS.get(element, "__undefined__")
+        if action is None:
+            return self._pass
+        if action is SKIP:
+            return self._skip
+        if isinstance(action, PushContext):
+            if state == "visit":
+                return lambda node: self._push_context(action.create(node, element))
+            return self._pop_context
+
+        # If the visit method is marked as pushing, then pop the context
+        if state == "depart":
+            visit_method = self._get_attr(f"visit_{element}", None)
+            is_pushing = getattr(visit_method, "__pushing_context__", False)
+            if is_pushing:
                 return self._pop_context
 
-        # If one of the handlers is defined, automatically add the other
+        # If one of the handlers is defined, automatically add the other as an empty handler
         if self._has_attr(f"visit_{element}") or self._has_attr(f"depart_{element}"):
             return self._pass
 
-        raise exp
+        return None
+
+    def unknown_visit(self, node):
+        """Warn once per instance for unsupported nodes."""
+        node_type = node.__class__.__name__
+        if node_type not in self._warned:
+            super().unknown_visit(node)
+            self._warned.add(node_type)
+        raise nodes.SkipNode
 
     ################################################################################
     # visit/depart handlers
     ################################################################################
 
+    @pushing_context
     def visit_warning(self, _node):
         """Sphinx warning directive."""
-        self.add("**WARNING**: ")
+        self._push_box("WARNING")
 
+    @pushing_context
     def visit_note(self, _node):
         """Sphinx note directive."""
-        self.add("**NOTE**: ")
+        self._push_box("NOTE")
 
+    @pushing_context
     def visit_seealso(self, _node):
-        self.add("**SEE ALSO**: ")
+        """Sphinx see also directive."""
+        self._push_box("SEE ALSO")
 
+    @pushing_context
     def visit_attention(self, _node):
-        self.add("**ATTENTION**: ")
+        self._push_box("ATTENTION")
 
     def visit_image(self, node):
         """Image directive."""
-        uri = node.attributes["uri"]
-        doc_folder = os.path.dirname(self.builder.current_doc_name)
-        if uri.startswith(doc_folder):
-            # drop docname prefix
-            doc_folder_len = len(doc_folder)
-            uri = uri[doc_folder_len:]
-            if uri.startswith("/"):
-                uri = "." + uri
-
+        uri = node["uri"]
         alt = node.attributes.get("alt", "image")
         # We don't need to add EOL before/after the image.
         # It will be handled by the visit/depart handlers of the paragraph.
         self.add(f"![{alt}]({uri})")
 
     # noinspection PyPep8Naming
     def visit_Text(self, node):  # pylint: disable=invalid-name
         text = node.astext().replace("\r", "")
-        if self._escape_text:
-            text = escape_chars(text)
+        if self.status.escape_text:
+            text = escape_markdown_chars(text)
         self.add(text)
 
     def visit_comment(self, _node):
-        self.ensure_eol()
-        self._escape_text = False
-        self._push_context(WrappedContext("<!-- ", " -->"))
+        self._push_status(escape_text=False)
+        self._push_context(WrappedContext("<!-- ", " -->", params=SubContextParams(1)))
 
     def depart_comment(self, _node):
         self._pop_context()
-        self._escape_text = True
+        self._pop_status()
 
+    @pushing_context
     def visit_paragraph(self, _node):
-        self.ensure_eol(2)
+        self._push_context(SubContext(SubContextParams(2, 2)))
 
-    depart_paragraph = visit_paragraph
     visit_compact_paragraph = visit_paragraph
-    depart_compact_paragraph = depart_paragraph
 
-    def visit_docinfo(self, _node):
-        self._in_docinfo = True
+    ################################################################################
+    # Line block
+    ################################################################################
+    # line_block
+    #   line
+    #   line
+    #   line
+    ################################################################################
+
+    @pushing_context
+    def visit_line_block(self, _node):
+        self._push_context(SubContext(SubContextParams(1, 1)))
+
+    @pushing_context
+    def visit_line(self, _node):
+        self._push_context(SubContext(SubContextParams(1, 1)))
 
-    def depart_docinfo(self, _node):
-        self._in_docinfo = False
+    def depart_line(self, _node):
+        self._pop_context()
+        self.add("<br/>", prefix_eol=1, suffix_eol=1)
 
-    def _process_docinfo_item(self, node):
-        """Called explicitly from methods in this class."""
-        self.ensure_eol(1, section="head")
-        self.add(f"% {node.astext()}\n", section="head")
-        raise nodes.SkipNode
+    ################################################################################
+    # Definition
+    ################################################################################
+    # definition_list
+    #   definition_list_item
+    #     term
+    #     definition
+    #       paragraph
+    ################################################################################
 
+    @pushing_context
     def visit_definition(self, _node):
-        self.ensure_eol(2)
-        self._start_level("    ")
-
-    depart_definition = _finish_level
+        self._push_context(
+            IndentContext(": ", only_first=True, support_multi_line_break=True, params=SubContextParams(1, 2))
+        )
 
     def visit_math_block(self, _node):
-        # docutils math block
-        self._escape_text = False
-        self.ensure_eol()
-        self.add("$$")
-        self.ensure_eol()
+        """docutils math block"""
+        self._push_status(escape_text=False)
+        self.add("$$", prefix_eol=1, suffix_eol=1)
 
     def depart_math_block(self, _node):
-        self._escape_text = True
-        self.ensure_eol()
-        self.add("$$")
-        self.ensure_eol(2)
-
-    def visit_displaymath(self, node):
-        """sphinx math blocks become displaymath"""
-        self.ensure_eol()
-        latex = node["latex"]
-        self.add(f"$$\n{latex}\n$$")
-        self.ensure_eol(2)
-        raise nodes.SkipNode
-
-    def visit_math(self, node):
-        """sphinx math node has 'latex' attribute, docutils does not"""
-        if "latex" in node:  # sphinx math node
-            latex = node["latex"]
-            self.add(f"${latex}$")
-            raise nodes.SkipNode
-        # docutils math node
-        self._escape_text = False
+        """docutils math block"""
+        self.add("$$", prefix_eol=1, suffix_eol=2)
+        self._pop_status()
+
+    def visit_math(self, _node):
+        """docutils math node"""
+        self._push_status(escape_text=False)
         self.add("$")
 
     def depart_math(self, _node):
-        # sphinx node skipped in visit, only docutils gets here
-        self._escape_text = True
+        """docutils math node"""
         self.add("$")
+        self._pop_status()
 
     def visit_literal(self, _node):
-        self._escape_text = False
+        self._push_status(escape_text=False)
         self.add("`")
 
     def depart_literal(self, _node):
         self.add("`")
-        self._escape_text = True
+        self._pop_status()
 
     def visit_literal_block(self, node):
-        self._escape_text = False
+        self._push_status(escape_text=False)
         code_type = node["classes"][1] if "code" in node["classes"] else ""
         if "language" in node:
             code_type = node["language"]
-        self.ensure_eol()
-        self.add("```" + code_type)
-        self.ensure_eol()
+        self.add(f"```{code_type}", prefix_eol=1, suffix_eol=1)
 
     def depart_literal_block(self, _node):
-        self._escape_text = True
-        self.ensure_eol()
-        self.add("```")
-        self.ensure_eol(2)
+        self.add("```", prefix_eol=1, suffix_eol=2)
+        self._pop_status()
 
     def visit_doctest_block(self, _node):
-        self._escape_text = False
-        self.ensure_eol()
-        self.add("```python")
-        self.ensure_eol()
+        self._push_status(escape_text=False)
+        self.add("```pycon", prefix_eol=1, suffix_eol=1)
 
     depart_doctest_block = depart_literal_block
 
+    @pushing_context
     def visit_block_quote(self, _node):
-        self.ensure_eol()
-        self._start_level("> ")
-
-    depart_block_quote = _finish_level
+        self._push_context(IndentContext("> "))
 
     def visit_problematic(self, node):
-        self.ensure_eol(2)
-        self.add(f"```\n{node.astext()}\n```")
-        self.ensure_eol(2)
-        raise nodes.SkipNode
-
-    def visit_system_message(self, node):
-        if node["level"] < self.document.reporter.report_level:
-            # Level is too low to display
-            raise nodes.SkipNode
-        line = node["line"] if node.hasattr("line") else ""
-        line = f", line {line}"
-        source = node["source"]
-        self.ensure_eol(2)
-        self.add(f"```System Message: {source}:{line}\n\n{node.astext()}\n```")
-        self.ensure_eol(2)
+        self.add(f"```\n{node.astext()}\n```", prefix_eol=2, suffix_eol=2)
         raise nodes.SkipNode
 
     def visit_section(self, node):
+        self.ensure_eol(2)
         if self.config.markdown_anchor_sections:
             for anchor in node.get("ids", []):
                 self._add_anchor(anchor)
 
-        self.section_level += 1
-        self.ensure_eol(2)
+        self._push_status(section_level=self.status.section_level + 1)
 
     def depart_section(self, _node):
-        self.section_level -= 1
+        self._pop_status()
 
+    @pushing_context
     def visit_title(self, _node):
-        self.ensure_eol(2)
-        self.add((self.section_level * "#") + " ")
-
-    def depart_title(self, _node):
-        self.ensure_eol(2)
+        self._push_context(TitleContext(self.status.section_level))
 
+    @pushing_context
     def visit_subtitle(self, _node):
-        self.ensure_eol(2)
-        self.add((self.section_level + 2) * "#" + " ")
-
-    depart_subtitle = depart_title
+        """
+        Docutils does not promote subtitles, so this might never be called.
+        However, we keep it here in case some future version will change this behaviour.
+        """
+        self._push_context(TitleContext(self.status.section_level + 1))  # pragma: no cover
 
+    @pushing_context
     def visit_rubric(self, _node):
-        """Sphinx Rubric, a heading without relation to the document sectioning
-        https://docutils.sourceforge.net/docs/ref/rst/directives.html#rubric."""
-        self.ensure_eol(2)
-        self.add("### ")
-
-    depart_rubric = depart_title
+        """Sphinx Rubric, a heading without relation to the document sectioning"""
+        self._push_context(TitleContext(3))
 
     def visit_transition(self, _node):
-        # Simply replace a transition by a horizontal rule.
-        # Could use three or more '*', '_' or '-'.
-        self.ensure_eol(2)
-        self.add("---")
-        self.ensure_eol(1)
+        """Simply replace a transition by a horizontal rule."""
+        # Can use three or more '*', '_' or '-'.
+        self.add("---", prefix_eol=2, suffix_eol=1)
         raise nodes.SkipNode
 
     def _adjust_url(self, url: str):
         """Replace `refuri` in reference with HTTP address, if possible"""
         if not self.config.markdown_http_base:
             return url
 
@@ -470,70 +452,93 @@
                 url = posixpath.normpath(f"{this_dir}/{url}")
         return f"{self.config.markdown_http_base}/{url}"
 
     def _fetch_ref_uri(self, node):
         uri = node.get("refuri", "")
 
         # Do not modify external URL in any way
-        if not node.get("internal", False):
+        if not node.get("internal", self.status.default_ref_internal):
             return uri
 
         uri = self._adjust_url(uri)
 
         # Whatever the URL is, add the anchor to it
         ref_id = node.get("refid", None)
         if ref_id is not None:
             uri = f"#{ref_id}"
 
         return uri
 
+    @pushing_context
     def visit_reference(self, node):
         url = self._fetch_ref_uri(node)
         self._push_context(WrappedContext("[", f"]({url})"))
 
-    depart_reference = _pop_context
-
+    @pushing_context
     def visit_download_reference(self, node):
-        filename = self._adjust_url(node.get("filename", ""))
-        self._push_context(WrappedContext("[", f"]({filename})"))
-
-    depart_download_reference = _pop_context
+        reftarget = self._adjust_url(node.get("reftarget", ""))
+        self._push_context(WrappedContext("[", f"]({reftarget})"))
 
     def _add_anchor(self, anchor: str):
-        self._escape_text = False
-        self.ensure_eol()
-        self.add(f'<a id="{anchor}"></a>')
-        self.ensure_eol()
-        self._escape_text = True
+        content = f'<a id="{escape_html_quote(anchor)}"></a>'
+        # Prevent adding the same anchor twice in the same context
+        if content not in self.ctx.content:
+            self.add(content, prefix_eol=2, suffix_eol=1)
 
     def visit_target(self, node):
         ref_id = node.get("refid", None)
         if ref_id is None:
             return
         self._add_anchor(ref_id)
 
-    def visit_only(self, node):
-        if node["expr"] != "markdown":
-            raise nodes.SkipNode
-        self.add(dedent(node.astext()))
+    def visit_topic(self, _node):
+        self._push_status(default_ref_internal=True, section_level=5)
+        self._push_context(IndentContext("> ", empty=True))
+
+    def depart_topic(self, _node):
+        self._pop_status()
+        self._pop_context()
+
+    ################################################################################
+    # lists
+    ################################################################################
+    # enumerated_list/bullet_list
+    #     list_item
+    #       paragraph (optional)
+    ###############################################################################
+
+    def _start_list(self, marker: Union[int, str]):
         self.ensure_eol()
+        if isinstance(marker, str) and marker[-1] != " ":
+            marker += " "
+        self._push_status(list_marker=ListMarker(marker))
 
-    def unknown_visit(self, node):
-        """Warn once per instance for unsupported nodes.
-        Intercept docinfo items if in docinfo block.
-        """
-        if self._in_docinfo:
-            self._process_docinfo_item(node)
-            return
-        # We really don't know this node type, warn once per node type
-        node_type = node.__class__.__name__
-        if node_type not in self._warned:
-            self.document.reporter.warning("The " + node_type + " element not yet supported in Markdown.")
-            self._warned.add(node_type)
-        raise nodes.SkipNode
+    def _end_list(self, _node=None):
+        self._pop_status()
+        # We need two line breaks to make sure the next paragraph will not merge into the list
+        self.ensure_eol(2)
+
+    def _start_list_item(self, _node=None):
+        marker = self.status.list_marker
+        marker.inc()
+        self._push_context(IndentContext(marker, only_first=True, params=SubContextParams(1, 1)))
+
+    _end_list_item = _pop_context
+
+    def visit_enumerated_list(self, _node):
+        self._start_list(0)
+
+    depart_enumerated_list = _end_list
+
+    def visit_bullet_list(self, node):
+        self._start_list(node.attributes.get("bullet", "*"))
+
+    depart_bullet_list = _end_list
+    visit_list_item = _start_list_item
+    depart_list_item = _end_list_item
 
     ################################################################################
     # desc
     ################################################################################
     # desc (desctype: {function, class, method, etc.)
     #   desc_signature
     #     desc_name
@@ -544,94 +549,74 @@
     #     field_list
     #       field
     #         field_name (e.g 'returns/parameters/raises')
     #         field_body
     ################################################################################
 
     def visit_desc(self, node):
-        self.desc_context.append(node.attributes.get("desctype", ""))
+        self._push_status(desc_type=node.attributes.get("desctype", ""))
 
     def depart_desc(self, _node):
-        self.desc_context.pop()
+        self._pop_status()
 
+    @pushing_context
     def visit_desc_signature(self, node):
         """the main signature of class/method"""
 
         # Insert anchors if enabled by the config
         if self.config.markdown_anchor_signatures:
             for anchor in node.get("ids", []):
                 self._add_anchor(anchor)
 
         # We don't want methods to be at the same level as classes,
         # If signature has a non-null class, that's means it is a signature
         # of a class method
-        self.ensure_eol()
-        if node.attributes.get("class", None):
-            self.add("#### ")
-        else:
-            self.add("### ")
+        h_level = 4 if node.get("class", None) else 3
+        self._push_context(TitleContext(h_level))
 
     def visit_desc_parameterlist(self, _node):
         self._push_context(WrappedContext("(", ")", wrap_empty=True))
         self._push_context(CommaSeparatedContext(", "))
 
     def depart_desc_parameterlist(self, _node):
         self._pop_context(count=2)
 
-    def depart_desc_signature(self, _node):
-        """the main signature of class/method"""
-        self.ensure_eol()
-
-    def sep_ctx(self, section="body") -> CommaSeparatedContext:
-        ctx = self.ctx(section)
+    @property
+    def sep_ctx(self) -> CommaSeparatedContext:
+        ctx = self.ctx
         assert isinstance(ctx, CommaSeparatedContext)
         return ctx
 
     def visit_desc_parameter(self, _node):
         """single method/class ctr param"""
-        self.sep_ctx().enter_parameter()
+        self.sep_ctx.enter_parameter()  # workaround pylint: disable=no-member
 
     def depart_desc_parameter(self, _node):
-        self.sep_ctx().exit_parameter()
+        self.sep_ctx.exit_parameter()  # workaround pylint: disable=no-member
 
     def visit_field_list(self, _node):
         self._start_list("*")
 
-    def depart_field_list(self, _node):
-        self._end_list()
-
-    def visit_field(self, _node):
-        self._start_list_item()
-
-    def depart_field(self, _node):
-        self._end_list_item()
+    depart_field_list = _end_list
+    visit_field = _start_list_item
+    depart_field = _end_list_item
 
+    @pushing_context
     def visit_field_body(self, _node):
-        self.ensure_eol(1)
-        self._push_context(SubContext())
-
-    def depart_field_body(self, _node):
-        self._pop_context()
-        self.ensure_eol(1)
+        self._push_context(SubContext(SubContextParams(1, 1)))
 
+    @pushing_context
     def visit_versionmodified(self, node):
         """
         Node for version change entries.
         Currently used for “versionadded”, “versionchanged” and “deprecated” directives.
         Type will hold something like 'deprecated'
         """
         node_type = node.attributes["type"].capitalize()
-        self.ensure_eol(1)
-        self.add(f"**{node_type}:** ")
-        self.ensure_eol(1)
-        self._push_context(SubContext())
-
-    def depart_versionmodified(self, _node):
-        self._pop_context()
-        self.ensure_eol(1)
+        self._push_box(node_type)
 
     ################################################################################
     # tables
     ################################################################################
     # table
     #   tgroup [cols=x]
     #     colspec
@@ -641,90 +626,40 @@
     #           paragraph (optional)
     #     tbody
     #       row
     #         entry
     #           paragraph (optional)
     ###############################################################################
 
-    def table_ctx(self, section="body") -> TableContext:
-        ctx = self.ctx(section)
+    @property
+    def table_ctx(self) -> TableContext:
+        ctx = self.ctx
         assert isinstance(ctx, TableContext)
         return ctx
 
+    @pushing_context
     def visit_table(self, _node):
-        self._push_context(TableContext())
-
-    depart_table = _pop_context
+        self._push_context(TableContext(params=SubContextParams(1, 1)))
 
     def visit_thead(self, _node):
-        self.table_ctx().enter_head()
+        self.table_ctx.enter_head()  # workaround pylint: disable=no-member
 
     def depart_thead(self, _node):
-        self.table_ctx().exit_head()
+        self.table_ctx.exit_head()  # workaround pylint: disable=no-member
 
     def visit_tbody(self, _node):
-        self.table_ctx().enter_body()
+        self.table_ctx.enter_body()  # workaround pylint: disable=no-member
 
     def depart_tbody(self, _node):
-        self.table_ctx().exit_body()
+        self.table_ctx.exit_body()  # workaround pylint: disable=no-member
 
     def visit_row(self, _node):
-        self.table_ctx().enter_row()
+        self.table_ctx.enter_row()  # workaround pylint: disable=no-member
 
     def depart_row(self, _node):
-        self.table_ctx().exit_row()
+        self.table_ctx.exit_row()  # workaround pylint: disable=no-member
 
     def visit_entry(self, _node):
-        self.table_ctx().enter_entry()
+        self.table_ctx.enter_entry()  # workaround pylint: disable=no-member
 
     def depart_entry(self, _node):
-        self.table_ctx().exit_entry()
-
-    ################################################################################
-    # lists
-    ################################################################################
-    # enumerated_list/bullet_list
-    #     list_item
-    #       paragraph (optional)
-    ###############################################################################
-
-    def _start_list(self, marker: Union[int, str]):
-        self.ensure_eol()
-        if isinstance(marker, str) and marker[-1] != " ":
-            marker += " "
-        self.list_context.append(marker)
-
-    def _end_list(self):
-        self.list_context.pop()
-        # We need two line breaks to make sure the next paragraph will not merge into the list
-        self.ensure_eol(2)
-
-    def _start_list_item(self):
-        marker = self.list_context[-1]
-        if isinstance(marker, int):
-            marker = f"{marker}. "
-            self.list_context[-1] += 1
-        # Make sure the list item prefix starts at a new line
-        self.ensure_eol()
-        self._push_context(IndentContext(marker, only_first=True))
-
-    def _end_list_item(self):
-        self._pop_context()
-        # Make sure the list item ends with a new line
-        self.ensure_eol()
-
-    def visit_enumerated_list(self, _node):
-        self._start_list(1)
-
-    def depart_enumerated_list(self, _node):
-        self._end_list()
-
-    def visit_bullet_list(self, node):
-        self._start_list(node.attributes.get("bullet", "*"))
-
-    depart_bullet_list = depart_enumerated_list
-
-    def visit_list_item(self, _node):
-        self._start_list_item()
-
-    def depart_list_item(self, _node):
-        self._end_list_item()
+        self.table_ctx.exit_entry()  # workaround pylint: disable=no-member
```

### Comparing `sphinx-markdown-builder-0.6.0/sphinx_markdown_builder/writer.py` & `sphinx-markdown-builder-0.6.1/sphinx_markdown_builder/writer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-docutils XML to markdown writer.
+Custom docutils writer for markdown.
 """
 from docutils import frontend, writers
 
 from sphinx_markdown_builder.translator import MarkdownTranslator
 
 
 class MarkdownWriter(writers.Writer):
@@ -11,15 +11,15 @@
     """Formats this writer supports."""
 
     output = None
     """Final translated form of `document`."""
 
     # Add configuration settings for additional Markdown flavours here.
     settings_spec = (
-        "Markdown-Specific Options",
+        "Markdown writer options",
         None,
         (
             (
                 "Extended Markdown syntax.",
                 ["--extended-markdown"],
                 {
                     "default": 0,
@@ -38,14 +38,14 @@
             ),
         ),
     )
 
     translator_class = MarkdownTranslator
 
     def __init__(self, builder=None):
-        writers.Writer.__init__(self)
+        super().__init__()
         self.builder = builder
 
     def translate(self):
         visitor = self.builder.create_translator(self.document, self.builder)
         self.document.walkabout(visitor)
         self.output = visitor.astext()
```

### Comparing `sphinx-markdown-builder-0.6.0/sphinx_markdown_builder.egg-info/PKG-INFO` & `sphinx-markdown-builder-0.6.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: sphinx-markdown-builder
-Version: 0.6.0
-Summary: Sphinx builder that generates markdown files from reStructuredText.
+Version: 0.6.1
+Summary: A Sphinx extension to add markdown generation support.
 Author-email: Liran Funaro <liran.funaro@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/liran-funaro/sphinx-markdown-builder
-Keywords: sphinx,markdown,docs,documentation,builder
+Keywords: sphinx,sphinx-extention,markdown,docs,documentation,builder
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # sphinx-markdown-builder
 
 [![Coverage Status](https://coveralls.io/repos/github/liran-funaro/sphinx-markdown-builder/badge.svg?branch=main)](https://coveralls.io/github/liran-funaro/sphinx-markdown-builder?branch=main)
 
-Sphinx builder that generates markdown files from reStructuredText.
+A Sphinx extension to add markdown generation support.
 
 ## Install
 
 ```sh
-pip3 install sphinx-markdown-builder==0.6.0
+pip3 install sphinx-markdown-builder==0.6.1
 ```
 
-
 ## Usage
 
 Add the extension to your `conf.py` file:
 ```python
 extensions = [
     ...,
     "sphinx_markdown_builder",
@@ -45,29 +44,38 @@
 sphinx-build -M markdown ./docs ./build
 ```
 
 ## Configurations
 
 You can add the following configurations to your `conf.py` file:
 
+* `markdown_anchor_sections`/`markdown_anchor_signatures`: If set to `True`, 
+  then anchors will be added before each section/function/class signature. 
+  This allows references to a specific anchor in the document.
+* `markdown_docinfo`: Adds metadata to the top of each document containing author, copyright, and version.
 * `markdown_http_base`: If set, all references will link to this prefix address
 * `markdown_uri_doc_suffix`: If set, all references will link to documents with this suffix.
-* `markdown_anchor_sections`/`markdown_anchor_signatures`: If set to `True`, then anchors will be added before each section/function/class signature. 
- This allows references to a specific anchor in the document.
 
 For example, if your `conf.py` file have the following configuration:
+
 ```python
 markdown_http_base = "https://your-domain.com/docs"
 markdown_uri_doc_suffix = ".html"
 ```
 
 Then a reference to `your-doc-name#your-header` will be substituted with `https://your-domain.com/docs/your-doc-name.html#your-header`. 
 
 ## Credits
-This project forked from [
-sphinx-markdown-builder](https://github.com/clayrisser/sphinx-markdown-builder), which was developed by [Clay Risser](https://github.com/clayrisser) under the [MIT](https://github.com/clayrisser/sphinx-markdown-builder/blob/master/LICENSE) license.
+This project forked from [clayrisser/sphinx-markdown-builder], which was developed by [Clay Risser] under the [MIT] license.
 
-The original implementation was based on [doctree2md](https://github.com/matthew-brett/nb2plots/blob/master/nb2plots/doctree2md.py) by [Matthew Brett](https://github.com/matthew-brett) under the [BSD-2](https://github.com/matthew-brett/nb2plots/blob/main/LICENSE) license.
+The original implementation was based on [doctree2md] by [Matthew Brett] under the [BSD-2] license.
 
 ## License
 
-[MIT](LICENSE)
+[MIT]
+
+[clayrisser/sphinx-markdown-builder]: https://github.com/clayrisser/sphinx-markdown-builder
+[Clay Risser]: https://github.com/clayrisser
+[doctree2md]: https://github.com/matthew-brett/nb2plots/blob/master/nb2plots/doctree2md.py
+[Matthew Brett]: https://github.com/matthew-brett
+[MIT]: LICENSE
+[BSD-2]: https://github.com/matthew-brett/nb2plots/blob/main/LICENSE
```

### Comparing `sphinx-markdown-builder-0.6.0/tests/test_builder.py` & `sphinx-markdown-builder-0.6.1/tests/test_builder.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,92 @@
 """
-Unit tests for the markdown builder
+Integration tests for the markdown builder
 """
 import os
 import shutil
+import stat
 from pathlib import Path
 from typing import Iterable
 
 import pytest
 from sphinx.cmd.build import main
 
 BUILD_PATH = "./tests/docs-build"
 SOURCE_PATH = "./tests/source"
 
-TEST_NAMES = ["direct", "http"]
-SOURCE_FLAGS = [[], ["-D", 'markdown_http_base="https://localhost"', "-D", 'markdown_uri_doc_suffix=".html"']]
-BUILD_PATH_OPTIONS = [os.path.join(BUILD_PATH, "direct"), os.path.join(BUILD_PATH, "http")]
+TEST_NAMES = ["defaults", "overrides"]
+SOURCE_FLAGS = [
+    [],
+    [
+        "-D",
+        'markdown_http_base="https://localhost"',
+        "-D",
+        'markdown_uri_doc_suffix=".html"',
+        "-D",
+        "markdown_docinfo=True",
+        "-D",
+        "markdown_anchor_sections=True",
+        "-D",
+        "markdown_anchor_signatures=True",
+    ],
+]
+BUILD_PATH_OPTIONS = [BUILD_PATH, os.path.join(BUILD_PATH, "overrides")]
 OPTIONS = list(zip(SOURCE_FLAGS, BUILD_PATH_OPTIONS))
 
 
+def _rm_build_path(build_path: str):
+    if os.path.exists(build_path):
+        shutil.rmtree(build_path)
+
+
+def _touch_sources():
+    for file_name in os.listdir(SOURCE_PATH):
+        _, ext = os.path.splitext(file_name)
+        if ext == ".rst":
+            Path(SOURCE_PATH, file_name).touch()
+            break
+
+
+def _chmod_output(build_path: str, apply_func):
+    if not os.path.exists(build_path):
+        return
+
+    for root, dirs, files in os.walk(build_path):
+        for file_name in files:
+            _, ext = os.path.splitext(file_name)
+            if ext == ".md":
+                p = Path(root, file_name)
+                p.chmod(apply_func(p.stat().st_mode))
+
+
 def run_sphinx(build_path, *flags):
-    return main(["-M", "markdown", SOURCE_PATH, build_path, *flags])
+    """Runs sphinx and validate success"""
+    ret_code = main(["-M", "markdown", SOURCE_PATH, build_path, *flags])
+    assert ret_code == 0
 
 
 @pytest.mark.parametrize(["flags", "build_path"], OPTIONS, ids=TEST_NAMES)
 def test_builder_make_all(flags: Iterable[str], build_path: str):
     run_sphinx(build_path, "-a", *flags)
 
 
 @pytest.mark.parametrize(["flags", "build_path"], OPTIONS, ids=TEST_NAMES)
 def test_builder_make_updated(flags: Iterable[str], build_path: str):
-    for file in os.listdir(SOURCE_PATH):
-        Path(SOURCE_PATH, file).touch()
-        break
+    _touch_sources()
     run_sphinx(build_path, *flags)
 
 
 @pytest.mark.parametrize(["flags", "build_path"], OPTIONS, ids=TEST_NAMES)
 def test_builder_make_missing(flags: Iterable[str], build_path: str):
-    if os.path.exists(build_path):
-        shutil.rmtree(build_path)
+    _rm_build_path(build_path)
     run_sphinx(build_path, *flags)
+
+
+@pytest.mark.parametrize(["flags", "build_path"], OPTIONS, ids=TEST_NAMES)
+def test_builder_access_issue(flags: Iterable[str], build_path: str):
+    _touch_sources()
+    flag = stat.S_IWUSR | stat.S_IWGRP | stat.S_IWOTH
+    _chmod_output(build_path, lambda mode: mode & ~flag)
+    try:
+        run_sphinx(build_path, *flags)
+    finally:
+        _chmod_output(build_path, lambda mode: mode | flag)
```

