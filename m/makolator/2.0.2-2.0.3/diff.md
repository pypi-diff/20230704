# Comparing `tmp/makolator-2.0.2.tar.gz` & `tmp/makolator-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makolator-2.0.2.tar", max compression
+gzip compressed data, was "makolator-2.0.3.tar", max compression
```

## Comparing `makolator-2.0.2.tar` & `makolator-2.0.3.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0     1067 2023-07-03 06:57:55.163055 makolator-2.0.2/LICENSE
--rw-r--r--   0        0        0     1223 2023-07-03 06:57:55.163055 makolator-2.0.2/README.md
--rw-r--r--   0        0        0     5006 2023-07-03 06:57:55.167055 makolator-2.0.2/makolator/__init__.py
--rw-r--r--   0        0        0     1182 2023-07-03 06:57:55.167055 makolator-2.0.2/makolator/__main__.py
--rw-r--r--   0        0        0     8305 2023-07-03 06:57:55.167055 makolator-2.0.2/makolator/_inplace.py
--rw-r--r--   0        0        0     4189 2023-07-03 06:57:55.167055 makolator-2.0.2/makolator/cli.py
--rw-r--r--   0        0        0     2209 2023-07-03 06:57:55.167055 makolator-2.0.2/makolator/config.py
--rw-r--r--   0        0        0     2004 2023-07-03 06:57:55.167055 makolator-2.0.2/makolator/datamodel.py
--rw-r--r--   0        0        0      897 2023-07-03 06:57:55.167055 makolator-2.0.2/makolator/escape.py
--rw-r--r--   0        0        0      106 2023-07-03 06:57:55.167055 makolator-2.0.2/makolator/exceptions.py
--rw-r--r--   0        0        0     7662 2023-07-03 06:57:55.167055 makolator-2.0.2/makolator/makolator.py
--rw-r--r--   0        0        0     2290 2023-07-03 06:57:55.167055 makolator-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     1915 1970-01-01 00:00:00.000000 makolator-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-04 21:52:11.733199 makolator-2.0.3/LICENSE
+-rw-r--r--   0        0        0     1223 2023-07-04 21:52:11.733199 makolator-2.0.3/README.md
+-rw-r--r--   0        0        0     5038 2023-07-04 21:52:11.733199 makolator-2.0.3/makolator/__init__.py
+-rw-r--r--   0        0        0     1182 2023-07-04 21:52:11.733199 makolator-2.0.3/makolator/__main__.py
+-rw-r--r--   0        0        0     8305 2023-07-04 21:52:11.733199 makolator-2.0.3/makolator/_inplace.py
+-rw-r--r--   0        0        0     1456 2023-07-04 21:52:11.733199 makolator-2.0.3/makolator/_util.py
+-rw-r--r--   0        0        0     4250 2023-07-04 21:52:11.733199 makolator-2.0.3/makolator/cli.py
+-rw-r--r--   0        0        0     2209 2023-07-04 21:52:11.733199 makolator-2.0.3/makolator/config.py
+-rw-r--r--   0        0        0     2004 2023-07-04 21:52:11.733199 makolator-2.0.3/makolator/datamodel.py
+-rw-r--r--   0        0        0     2006 2023-07-04 21:52:11.733199 makolator-2.0.3/makolator/escape.py
+-rw-r--r--   0        0        0     1215 2023-07-04 21:52:11.733199 makolator-2.0.3/makolator/exceptions.py
+-rw-r--r--   0        0        0     1902 2023-07-04 21:52:11.733199 makolator-2.0.3/makolator/info.py
+-rw-r--r--   0        0        0     8977 2023-07-04 21:52:11.733199 makolator-2.0.3/makolator/makolator.py
+-rw-r--r--   0        0        0     2348 2023-07-04 21:52:11.733199 makolator-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1915 1970-01-01 00:00:00.000000 makolator-2.0.3/PKG-INFO
```

### Comparing `makolator-2.0.2/LICENSE` & `makolator-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `makolator-2.0.2/README.md` & `makolator-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `makolator-2.0.2/makolator/__init__.py` & `makolator-2.0.3/makolator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,8 +178,9 @@
 # pylint: disable=unused-import
 from outputfile import Existing
 
 from .config import Config
 from .datamodel import Datamodel
 from .escape import tex
 from .exceptions import MakolatorError
+from .info import Info, get_cli
 from .makolator import Makolator
```

### Comparing `makolator-2.0.2/makolator/__main__.py` & `makolator-2.0.3/makolator/__main__.py`

 * *Files identical despite different names*

### Comparing `makolator-2.0.2/makolator/_inplace.py` & `makolator-2.0.3/makolator/_inplace.py`

 * *Files identical despite different names*

### Comparing `makolator-2.0.2/makolator/cli.py` & `makolator-2.0.3/makolator/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 """
 Command Line Interface.
 """
 import argparse
 from pathlib import Path
 
-from makolator import Config, Existing, Makolator
+from makolator import Config, Existing, Info, Makolator, get_cli
 
 
 def main(args=None):
     """Command Line Interface Processing."""
     parser = argparse.ArgumentParser(
         prog="makolator",
         description="Mako Templates (https://www.makotemplates.org/) extended.",
@@ -106,14 +106,15 @@
     if args.cmd:
         config = Config(
             verbose=args.verbose,
             diffout=print if args.show_diff else None,
             existing=args.existing,
             template_paths=args.template_path + [Path(".")],
         )
-        mklt = Makolator(config=config)
+        info = Info(cli=get_cli())
+        mklt = Makolator(config=config, info=info)
         if args.cmd == "gen":
             mklt.gen(args.templates, args.output)
         else:
             mklt.inplace(args.templates, args.inplace, ignore_unknown=args.ignore_unknown)
     else:
         parser.print_help()
```

### Comparing `makolator-2.0.2/makolator/config.py` & `makolator-2.0.3/makolator/config.py`

 * *Files identical despite different names*

### Comparing `makolator-2.0.2/makolator/datamodel.py` & `makolator-2.0.3/makolator/datamodel.py`

 * *Files identical despite different names*

### Comparing `makolator-2.0.2/makolator/makolator.py` & `makolator-2.0.3/makolator/makolator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+#
+# MIT License
+#
+# Copyright (c) 2023 nbiotcloud
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
 """
 The Makolator.
 
 A simple API to an improved Mako.
 """
 
 import hashlib
@@ -17,17 +40,19 @@
 from mako.lookup import TemplateLookup
 from mako.runtime import Context
 from mako.template import Template
 from outputfile import Existing, open_
 from uniquer import uniquelist
 
 from ._inplace import InplaceRenderer
+from ._util import Paths, norm_paths
 from .config import Config
 from .datamodel import Datamodel
 from .exceptions import MakolatorError
+from .info import Info
 
 LOGGER = logging.getLogger("makolator")
 
 
 @define
 class Makolator:
     """
@@ -38,14 +63,17 @@
 
     config: Config = field(factory=Config)
     """The Configuration."""
 
     datamodel: Datamodel = field(factory=Datamodel)
     """The Data Container."""
 
+    info: Info = field(factory=Info)
+    """Makolator Information."""
+
     __cache_path: Optional[Path] = None
 
     def __del__(self):
         if self.__cache_path:
             rmtree(self.__cache_path)
             self.__cache_path = None
 
@@ -84,25 +112,26 @@
             try:
                 yield file
             finally:
                 file.close()
                 if self.config.verbose:
                     print(f"'{filepath!s}'... {file.state.value}")
 
-    def gen(self, template_filepaths: List[Path], dest: Optional[Path] = None, context: Optional[dict] = None):
+    def gen(self, template_filepaths: Paths, dest: Optional[Path] = None, context: Optional[dict] = None):
         """
         Render template file.
 
         Args:
             template_filepaths: Templates.
 
         Keyword Args:
             dest: Output File.
             context: Key-Value Pairs pairs forwarded to the template.
         """
+        template_filepaths = norm_paths(template_filepaths)
         LOGGER.debug("gen(%r, %r)", [str(filepath) for filepath in template_filepaths], dest)
         tplfilepaths, lookup = self._create_template_lookup(
             template_filepaths, self.config.template_paths, required=True
         )
         templates = self._create_templates(tplfilepaths, lookup)
         context = context or {}
         if dest is None:
@@ -117,15 +146,15 @@
 
     def _render(self, template: Template, output, dest: Optional[Path], context: dict):
         context = Context(output, **self._get_render_context(dest, context))
         template.render_context(context)
 
     def inplace(
         self,
-        template_filepaths: List[Path],
+        template_filepaths: Paths,
         filepath: Path,
         context: Optional[dict] = None,
         ignore_unknown: bool = False,
     ):
         """
         Update generated code within `filename` between BEGIN/END markers.
 
@@ -133,14 +162,15 @@
             template_filepaths: Templates.
             dest: File to update.
 
         Keyword Args:
             context: Key-Value Pairs pairs forwarded to the template.
             ignore_unknown: Ignore unknown inplace markers, instead of raising an error.
         """
+        template_filepaths = norm_paths(template_filepaths)
         LOGGER.debug("inplace(%r, %r)", [str(filepath) for filepath in template_filepaths], filepath)
         tplfilepaths, lookup = self._create_template_lookup(template_filepaths, self.config.template_paths)
         templates = tuple(self._create_templates(tplfilepaths, lookup))
         config = self.config
         context = context or {}
         inplace = InplaceRenderer(config.template_marker, config.inplace_marker, templates, ignore_unknown, context)
         with self.open_outputfile(filepath, existing=Existing.KEEP_TIMESTAMP, newline="") as outputfile:
@@ -197,16 +227,15 @@
         if not found and required:
             raise MakolatorError(f"None of the templates {_humanify(filepaths)} found at {_humanify(searchpaths)}.")
 
     def _get_render_context(self, output_filepath: Optional[Path], context: dict) -> dict:
         result = {
             "datamodel": self.datamodel,
             "output_filepath": output_filepath,
-            "gen": self.gen,
-            "inplace": self.inplace,
+            "makolator": self,
         }
         result.update(context)
         return result
 
 
 def _humanify(iterable):
     if iterable:
```

### Comparing `makolator-2.0.2/pyproject.toml` & `makolator-2.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "makolator"
-version = "2.0.2"
+version = "2.0.3"
 description = "Extended Mako Templates for Python"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -32,14 +32,15 @@
 uniquer = "^1.0.0"
 
 [tool.poetry.group.test.dependencies]
 black = '^23.3.0'
 coverage = '^6.4.4'
 isort = '^5.9'
 mypy = "^1.3.0"
+nbcpychecker = '^1.0.0'
 pylint = '^2.15'
 pytest = '^7.3'
 
 [tool.poetry.group.doc.dependencies]
 sphinx = '^5.1.1'
 sphinx-rtd-theme = "^1.0.0"
 sphinxemoji = ">=0.2.0"
@@ -108,8 +109,9 @@
     poetry run coverage run -a --source=makolator --branch -m makolator
     poetry run coverage report
     poetry run coverage html
     poetry run coverage xml
     poetry run pylint makolator tests
     poetry run mypy makolator
     poetry run make html -C docs
+    poetry run nbcpychecker check
 """
```

### Comparing `makolator-2.0.2/PKG-INFO` & `makolator-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makolator
-Version: 2.0.2
+Version: 2.0.3
 Summary: Extended Mako Templates for Python
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

