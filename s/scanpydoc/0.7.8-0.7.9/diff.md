# Comparing `tmp/scanpydoc-0.7.8.tar.gz` & `tmp/scanpydoc-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scanpydoc-0.7.8.tar", last modified: Fri Mar 10 15:21:44 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `scanpydoc-0.7.8.tar` & `scanpydoc-0.7.9.tar`

### file list

```diff
@@ -1,33 +1,36 @@
--rw-r--r--   0        0        0      122 2019-08-21 12:35:17.698271 scanpydoc-0.7.8/.editorconfig
--rw-r--r--   0        0        0      816 2023-03-10 15:20:57.742845 scanpydoc-0.7.8/.github/workflows/ci.yml
--rw-r--r--   0        0        0      141 2019-09-04 17:37:13.117667 scanpydoc-0.7.8/.gitignore
--rw-r--r--   0        0        0      293 2023-02-07 10:34:18.531285 scanpydoc-0.7.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      168 2020-11-18 10:36:01.381899 scanpydoc-0.7.8/.readthedocs.yml
--rw-r--r--   0        0        0      197 2023-02-07 10:34:18.531285 scanpydoc-0.7.8/.vscode/settings.json
--rw-r--r--   0        0        0    32422 2019-01-03 15:54:20.611873 scanpydoc-0.7.8/LICENSE
--rw-r--r--   0        0        0     1113 2021-09-06 11:16:53.522180 scanpydoc-0.7.8/README.rst
--rw-r--r--   0        0        0       80 2019-01-03 13:48:15.910309 scanpydoc-0.7.8/docs/_templates/autosummary/base.rst
--rw-r--r--   0        0        0      517 2019-09-04 17:53:09.602346 scanpydoc-0.7.8/docs/_templates/autosummary/module.rst
--rw-r--r--   0        0        0     1889 2022-03-17 16:34:35.720228 scanpydoc-0.7.8/docs/conf.py
--rw-r--r--   0        0        0      249 2020-07-31 12:27:29.129891 scanpydoc-0.7.8/docs/index.rst
--rw-r--r--   0        0        0     1409 2023-02-07 10:19:44.737764 scanpydoc-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     1209 2022-03-17 12:58:38.247279 scanpydoc-0.7.8/scanpydoc/__init__.py
--rw-r--r--   0        0        0     1942 2021-09-06 11:11:48.203517 scanpydoc-0.7.8/scanpydoc/autosummary_generate_imported.py
--rw-r--r--   0        0        0     3590 2021-09-06 11:11:48.203517 scanpydoc-0.7.8/scanpydoc/definition_list_typed_field.py
--rw-r--r--   0        0        0     4620 2022-03-17 16:48:53.913855 scanpydoc-0.7.8/scanpydoc/elegant_typehints/__init__.py
--rw-r--r--   0        0        0     1846 2021-09-06 11:11:48.203517 scanpydoc-0.7.8/scanpydoc/elegant_typehints/autodoc_patch.py
--rw-r--r--   0        0        0      378 2022-01-06 12:07:21.636604 scanpydoc-0.7.8/scanpydoc/elegant_typehints/example.py
--rw-r--r--   0        0        0     5165 2023-03-10 15:20:57.742845 scanpydoc-0.7.8/scanpydoc/elegant_typehints/formatting.py
--rw-r--r--   0        0        0     3342 2022-03-18 13:44:58.057911 scanpydoc-0.7.8/scanpydoc/elegant_typehints/return_tuple.py
--rw-r--r--   0        0        0      104 2019-09-04 17:51:03.459290 scanpydoc-0.7.8/scanpydoc/elegant_typehints/static/typehints.css
--rw-r--r--   0        0        0     5382 2022-03-17 12:58:17.010341 scanpydoc-0.7.8/scanpydoc/rtd_github_links.py
--rw-r--r--   0        0        0     1665 2021-09-06 10:53:45.210492 scanpydoc-0.7.8/scanpydoc/theme/__init__.py
--rw-r--r--   0        0        0     1294 2021-07-12 10:01:36.796745 scanpydoc-0.7.8/scanpydoc/theme/layout.html
--rw-r--r--   0        0        0     3584 2021-12-19 13:23:54.854177 scanpydoc-0.7.8/scanpydoc/theme/static/css/scanpy.css
--rw-r--r--   0        0        0      513 2021-07-12 10:01:36.796745 scanpydoc-0.7.8/scanpydoc/theme/theme.conf
--rw-r--r--   0        0        0     2465 2022-01-10 16:07:22.719946 scanpydoc-0.7.8/tests/conftest.py
--rw-r--r--   0        0        0      727 2019-10-25 11:53:23.406024 scanpydoc-0.7.8/tests/test_base.py
--rw-r--r--   0        0        0     2622 2019-10-25 10:45:46.111818 scanpydoc-0.7.8/tests/test_definition_list_typed_field.py
--rw-r--r--   0        0        0     9858 2023-03-10 15:20:57.742845 scanpydoc-0.7.8/tests/test_elegant_typehints.py
--rw-r--r--   0        0        0     1087 2022-03-17 12:58:17.011341 scanpydoc-0.7.8/tests/test_rtd_github_links.py
--rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 scanpydoc-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/.editorconfig
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/.prettierrc
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/.readthedocs.yml
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/.vscode/settings.json
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/docs/conf.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/docs/index.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/docs/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/docs/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/_version.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/autosummary_generate_imported.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/definition_list_typed_field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/py.typed
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/rtd_github_links.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/__init__.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/autodoc_patch.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/example.py
+-rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/formatting.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/return_tuple.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/static/typehints.css
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/theme/__init__.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/theme/layout.html
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/theme/theme.conf
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/theme/static/css/scanpy.css
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/tests/conftest.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/tests/test_base.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/tests/test_definition_list_typed_field.py
+-rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/tests/test_elegant_typehints.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/tests/test_rtd_github_links.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/.gitignore
+-rw-r--r--   0        0        0    32422 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/LICENSE
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/README.rst
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/PKG-INFO
```

### Comparing `scanpydoc-0.7.8/.github/workflows/ci.yml` & `scanpydoc-0.7.9/.github/workflows/ci.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
 name: Python tests
 
 on:
   push:
-    branches: [ master ]
+    branches: [main]
   pull_request:
-    branches: [ master ]
+    branches: [main]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
-    - uses: actions/checkout@v2
-    - uses: actions/setup-python@v2
-      with:
-        python-version: ${{ matrix.python-version }}
-    - uses: actions/cache@v2
-      with:
-        path: |
-          ~/.cache/pip
-          ~/.cache/pre-commit
-        key: ${{ runner.os }}-pip-${{ hashFiles('pyproject.toml') }}
-    - name: dependencies
-      run: |
-        pip install --upgrade pip wheel
-        pip install .[test,typehints]
-    - name: tests
-      run: pytest --color=yes
+      - uses: actions/checkout@v2
+      - uses: actions/setup-python@v2
+        with:
+          python-version: ${{ matrix.python-version }}
+      - uses: actions/cache@v2
+        with:
+          path: |
+            ~/.cache/pip
+            ~/.cache/pre-commit
+          key: ${{ runner.os }}-pip-${{ hashFiles('pyproject.toml') }}
+      - name: dependencies
+        run: |
+          pip install --upgrade pip wheel
+          pip install .[test,typehints]
+      - name: tests
+        run: pytest --color=yes
```

### Comparing `scanpydoc-0.7.8/LICENSE` & `scanpydoc-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.7.8/README.rst` & `scanpydoc-0.7.9/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -10,13 +10,13 @@
    :alt: PiPI version
 .. |docs| image:: https://readthedocs.com/projects/icb-scanpydoc/badge/
    :target: https://icb-scanpydoc.readthedocs-hosted.com/
    :alt: doc build status
 .. |tests| image:: https://github.com/theislab/scanpydoc/actions/workflows/ci.yml/badge.svg
    :target: https://github.com/theislab/scanpydoc/actions/workflows/ci.yml
    :alt: python test status
-.. |checks| image:: https://results.pre-commit.ci/badge/github/theislab/scanpydoc/master.svg
-   :target: https://results.pre-commit.ci/latest/github/theislab/scanpydoc/master
+.. |checks| image:: https://results.pre-commit.ci/badge/github/theislab/scanpydoc/main.svg
+   :target: https://results.pre-commit.ci/latest/github/theislab/scanpydoc/main
    :alt: pre-commit.ci status
-.. |cov| image:: https://codecov.io/gh/theislab/scanpydoc/branch/master/graph/badge.svg
+.. |cov| image:: https://codecov.io/gh/theislab/scanpydoc/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/theislab/scanpydoc
    :alt: coverage
```

### Comparing `scanpydoc-0.7.8/docs/_templates/autosummary/module.rst` & `scanpydoc-0.7.9/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.7.8/docs/conf.py` & `scanpydoc-0.7.9/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 # Generate .rst stubs for modules using autosummary
 autosummary_generate = True
 # Don’t add module paths to documented functions’ names
 add_module_names = False
 
 html_theme = "scanpydoc"
 html_context = dict(
-    github_user="theislab", github_repo="scanpydoc", github_version="master"
+    github_user="theislab", github_repo="scanpydoc", github_version="main"
 )
 
 # proj/doc/conf.py/../.. → proj
 project_dir = Path(__file__).parent.parent
 
 
 def setup(app: Sphinx):
```

### Comparing `scanpydoc-0.7.8/scanpydoc/__init__.py` & `scanpydoc-0.7.9/src/scanpydoc/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-"""A series of Sphinx extensions to get easy to maintain, numpydoc style documentation.
+"""A series of Sphinx extensions to get maintainable numpydoc style documentation.
 
 This module is also an extension itself which simply sets up all included extensions.
 """
+from __future__ import annotations
+
 from textwrap import indent
-from typing import Any, Dict
+from typing import Any
 
-from get_version import get_version
 from sphinx.application import Sphinx
 
+from ._version import __version__
 
-__version__ = get_version(__file__, vcs="git")
 
 metadata = dict(version=__version__, env_version=1, parallel_read_safe=True)
 
 # Can’t seem to be able to do this in numpydoc style:
 # https://github.com/sphinx-doc/sphinx/issues/5887
 setup_sig_str = """\
 Args:
@@ -26,15 +27,15 @@
 
 def _setup_sig(fn):
     fn.__doc__ += "\n\n" + indent(setup_sig_str, " " * 4)
     return fn
 
 
 @_setup_sig
-def setup(app: Sphinx) -> Dict[str, Any]:
-    """Set up all included extensions!"""
+def setup(app: Sphinx) -> dict[str, Any]:
+    """Set up all included extensions!."""
     app.setup_extension("scanpydoc.autosummary_generate_imported")
     app.setup_extension("scanpydoc.definition_list_typed_field")
     app.setup_extension("scanpydoc.elegant_typehints")
     app.setup_extension("scanpydoc.rtd_github_links")
     app.setup_extension("scanpydoc.theme")
     return metadata
```

### Comparing `scanpydoc-0.7.8/scanpydoc/autosummary_generate_imported.py` & `scanpydoc-0.7.9/src/scanpydoc/autosummary_generate_imported.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Generate autosummary docs for imported members.
 
-This extension patches the :mod:`~sphinx.ext.autosummary` extension to generate docs for imported members.
-It needs to be loaded and :confval:`autosummary_generate` needs to be set to :obj:`True`.
+This extension patches the :mod:`~sphinx.ext.autosummary` extension
+to generate docs for imported members.
+It needs to be loaded and :confval:`autosummary_generate` needs to be set to ``True``.
 
 This will hopefully be superseded by the ability to add ``:imported-members:``
 to `autosummary templates`_ in the future. See `Sphinx issue 4372`_.
 
 .. _autosummary templates: http://www.sphinx-doc.org/en/master/usage/extensions/autosummary.html#customizing-templates
 .. _Sphinx issue 4372: https://github.com/sphinx-doc/sphinx/issues/4372
 """
+from __future__ import annotations
 
 import logging
 from pathlib import Path
-from typing import Any, Dict
+from typing import Any
 
 from sphinx.application import Sphinx
 from sphinx.ext import autosummary
 from sphinx.ext.autosummary.generate import generate_autosummary_docs
 
 from . import _setup_sig, metadata
 
@@ -56,12 +58,12 @@
         base_path=app.srcdir,
         imported_members=True,
         app=app,
     )
 
 
 @_setup_sig
-def setup(app: Sphinx) -> Dict[str, Any]:
+def setup(app: Sphinx) -> dict[str, Any]:
     """Patch autosummary to generate docs for imported members as well."""
     autosummary.process_generate_options = _generate_stubs
 
     return metadata
```

### Comparing `scanpydoc-0.7.8/scanpydoc/definition_list_typed_field.py` & `scanpydoc-0.7.9/src/scanpydoc/definition_list_typed_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Prettier function parameter documentation.
 
 This extension replaces the default :class:`~sphinx.domains.python.PyTypedField`
 with a derivative :class:`DLTypedField`, which renders item items
 (e.g. function parameters) as definition lists instead of simple paragraphs.
 """
 
-from typing import Any, Dict, List, Tuple
+from __future__ import annotations
+
+from typing import Any
 
 from docutils import nodes
 from sphinx import addnodes
 from sphinx.application import Sphinx
 from sphinx.domains.python import PyObject, PyTypedField
 from sphinx.environment import BuildEnvironment
 
@@ -26,27 +28,29 @@
     """
 
     #: Override the list type
     list_type = nodes.definition_list
 
     def make_field(
         self,
-        types: Dict[str, List[nodes.Node]],
+        types: dict[str, list[nodes.Node]],
         domain: str,
-        items: Tuple[str, List[nodes.inline]],
-        env: BuildEnvironment = None,
+        items: tuple[str, list[nodes.inline]],
+        env: BuildEnvironment | None = None,
         **kw,
     ) -> nodes.field:
-        """Render a field to a document-tree node representing a definition list item."""
+        """
+        Render a field to a document-tree node representing a definition list item.
+        """
 
         def make_refs(role_name, name, node):
             return self.make_xrefs(role_name, domain, name, node, env=env, **kw)
 
         def handle_item(
-            fieldarg: str, content: List[nodes.inline]
+            fieldarg: str, content: list[nodes.inline]
         ) -> nodes.definition_list_item:
             head = nodes.term()
             head += make_refs(self.rolename, fieldarg, addnodes.literal_strong)
             field_type = types.pop(fieldarg, None)
             if field_type is not None:
                 head += nodes.Text(" : ")
                 if len(field_type) == 1 and isinstance(field_type[0], nodes.Text):
@@ -60,23 +64,24 @@
             body_content = nodes.paragraph("", "", *content)
             body = nodes.definition("", body_content)
 
             return nodes.definition_list_item("", head, body)
 
         field_name = nodes.field_name("", self.label)
         assert not self.can_collapse
-        body_node = self.list_type()
+        # “simple” for pydata sphinx theme
+        body_node = self.list_type(classes=["simple"])
         for field_arg, content in items:
             body_node += handle_item(field_arg, content)
         field_body = nodes.field_body("", body_node)
         return nodes.field("", field_name, field_body)
 
 
 @_setup_sig
-def setup(app: Sphinx) -> Dict[str, Any]:
+def setup(app: Sphinx) -> dict[str, Any]:
     """Replace :class:`~sphinx.domains.python.PyTypedField` with ours."""
     napoleon_requested = "sphinx.ext.napoleon" in app.config.extensions
     napoleon_loaded = next(
         (True for ft in PyObject.doc_field_types if ft.name == "keyword"), False
     )
     if napoleon_requested and not napoleon_loaded:
         raise RuntimeError(f"Please load sphinx.ext.napoleon before {__name__}")
```

### Comparing `scanpydoc-0.7.8/scanpydoc/elegant_typehints/__init__.py` & `scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,20 @@
                      A floating point number
 
 
 .. _sphinx issue 4826: https://github.com/sphinx-doc/sphinx/issues/4826
 .. _sphinx-autodoc-typehints issue 38: https://github.com/agronholm/sphinx-autodoc-typehints/issues/38
 
 """
+from __future__ import annotations
+
 from collections import ChainMap
 from functools import partial
 from pathlib import Path
-from typing import Any, Dict
+from typing import Any
 
 from docutils.parsers.rst import roles
 from sphinx.application import Sphinx
 from sphinx.config import Config
 from sphinx.ext.autodoc import ClassDocumenter
 
 from .. import _setup_sig, metadata
@@ -86,15 +88,15 @@
     config.html_static_path.append(str(HERE / "static"))
 
 
 example_func.__module__ = "scanpydoc.elegant_typehints"  # Make it show up here
 
 
 @_setup_sig
-def setup(app: Sphinx) -> Dict[str, Any]:
+def setup(app: Sphinx) -> dict[str, Any]:
     """Patches :mod:`sphinx_autodoc_typehints` for a more elegant display."""
     # TODO: Unsure if “html” is sufficient or if we need to do “env”;
     #       Depends on when the autodoc-process-docstring event is handled.
     app.add_config_value("qualname_overrides", {}, "html")
     app.add_config_value("annotate_defaults", True, "html")
     app.add_css_file("typehints.css")
     app.connect("config-inited", _init_vars)
```

### Comparing `scanpydoc-0.7.8/scanpydoc/elegant_typehints/autodoc_patch.py` & `scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/autodoc_patch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
+from collections.abc import Callable, Mapping
 from functools import wraps
-from typing import Callable, Mapping, Tuple
 
 from docutils.statemachine import StringList
 from sphinx.ext.autodoc import ClassDocumenter
 
 
 def dir_head_adder(
     qualname_overrides: Mapping[str, str],
@@ -30,15 +32,15 @@
                 (f".. py:{direc}:: {old_cls}", f"   :module: {old_mod}"),
                 (f".. py:{direc}:: {new_cls}", f"   :module: {new_mod}"),
             )
 
     return add_directive_header
 
 
-def replace_multi_suffix(lines: StringList, old: Tuple[str, str], new: Tuple[str, str]):
+def replace_multi_suffix(lines: StringList, old: tuple[str, str], new: tuple[str, str]):
     if len(old) != len(new) != 2:
         raise NotImplementedError("Only supports replacing 2 lines")
     for l, line in enumerate(lines):
         start = line.find(old[0])
         if start == -1:
             continue
         prefix = line[:start]
```

### Comparing `scanpydoc-0.7.8/scanpydoc/elegant_typehints/formatting.py` & `scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/formatting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-import collections.abc as cabc
+from __future__ import annotations
+
 import inspect
+from collections.abc import Callable, Iterable, Mapping, Sequence
 from functools import partial
-from typing import Any, Dict, Iterable, List, Optional, Sequence, Tuple, Type, Union
-
-from sphinx.config import Config
-
-
-try:  # 3.8 additions
-    from typing import Literal, get_args, get_origin
-except ImportError:
-    from typing_extensions import Literal, get_args, get_origin
+from typing import Any, Literal, get_args, get_origin
 
 from docutils import nodes
 from docutils.nodes import Node
 from docutils.parsers.rst.roles import set_classes
 from docutils.parsers.rst.states import Inliner, Struct
 from docutils.utils import SystemMessage, unescape
+from sphinx.config import Config
 from sphinx_autodoc_typehints import format_annotation as _format_orig
 
 from scanpydoc import elegant_typehints
 
 
-def _format_full(annotation: Type[Any], config: Config) -> Optional[str]:
+def _format_full(annotation: type[Any], config: Config) -> str | None:
     if inspect.isclass(annotation) and annotation.__module__ == "builtins":
         return None
 
     origin = get_origin(annotation)
     tilde = "" if config.typehints_fully_qualified else "~"
 
     annotation_cls = annotation if inspect.isclass(annotation) else type(annotation)
@@ -42,92 +37,96 @@
         role = "exc" if issubclass(annotation_cls, BaseException) else "class"
         if override is not None:
             return f":py:{role}:`{tilde}{override}`"
 
     return None
 
 
-def _format_terse(annotation: Type[Any], config: Config) -> str:
+def _format_terse(annotation: type[Any], config: Config) -> str:
+    from typing import Mapping as t_Mapping
+    from typing import Union
+
     origin = get_origin(annotation)
     args = get_args(annotation)
     tilde = "" if config.typehints_fully_qualified else "~"
     fmt = partial(_format_terse, config=config)
 
     # display `Union[A, B]` as `A | B`
     if origin is Union:
         # Never use the `Optional` keyword in the displayed docs.
         # Use `| None` instead, similar to other large numerical packages.
         return " | ".join(map(fmt, args))
 
     # do not show the arguments of Mapping
-    if origin is cabc.Mapping:
-        return f":py:class:`{tilde}typing.Mapping`"
+    if origin is Mapping or origin is t_Mapping:
+        return f":py:class:`{tilde}collections.abc.Mapping`"
 
     # display dict as {k: v}
     if origin is dict and len(args) == 2:
         k, v = args
         return f"{{{fmt(k)}: {fmt(v)}}}"
 
     # display Callable[[a1, a2], r] as (a1, a2) -> r
-    if origin is cabc.Callable and len(args) == 2:
+    if origin is Callable and len(args) == 2:
         params, ret = args
         params = ["…"] if params is Ellipsis else map(fmt, params)
         return f"({', '.join(params)}) → {fmt(ret)}"
 
     # display Literal as {'a', 'b', ...}
     if origin is Literal:
         return f"{{{', '.join(map(repr, args))}}}"
 
     return _format_full(annotation, config) or _format_orig(annotation, config)
 
 
-def format_annotation(annotation: Type[Any], config: Config) -> Optional[str]:
+def format_annotation(annotation: type[Any], config: Config) -> str | None:
     """Generate reStructuredText containing links to the types.
 
     Unlike :func:`sphinx_autodoc_typehints.format_annotation`,
     it tries to achieve a simpler style as seen in numeric packages like numpy.
 
     Args:
+    ----
         annotation: A type or class used as type annotation.
         config: Sphinx config containing ``sphinx-autodoc-typehints``’s options.
 
     Returns:
+    -------
         reStructuredText describing the type
     """
-
     curframe = inspect.currentframe()
     calframe = inspect.getouterframes(curframe, 2)
     if calframe[2].function in {"process_docstring", "_inject_signature"} or (
         calframe[2].function == "_inject_types_to_docstring"
         and calframe[3].function == "process_docstring"
     ):
         return format_both(annotation, config)
     else:  # recursive use
         return _format_full(annotation, config)
 
 
-def format_both(annotation: Type[Any], config: Config) -> str:
+def format_both(annotation: type[Any], config: Config) -> str:
     terse = _format_terse(annotation, config)
     full = _format_full(annotation, config) or _format_orig(annotation, config)
     if terse == full:
         return terse
     return f":annotation-terse:`{_escape(terse)}`\\ :annotation-full:`{_escape(full)}`"
 
 
 def _role_annot(
     name: str,
     rawtext: str,
     text: str,
     lineno: int,
     inliner: Inliner,
-    options: Dict[str, Any] = {},
+    options: dict[str, Any] = {},
     content: Sequence[str] = (),
     # *,  # https://github.com/ambv/black/issues/613
     additional_classes: Iterable[str] = (),
-) -> Tuple[List[Node], List[SystemMessage]]:
+) -> tuple[list[Node], list[SystemMessage]]:
     options = options.copy()
     set_classes(options)
     if additional_classes:
         options["classes"] = options.get("classes", []).copy()
         options["classes"].extend(additional_classes)
     memo = Struct(
         document=inliner.document, reporter=inliner.reporter, language=inliner.language
```

### Comparing `scanpydoc-0.7.8/scanpydoc/elegant_typehints/return_tuple.py` & `scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/return_tuple.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+from __future__ import annotations
+
 import inspect
 import re
 from logging import getLogger
-from typing import Any, List, Optional, Tuple, Type, Union, get_type_hints
-
-
-try:  # 3.8 additions
-    from typing import get_args, get_origin
-except ImportError:
-    from typing_extensions import get_args, get_origin
+from typing import Any, get_args, get_origin, get_type_hints
 
 from sphinx.application import Sphinx
 from sphinx.ext.autodoc import Options
 
 from .formatting import format_both
 
 
 logger = getLogger(__name__)
 re_ret = re.compile("^:returns?: ")
 
 
-def get_tuple_annot(annotation: Optional[Type]) -> Optional[Tuple[Type, ...]]:
+def get_tuple_annot(annotation: type | None) -> tuple[type, ...] | None:
+    from typing import Tuple, Union
+
     if annotation is None:
         return None
     origin = get_origin(annotation)
     if not origin:
         return None
     if origin is Union:
         for annotation in get_args(annotation):
@@ -36,33 +34,30 @@
 
 
 def process_docstring(
     app: Sphinx,
     what: str,
     name: str,
     obj: Any,
-    options: Optional[Options],
-    lines: List[str],
+    options: Options | None,
+    lines: list[str],
 ) -> None:
     # Handle complex objects
     if isinstance(obj, property):
         obj = obj.fget
     if not callable(obj):
         return
     if what in ("class", "exception"):
         obj = obj.__init__
     obj = inspect.unwrap(obj)
     try:
         hints = get_type_hints(obj)
     except (AttributeError, TypeError):
         # Introspecting a slot wrapper will raise TypeError
         return
-    except NameError as e:
-        check_bpo_34776(obj, e)
-        return
     ret_types = get_tuple_annot(hints.get("return"))
     if ret_types is None:
         return
 
     # Get return section
     i_prefix = None
     l_start = None
@@ -86,36 +81,7 @@
         if line.isidentifier() and lines[l + l_start + 1].startswith("    "):
             idxs_ret_names.append(l + l_start)
 
     if len(idxs_ret_names) == len(ret_types):
         for l, rt in zip(idxs_ret_names, ret_types):
             typ = format_both(rt, app.config)
             lines[l : l + 1] = [f"{lines[l]} : {typ}"]
-
-
-# def process_signature(
-#     app: Sphinx,
-#     what: str,
-#     name: str,
-#     obj: Any,
-#     options: Options,
-#     signature: Optional[str],
-#     return_annotation: str,
-# ) -> Optional[Tuple[Optional[str], Optional[str]]]:
-#     return signature, return_annotation
-
-
-def check_bpo_34776(obj: Any, e: NameError):
-    import sys
-
-    ancient = sys.version_info < (3, 7)
-    old_3_7 = (3, 7) < sys.version_info < (3, 7, 6)
-    old_3_8 = (3, 8) < sys.version_info < (3, 8, 1)
-    if ancient or old_3_7 or old_3_8:
-        v = ".".join(map(str, sys.version_info[:3]))
-        logger.warning(
-            f"Error documenting {obj!r}: To avoid this, "
-            f"your Python version {v} must be at least 3.7.6 or 3.8.1. "
-            "For more information see https://bugs.python.org/issue34776"
-        )
-    else:
-        raise e  # No idea what happened
```

### Comparing `scanpydoc-0.7.8/scanpydoc/rtd_github_links.py` & `scanpydoc-0.7.9/src/scanpydoc/rtd_github_links.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""GitHub URLs for class and method pages
+"""GitHub URLs for class and method pages.
 
 This extension registers a :ref:`Jinja filter <jinja:filters>` called :func:`github_url`
 that you can use to convert a module path into a GitHub URL
 
 Configuration
 -------------
 
@@ -39,39 +39,39 @@
 """
 from __future__ import annotations
 
 import inspect
 import sys
 from pathlib import Path, PurePosixPath
 from types import ModuleType
-from typing import Any, Dict, Tuple
+from typing import Any
 
 from jinja2.defaults import DEFAULT_FILTERS
 from sphinx.application import Sphinx
 from sphinx.config import Config
 
 from . import _setup_sig, metadata
 
 
 project_dir = None  # type: Path
 github_base_url = None  # type: str
 
 
 def _init_vars(app: Sphinx, config: Config):
-    """Called when ``conf.py`` has been loaded"""
+    """Called when ``conf.py`` has been loaded."""
     global github_base_url, project_dir
     _check_html_context(config)
     github_base_url = "https://github.com/{github_user}/{github_repo}/tree/{github_version}".format_map(
         config.html_context
     )
     project_dir = Path(config.project_dir)
 
 
-def _get_obj_module(qualname: str) -> Tuple[Any, ModuleType]:
-    """Get a module/class/attribute and its original module by qualname"""
+def _get_obj_module(qualname: str) -> tuple[Any, ModuleType]:
+    """Get a module/class/attribute and its original module by qualname."""
     modname = qualname
     attr_path = []
     while modname not in sys.modules:
         modname, leaf = modname.rsplit(".", 1)
         attr_path.insert(0, leaf)
 
     # retrieve object and find original module name
@@ -106,17 +106,19 @@
         return start, start + len(lines) - 1
 
 
 def github_url(qualname: str) -> str:
     """Get the full GitHub URL for some object’s qualname.
 
     Args:
+    ----
         qualname: The full qualified name of a function, class, method or module
 
     Returns:
+    -------
         A GitHub URL derived from the :confval:`html_context`.
     """
     try:
         obj, module = _get_obj_module(qualname)
     except Exception:
         print(f"Error in github_url({qualname!r}):", file=sys.stderr)
         raise
@@ -147,15 +149,15 @@
         raise ValueError(
             f"Extension {__name__} needs “{mvs}” to be defined in conf.py.\n"
             f"html_context = {html_context!r}"
         )
 
 
 @_setup_sig
-def setup(app: Sphinx) -> Dict[str, Any]:
+def setup(app: Sphinx) -> dict[str, Any]:
     """Register the :func:`github_url` :ref:`Jinja filter <jinja:filters>`."""
     # Guess default project dir
     proj_dir = Path.cwd()
     if proj_dir.name == "docs":
         proj_dir = proj_dir.parent
     elif not (proj_dir / "docs").is_dir():
         proj_dir = proj_dir.parent
```

### Comparing `scanpydoc-0.7.8/scanpydoc/theme/__init__.py` & `scanpydoc-0.7.9/src/scanpydoc/theme/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,10 +76,10 @@
 
 
 HERE = Path(__file__).parent.resolve()
 
 
 @_setup_sig
 def setup(app: Sphinx):
-    """Setup theme (like an extension)"""
+    """Setup theme (like an extension)."""
     app.add_html_theme("scanpydoc", str(HERE))
     return dict(parallel_read_safe=True, parallel_write_safe=True)
```

### Comparing `scanpydoc-0.7.8/scanpydoc/theme/layout.html` & `scanpydoc-0.7.9/src/scanpydoc/theme/layout.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 {% extends "sphinx_rtd_theme/layout.html" %}
 
 <!-- Have to use htmltitle to include this earlier as our style -->
-{%- block htmltitle %}
-{{ super() }}
-{% if theme_docsearch_key and theme_docsearch_index %}
-<link rel=stylesheet href="https://cdn.jsdelivr.net/npm/docsearch.js@{{ theme_docsearch_js_version }}/dist/cdn/docsearch.min.css"/>
-{% endif %}
-{%- endblock -%}
+{%- block htmltitle %} {{ super() }} {% if theme_docsearch_key and theme_docsearch_index
+%}
+<link
+    rel="stylesheet"
+    href="https://cdn.jsdelivr.net/npm/docsearch.js@{{ theme_docsearch_js_version }}/dist/cdn/docsearch.min.css"
+/>
+{% endif %} {%- endblock -%}
 
 <!-- Styles that come last -->
-{%- block extrahead %}
-{{ super() }}
-{% if theme_accent_color %}
+{%- block extrahead %} {{ super() }} {% if theme_accent_color %}
 <style>
-:root { --accent-color: {{ theme_accent_color }} }
+    :root { --accent-color: {{ theme_accent_color }} }
 </style>
-{% endif %}
-{% endblock %}
-
-{% set safe_version = version if version in ["latest", "stable"] else "latest" %}
-
-{% block scripts %}
-{{ super() }}
-{% if theme_docsearch_key and theme_docsearch_index %}
+{% endif %} {% endblock %} {% set safe_version = version if version in ["latest",
+"stable"] else "latest" %} {% block scripts %} {{ super() }} {% if theme_docsearch_key
+and theme_docsearch_index %}
 <script src="https://cdn.jsdelivr.net/npm/docsearch.js@{{ theme_docsearch_js_version }}/dist/cdn/docsearch.min.js"></script>
 <script>
-  document.addEventListener('DOMContentLoaded', () => docsearch({
-    apiKey: '{{ theme_docsearch_key }}',
-    indexName: '{{ theme_docsearch_index }}',
-    inputSelector: '#rtd-search-form > input[name="q"]',
-    algoliaOptions: {
-      facetFilters: ['version:{{ theme_docsearch_doc_version or safe_version }}'],
-      hitsPerPage: 10,
-    },
-    debug: {{ theme_docsearch_debug }},
-  }))
+    document.addEventListener('DOMContentLoaded', () => docsearch({
+      apiKey: '{{ theme_docsearch_key }}',
+      indexName: '{{ theme_docsearch_index }}',
+      inputSelector: '#rtd-search-form > input[name="q"]',
+      algoliaOptions: {
+        facetFilters: ['version:{{ theme_docsearch_doc_version or safe_version }}'],
+        hitsPerPage: 10,
+      },
+      debug: {{ theme_docsearch_debug }},
+    }))
 </script>
-{% endif %}
-{% endblock %}
+{% endif %} {% endblock %}
```

### Comparing `scanpydoc-0.7.8/scanpydoc/theme/static/css/scanpy.css` & `scanpydoc-0.7.9/src/scanpydoc/theme/static/css/scanpy.css`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,85 @@
 @import "theme.css";
 
 /* ReadTheDocs theme global changes */
 
-:root { --accent-color: #f07e44 }
-.wy-nav-top { background-color: var(--accent-color) }
-.wy-nav-content { max-width: 1200px }
-.wy-side-nav-search { background-color: transparent }
-.wy-side-nav-search input[type="text"] { border-width: 0 }
-.wy-side-nav-search a.icon-home { font-size: 2em; color: var(--accent-color) }
-.wy-side-nav-search a.icon-home::before { content: none }
-.wy-menu li a { overflow: hidden; text-overflow: ellipsis; }  /* display ellipsis in long items */
+:root {
+    --accent-color: #f07e44;
+}
+.wy-nav-top {
+    background-color: var(--accent-color);
+}
+.wy-nav-content {
+    max-width: 1200px;
+}
+.wy-side-nav-search {
+    background-color: transparent;
+}
+.wy-side-nav-search input[type="text"] {
+    border-width: 0;
+}
+.wy-side-nav-search a.icon-home {
+    font-size: 2em;
+    color: var(--accent-color);
+}
+.wy-side-nav-search a.icon-home::before {
+    content: none;
+}
+.wy-menu li a {
+    /* display ellipsis in long items */
+    overflow: hidden;
+    text-overflow: ellipsis;
+}
 
 /* DocSearch adaptations */
 
-.wy-nav-side { overflow: visible; }
-.wy-side-scroll { overflow: inherit; }
+.wy-nav-side {
+    overflow: visible;
+}
+.wy-side-scroll {
+    overflow: inherit;
+}
 
 /* Making it a bit wider */
 .algolia-autocomplete .ds-dropdown-menu {
-  max-width: 1000px;
-  min-width: 80vw;
+    max-width: 1000px;
+    min-width: 80vw;
 }
 
 /* Custom classes */
 
-.small { font-size:40% }
-.smaller, .pr, .issue { font-size:70% }
-
+.small {
+    font-size: 40%;
+}
+.smaller,
+.pr,
+.issue {
+    font-size: 70%;
+}
 
 /* Custom classes with bootstrap buttons */
 
 .tutorial,
 .tutorial:visited,
-.tutorial:hover
-{
+.tutorial:hover {
     /* text-decoration: underline; */
     font-weight: bold;
     padding: 2px 5px;
     white-space: nowrap;
     max-width: 100%;
-    background: #EF3270;  /* color from the tail of the scampy */
-    border: solid 1px #EF3270;
-    border-radius: .25rem;
+    background: #ef3270; /* color from the tail of the scampy */
+    border: solid 1px #ef3270;
+    border-radius: 0.25rem;
     font-size: 75%;
     /* font-family: SFMono-Regular,Menlo,Monaco,Consolas,"Liberation Mono","Courier New",Courier,monospace; */
     color: #404040;
     overflow-x: auto;
     box-sizing: border-box;
 }
 
-
 /* Formatting of RTD markup: rubrics and sidebars and admonitions */
 
 /* sidebar */
 .rst-content .sidebar {
     /* margin: 0px 0px 0px 12px; */
     padding-bottom: 0px;
 }
@@ -67,71 +93,70 @@
 }
 
 /* less space after bullet lists in admonitions like warnings and notes */
 .rst-content .section .admonition ul {
     margin-bottom: 6px;
 }
 
-
 /* Code: literals and links */
 
 .rst-content tt.literal,
 .rst-content code.literal {
     color: #404040;
 }
 /* slim font weight for non-link code */
 .rst-content tt:not(.xref),
 .rst-content code:not(.xref),
 .rst-content *:not(a) > tt.xref,
 .rst-content *:not(a) > code.xref,
-.rst-content dl:not(.docutils) code
-{
+.rst-content dl:not(.docutils) code {
     font-weight: normal;
 }
 .rst-content a > tt.xref,
 .rst-content a > code.xref,
 .rst-content dl:not(.docutils) a > tt.xref,
-.rst-content dl:not(.docutils) a > code.xref
-{
-    font-weight: bold;  /* underline looks clumsy, in particular with buttons and
+.rst-content dl:not(.docutils) a > code.xref {
+    font-weight: bold; /* underline looks clumsy, in particular with buttons and
                            other hyperlinks, which don't come with underlines */
 }
 
-
 /* Just one box for annotation code for a less noisy look */
 
 .rst-content .annotation {
     padding: 2px 5px;
     background-color: white;
     border: 1px solid #e1e4e5;
 }
 .rst-content .annotation tt,
 .rst-content .annotation code {
     padding: 0 0;
     background-color: transparent;
     border: 0 solid transparent;
 }
 
-
 /* Parameter lists */
 
 /* Mimick rubric style used for other headings */
 /* TODO: once scanpydoc adds classes, also change return types like this */
 .rst-content dl:not(.docutils) dl > dt {
     font-weight: bold;
     background: none transparent;
     border-left: none;
     margin: 0 0 12px;
     padding: 3px 0 0;
     font-size: 111.11%;
 }
 /* Parameters contain <strong> parts and don’t need bold font */
-.rst-content dl.field-list dl > dt { font-weight: unset }
+.rst-content dl.field-list dl > dt {
+    font-weight: unset;
+}
 /* Add colon between return tuple element name and type */
-.rst-content dl:not(.docutils) dl > dt .classifier::before { content: ' : ' }
+.rst-content dl:not(.docutils) dl > dt .classifier::before {
+    content: " : ";
+}
 
 /* Function headers */
 
 .rst-content dl:not(.docutils) dt {
     background: #edf0f2;
     color: #404040;
     border-top: solid 3px #343131;
```

### Comparing `scanpydoc-0.7.8/scanpydoc/theme/theme.conf` & `scanpydoc-0.7.9/src/scanpydoc/theme/theme.conf`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.7.8/tests/test_base.py` & `scanpydoc-0.7.9/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.7.8/tests/test_definition_list_typed_field.py` & `scanpydoc-0.7.9/tests/test_definition_list_typed_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 from sphinx.application import Sphinx
 from sphinx.builders.html import StandaloneHTMLBuilder
+from sphinx.testing.restructuredtext import parse
 from sphinx.writers.html import HTMLTranslator
 from sphinx.writers.html5 import HTML5Translator
 
 
 @pytest.fixture
 def app(make_app_setup) -> Sphinx:
     app = make_app_setup()
@@ -34,15 +35,15 @@
     app_no_setup = make_app_setup()
     assert app is not make_app_setup
     assert "scanpydoc.definition_list_typed_field" in app.extensions
     assert "scanpydoc.definition_list_typed_field" not in app_no_setup.extensions
 
 
 @pytest.mark.parametrize("code,n", [(params_code, 2), (params_code_single, 1)])
-def test_convert_params(app, parse, code, n):
+def test_convert_params(app, code, n):
     # the directive class is PyModuleLevel → PyObject → ObjectDescription
     # ObjectDescription.run uses a DocFieldTransformer to transform members
     # the signature of each Directive(
     #     name, arguments, options, content, lineno,
     #     content_offset, block_text, state, state_machine,
     # )
 
@@ -65,15 +66,15 @@
         assert dli[1].tagname == "definition"
 
     # print(doc.asdom().toprettyxml())
 
 
 @pytest.mark.parametrize("translator", [HTMLTranslator, HTML5Translator])
 @pytest.mark.parametrize("code", [params_code, params_code_single])
-def test_render_params_html4(app, parse, render, translator, code):
+def test_render_params_html4(app, render, translator, code):
     app.config.html4_writer = translator is HTMLTranslator
     assert app.builder.__class__ is StandaloneHTMLBuilder
     assert app.builder.default_translator_class is translator
 
     doc = parse(app, code)
     html = render(app, doc)
     assert "<dl" in html
```

### Comparing `scanpydoc-0.7.8/tests/test_elegant_typehints.py` & `scanpydoc-0.7.9/tests/test_elegant_typehints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
+from __future__ import annotations
+
 import inspect
 import re
 import sys
 import typing as t
+from collections.abc import Callable, Mapping
 from pathlib import Path
-
-
-try:  # 3.8 additions
-    from typing import Literal, get_args, get_origin
-except ImportError:
-    from typing_extensions import Literal, get_args, get_origin
+from typing import Any
 
 import pytest
 import sphinx_autodoc_typehints as sat
 from sphinx.application import Sphinx
+from sphinx.testing.restructuredtext import parse
 
 from scanpydoc.elegant_typehints.formatting import (
     _format_full,
     _format_terse,
     format_annotation,
 )
 from scanpydoc.elegant_typehints.return_tuple import process_docstring
@@ -52,15 +51,15 @@
             "_testmod.Excep2": "test.Excep2",
         },
     )
 
 
 @pytest.fixture
 def process_doc(app):
-    def process(fn: t.Callable) -> t.List[str]:
+    def process(fn: Callable) -> list[str]:
         lines = inspect.getdoc(fn).split("\n")
         sat.process_docstring(app, "function", fn.__name__, fn, None, lines)
         process_docstring(app, "function", fn.__name__, fn, None, lines)
         return lines
 
     return process
 
@@ -72,65 +71,61 @@
 
 def test_default(app):
     assert format_annotation(str, app.config) is None
 
 
 def test_alternatives(process_doc):
     def fn_test(s: str):
-        """
-        :param s: Test
-        """
+        """:param s: Test"""
 
     assert process_doc(fn_test) == [":type s: :py:class:`str`", ":param s: Test"]
 
 
 def test_defaults_simple(process_doc):
     def fn_test(s: str = "foo", n: None = None, i_: int = 1):
-        r"""
-        :param s: Test S
+        r""":param s: Test S
         :param n: Test N
         :param i\_: Test I
         """
 
     assert process_doc(fn_test) == [
         ":type s: :py:class:`str` (default: ``'foo'``)",
         ":param s: Test S",
         ":type n: :py:obj:`None` (default: ``None``)",
         ":param n: Test N",
         r":type i\_: :py:class:`int` (default: ``1``)",
         r":param i\_: Test I",
     ]
 
 
+@pytest.mark.skipif(sys.version_info < (3, 9), reason="s-a-t bug in Python 3.8")
 def test_defaults_complex(process_doc):
-    def fn_test(m: t.Mapping[str, int] = {}):
-        """
-        :param m: Test M
-        """
+    def fn_test(m: Mapping[str, int] = {}):
+        """:param m: Test M"""
 
     assert process_doc(fn_test) == [
         ":type m: "
-        r":annotation-terse:`:py:class:\`~typing.Mapping\``\ "
+        r":annotation-terse:`:py:class:\`~collections.abc.Mapping\``\ "
         r":annotation-full:`"
-        r":py:class:\`~typing.Mapping\`\[:py:class:\`str\`, :py:class:\`int\`]"
+        r":py:class:\`~collections.abc.Mapping\`\[:py:class:\`str\`, :py:class:\`int\`]"
         "` (default: ``{}``)",
         ":param m: Test M",
     ]
 
 
 def test_mapping(app):
     assert (
-        _format_terse(t.Mapping[str, t.Any], app.config)
-        == ":py:class:`~typing.Mapping`"
+        _format_terse(t.Mapping[str, Any], app.config)
+        == ":py:class:`~collections.abc.Mapping`"
     )
-    assert _format_full(t.Mapping[str, t.Any], app.config) is None
+    assert _format_full(t.Mapping[str, Any], app.config) is None
 
 
 def test_dict(app):
-    assert _format_terse(t.Dict[str, t.Any], app.config) == (
+    assert _format_terse(t.Dict[str, Any], app.config) == (
         "{:py:class:`str`: :py:data:`~typing.Any`}"
     )
 
 
 @pytest.mark.parametrize(
     "annotation,expected",
     [
@@ -142,16 +137,16 @@
     ],
 )
 def test_callable_terse(app, annotation, expected):
     assert _format_terse(annotation, app.config) == expected
 
 
 def test_literal(app):
-    assert _format_terse(Literal["str", 1, None], app.config) == "{'str', 1, None}"
-    assert _format_full(Literal["str", 1, None], app.config) is None
+    assert _format_terse(t.Literal["str", 1, None], app.config) == "{'str', 1, None}"
+    assert _format_full(t.Literal["str", 1, None], app.config) is None
 
 
 @pytest.mark.skipif(sys.version_info < (3, 10), reason="Syntax only available on 3.10+")
 def test_syntax_vs_typing(app):
     u = eval("int | str")
     assert _format_terse(u, app.config) == ":py:class:`int` | :py:class:`str`"
     assert _format_full(u, app.config) is None  # this used to crash
@@ -178,15 +173,15 @@
     app.config.typehints_fully_qualified = True
     assert _format_terse(t.Union[_testmod.Class, str], app.config) == (
         r":py:class:`test.Class` | :py:class:`str`"
     )
     assert _format_full(t.Union[_testmod.Class, str], app.config) is None
 
 
-def test_classes_get_added(app, parse):
+def test_classes_get_added(app):
     doc = parse(app, r":annotation-full:`:py:class:\`str\``")
     assert doc[0].tagname == "paragraph"
     assert doc[0][0].tagname == "inline"
     assert doc[0][0]["classes"] == ["annotation", "full"]
     # print(doc.asdom().toprettyxml())
 
 
@@ -208,15 +203,15 @@
     ids=lambda p: str(p).replace("typing.", ""),
 )
 def test_typing_classes(app, annotation, formatter):
     app.config.typehints_fully_qualified = True
     name = (
         getattr(annotation, "_name", None)
         or getattr(annotation, "__name__", None)
-        or getattr(get_origin(annotation), "_name", None)
+        or getattr(t.get_origin(annotation), "_name", None)
         # 3.6 _Any and _Union
         or annotation.__class__.__name__[1:]
     )
     if formatter is _format_terse and name in {"Union", "Callable"}:
         pytest.skip("Tested elsewhere")
     output = formatter(annotation, app.config)
     assert output is None or output.startswith(f":py:data:`typing.{name}")
@@ -244,15 +239,14 @@
         f'<(code|span)?[^>]*><span class="pre">{sub}</span></(code|span)>',
         out,
     ), out
     assert f'<a class="headerlink" href="#test.{sub}"' in out, out
     assert re.search(rf"Bases: <code[^>]*><span[^>]*>(?:test\.)?{base}", out), out
 
 
-@pytest.mark.skipif(sys.version_info < (3, 7), reason="bpo-34776 only fixed on 3.7+")
 def test_fwd_ref(app, make_module):
     make_module(
         "fwd_mod",
         """\
         from dataclasses import dataclass
 
         @dataclass
@@ -261,15 +255,15 @@
 
         @dataclass
         class B:
             a: A
         """,
     )
     Path(app.srcdir, "index.rst").write_text(
-        f"""\
+        """\
 .. autosummary::
 
    fwd_mod.A
    fwd_mod.B
 """
     )
     app.setup_extension("sphinx.ext.autosummary")
@@ -310,15 +304,15 @@
 @pytest.mark.parametrize(
     "return_ann, foo_rendered",
     [
         (t.Tuple[str, int], ":py:class:`str`"),
         (t.Optional[t.Tuple[str, int]], ":py:class:`str`"),
         (
             t.Tuple[t.Mapping[str, float], int],
-            r":annotation-terse:`:py:class:\`~typing.Mapping\``\ "
+            r":annotation-terse:`:py:class:\`~collections.abc.Mapping\``\ "
             r":annotation-full:`:py:class:\`~typing.Mapping\`\["
             r":py:class:\`str\`, :py:class:\`float\`"
             r"]`",
         ),
     ],
     ids=["Tuple", "Optional[Tuple]", "Complex"],
 )
@@ -338,22 +332,21 @@
         "             A foo!",
         "         bar : :py:class:`int`",
         "             A bar!",
     ]
 
 
 def test_return_too_many(process_doc):
-    def fn_test() -> t.Tuple[int, str]:
-        """
-        :return: foo
-                     A foo!
-                 bar
-                     A bar!
-                 baz
-                     A baz!
+    def fn_test() -> tuple[int, str]:
+        """:return: foo
+        A foo!
+        bar
+        A bar!
+        baz
+        A baz!
         """
 
     assert not any(
         "annotation-terse" in l
         for l in process_doc(fn_test)
         if not l.startswith(":rtype:")
     )
```

### Comparing `scanpydoc-0.7.8/tests/test_rtd_github_links.py` & `scanpydoc-0.7.9/tests/test_rtd_github_links.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import dataclasses
-from dataclasses import Field, dataclass, field
+from dataclasses import Field
 from pathlib import Path
 
 import pytest
 from _pytest.monkeypatch import MonkeyPatch
 
 from scanpydoc.rtd_github_links import _get_linenos, _get_obj_module, github_url
 
@@ -23,17 +22,17 @@
     assert (
         github_url("scanpydoc.rtd_github_links.github_url")
         == f"./scanpydoc/rtd_github_links.py#L{s}-L{e}"
     )
 
 
 def test_get_obj_module():
-    import get_version
+    import sphinx.application as sa
 
-    obj, mod = _get_obj_module("scanpydoc.get_version")
-    assert obj is get_version.get_version
-    assert mod is get_version
+    obj, mod = _get_obj_module("scanpydoc.Sphinx")
+    assert obj is sa.Sphinx
+    assert mod is sa
 
 
 def test_get_obj_module_anntation():
     obj, mod = _get_obj_module("scanpydoc.rtd_github_links._TestCls.test_attr")
     assert isinstance(obj, Field)
```

### Comparing `scanpydoc-0.7.8/PKG-INFO` & `scanpydoc-0.7.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: scanpydoc
-Version: 0.7.8
-Summary: A series of Sphinx extensions to get easy to maintain, numpydoc style documentation.
-Home-page: https://github.com/theislab/scanpydoc/
-Author: Philipp Angerer
-Author-email: phil.angerer@gmail.com
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
+Version: 0.7.9
+Summary: A series of Sphinx extensions to get maintainable numpydoc style documentation.
+Project-URL: Source, https://github.com/theislab/scanpydoc/
+Project-URL: Documentation, https://icb-scanpydoc.readthedocs-hosted.com/
+Author-email: Philipp Angerer <phil.angerer@gmail.com>
+License-Expression: GPL-3.0-or-later
+License-File: LICENSE
+Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Framework :: Sphinx :: Extension
+Requires-Python: >=3.8.1
 Requires-Dist: sphinx>=3.0
-Requires-Dist: get_version
-Requires-Dist: pre-commit ; extra == "dev"
-Requires-Dist: scanpydoc[typehints] ; extra == "doc"
-Requires-Dist: sphinx-rtd-theme ; extra == "doc"
-Requires-Dist: pytest ; extra == "test"
-Requires-Dist: pytest-cov ; extra == "test"
-Requires-Dist: typing_extensions>=3.10 ; extra == "test" and ( python_version<"3.8")
-Requires-Dist: sphinx-rtd-theme ; extra == "theme"
-Requires-Dist: sphinx-autodoc-typehints>=1.15.2 ; extra == "typehints"
-Project-URL: Documentation, https://icb-scanpydoc.readthedocs-hosted.com/
 Provides-Extra: dev
+Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: doc
+Requires-Dist: scanpydoc[typehints]; extra == 'doc'
+Requires-Dist: sphinx-rtd-theme; extra == 'doc'
 Provides-Extra: test
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
 Provides-Extra: theme
+Requires-Dist: sphinx-rtd-theme; extra == 'theme'
 Provides-Extra: typehints
+Requires-Dist: sphinx-autodoc-typehints>=1.15.2; extra == 'typehints'
+Description-Content-Type: text/x-rst
 
 scanpydoc |pypi| |docs| |tests| |checks| |cov|
 ==============================================
 
 A collection of Sphinx extensions similar to (but more flexible than) numpydoc.
 
 Check the self-documenting documentation at https://icb-scanpydoc.readthedocs-hosted.com
@@ -42,14 +40,13 @@
    :alt: PiPI version
 .. |docs| image:: https://readthedocs.com/projects/icb-scanpydoc/badge/
    :target: https://icb-scanpydoc.readthedocs-hosted.com/
    :alt: doc build status
 .. |tests| image:: https://github.com/theislab/scanpydoc/actions/workflows/ci.yml/badge.svg
    :target: https://github.com/theislab/scanpydoc/actions/workflows/ci.yml
    :alt: python test status
-.. |checks| image:: https://results.pre-commit.ci/badge/github/theislab/scanpydoc/master.svg
-   :target: https://results.pre-commit.ci/latest/github/theislab/scanpydoc/master
+.. |checks| image:: https://results.pre-commit.ci/badge/github/theislab/scanpydoc/main.svg
+   :target: https://results.pre-commit.ci/latest/github/theislab/scanpydoc/main
    :alt: pre-commit.ci status
-.. |cov| image:: https://codecov.io/gh/theislab/scanpydoc/branch/master/graph/badge.svg
+.. |cov| image:: https://codecov.io/gh/theislab/scanpydoc/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/theislab/scanpydoc
    :alt: coverage
-
```

