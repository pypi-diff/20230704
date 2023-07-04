# Comparing `tmp/rez_pip-0.1.0.tar.gz` & `tmp/rez_pip-0.2.0.tar.gz`

## Comparing `rez_pip-0.1.0.tar` & `rez_pip-0.2.0.tar`

### file list

```diff
@@ -1,43 +1,51 @@
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 rez_pip-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0    14255 2020-02-02 00:00:00.000000 rez_pip-0.1.0/NOTES.md
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 rez_pip-0.1.0/codecov.yml
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 rez_pip-0.1.0/mypy.ini
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 rez_pip-0.1.0/noxfile.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 rez_pip-0.1.0/pytest.ini
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 rez_pip-0.1.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 rez_pip-0.1.0/docs/make.bat
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 rez_pip-0.1.0/docs/requirements.txt
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 rez_pip-0.1.0/docs/source/conf.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 rez_pip-0.1.0/docs/source/faq.rst
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 rez_pip-0.1.0/docs/source/index.rst
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 rez_pip-0.1.0/docs/source/installation.rst
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 rez_pip-0.1.0/docs/source/package_structure.rst
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 rez_pip-0.1.0/docs/source/transition.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 rez_pip-0.1.0/docs/source/user_guide.rst
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 rez_pip-0.1.0/scripts/download_pip.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rez_pip-0.1.0/src/rez_pip/__init__.py
--rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 rez_pip-0.1.0/src/rez_pip/__main__.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 rez_pip-0.1.0/src/rez_pip/download.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 rez_pip-0.1.0/src/rez_pip/exceptions.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 rez_pip-0.1.0/src/rez_pip/install.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 rez_pip-0.1.0/src/rez_pip/pip.py
--rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 rez_pip-0.1.0/src/rez_pip/rez.py
--rw-r--r--   0        0        0    23742 2020-02-02 00:00:00.000000 rez_pip-0.1.0/src/rez_pip/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rez_pip-0.1.0/src/rez_pip/data/__init__.py
--rw-r--r--   0        0        0  2034201 2020-02-02 00:00:00.000000 rez_pip-0.1.0/src/rez_pip/data/pip.pyz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rez_pip-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 rez_pip-0.1.0/tests/_test_integration.py
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 rez_pip-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 rez_pip-0.1.0/tests/requirements.txt
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 rez_pip-0.1.0/tests/simpleindex.toml
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 rez_pip-0.1.0/tests/test_download.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 rez_pip-0.1.0/tests/test_install.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 rez_pip-0.1.0/tests/test_integration.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 rez_pip-0.1.0/tests/test_pip.py
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 rez_pip-0.1.0/tests/test_rez.py
--rw-r--r--   0        0        0     8346 2020-02-02 00:00:00.000000 rez_pip-0.1.0/tests/test_utils.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 rez_pip-0.1.0/.gitignore
--rw-r--r--   0        0        0    11351 2020-02-02 00:00:00.000000 rez_pip-0.1.0/LICENSE
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 rez_pip-0.1.0/README.md
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 rez_pip-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    17021 2020-02-02 00:00:00.000000 rez_pip-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 rez_pip-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 rez_pip-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    14255 2020-02-02 00:00:00.000000 rez_pip-0.2.0/NOTES.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 rez_pip-0.2.0/codecov.yml
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 rez_pip-0.2.0/mypy.ini
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 rez_pip-0.2.0/noxfile.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 rez_pip-0.2.0/pytest.ini
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 rez_pip-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 rez_pip-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 rez_pip-0.2.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 rez_pip-0.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 rez_pip-0.2.0/docs/source/faq.rst
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 rez_pip-0.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 rez_pip-0.2.0/docs/source/metadata.rst
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 rez_pip-0.2.0/docs/source/transition.rst
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 rez_pip-0.2.0/docs/source/user_guide.rst
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 rez_pip-0.2.0/scripts/download_pip.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rez_pip-0.2.0/src/rez_pip/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 rez_pip-0.2.0/src/rez_pip/__main__.py
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 rez_pip-0.2.0/src/rez_pip/cli.py
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 rez_pip-0.2.0/src/rez_pip/download.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 rez_pip-0.2.0/src/rez_pip/exceptions.py
+-rw-r--r--   0        0        0     7382 2020-02-02 00:00:00.000000 rez_pip-0.2.0/src/rez_pip/install.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 rez_pip-0.2.0/src/rez_pip/pip.py
+-rw-r--r--   0        0        0     9020 2020-02-02 00:00:00.000000 rez_pip-0.2.0/src/rez_pip/rez.py
+-rw-r--r--   0        0        0    23742 2020-02-02 00:00:00.000000 rez_pip-0.2.0/src/rez_pip/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rez_pip-0.2.0/src/rez_pip/data/__init__.py
+-rw-r--r--   0        0        0  2034201 2020-02-02 00:00:00.000000 rez_pip-0.2.0/src/rez_pip/data/pip.pyz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     8197 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/constraints.txt
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/requirements.txt
+-rw-r--r--   0        0        0    10118 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/test_cli.py
+-rw-r--r--   0        0        0    13313 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/test_download.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/test_install.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/test_integration.py
+-rw-r--r--   0        0        0     5860 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/test_pip.py
+-rw-r--r--   0        0        0     8628 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/test_rez.py
+-rw-r--r--   0        0        0     8346 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/utils.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/data/src_packages/console_scripts/pyproject.toml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/data/src_packages/console_scripts/src/console_scripts/__init__.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/data/src_packages/package_a/pyproject.toml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/data/src_packages/package_a/src/console_scripts/__init__.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/data/src_packages/package_b/pyproject.toml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 rez_pip-0.2.0/tests/data/src_packages/package_b/src/console_scripts/__init__.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 rez_pip-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11351 2020-02-02 00:00:00.000000 rez_pip-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 rez_pip-0.2.0/README.md
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 rez_pip-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    17151 2020-02-02 00:00:00.000000 rez_pip-0.2.0/PKG-INFO
```

### Comparing `rez_pip-0.1.0/NOTES.md` & `rez_pip-0.2.0/NOTES.md`

 * *Files identical despite different names*

### Comparing `rez_pip-0.1.0/noxfile.py` & `rez_pip-0.2.0/noxfile.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def lint(session: nox.Session):
     pass
 
 
 @nox.session()
 def mypy(session: nox.Session):
     session.install("mypy")
-    session.install(".")
+    session.install(".", "-c", "tests/constraints.txt")
 
     session.run("mypy")
 
 
 @nox.session()
 def format(session: nox.Session):
     session.install("black")
```

### Comparing `rez_pip-0.1.0/docs/Makefile` & `rez_pip-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rez_pip-0.1.0/docs/make.bat` & `rez_pip-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rez_pip-0.1.0/docs/source/conf.py` & `rez_pip-0.2.0/docs/source/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,18 +14,26 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     # first-party extensions
     "sphinx.ext.autodoc",
     "sphinx.ext.extlinks",
     "sphinx.ext.intersphinx",
+    "sphinx.ext.autosectionlabel",
+    # Third-part
+    "sphinx_inline_tabs",
 ]
 
 templates_path = ["_templates"]
 exclude_patterns = []
 
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "furo"
 html_static_path = ["_static"]
+
+# -- Options for sphinx.ext.autosectionlabel ---------------------------------
+# https://www.sphinx-doc.org/en/master/usage/extensions/autosectionlabel.html
+
+autosectionlabel_prefix_document = True
```

### Comparing `rez_pip-0.1.0/scripts/download_pip.py` & `rez_pip-0.2.0/scripts/download_pip.py`

 * *Files identical despite different names*

### Comparing `rez_pip-0.1.0/src/rez_pip/__main__.py` & `rez_pip-0.2.0/src/rez_pip/install.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,203 +1,206 @@
+"""
+Code that takes care of installing (extracting) wheels.
+"""
+import io
 import os
 import sys
-import shutil
 import typing
+import zipfile
 import logging
-import argparse
 import pathlib
-import tempfile
+import sysconfig
 
 if sys.version_info >= (3, 10):
     import importlib.metadata as importlib_metadata
 else:
     import importlib_metadata
 
-import rich
-import rich.markup
-import rich.logging
-import rez.vendor.version.version
-
-import rez_pip.pip
-import rez_pip.rez
-import rez_pip.data
-import rez_pip.install
-import rez_pip.download
-import rez_pip.exceptions
-
-_LOG = logging.getLogger("rez_pip")
-
-
-def parseArgs() -> typing.Tuple[argparse.Namespace, typing.List[str]]:
-    parser = argparse.ArgumentParser(
-        description="Ingest and convert python packages to rez packages.",
-        add_help=False,
-    )
-    parser.add_argument("packages", nargs="*", help="Packages to install.")
-
-    generalGroup = parser.add_argument_group(title="general options")
-    generalGroup.add_argument(
-        "-r",
-        "--requirement",
-        action="append",
-        metavar="<file>",
-        help="Install from the given requirements file. This option can be used multiple times.",
-    )
-    generalGroup.add_argument(
-        "-c",
-        "--constraint",
-        action="append",
-        metavar="<file>",
-        help="Constrain versions using the given constraints file. This option can be used multiple times.",
-    )
-    generalGroup.add_argument(
-        "--install-path",
-        metavar="<path>",
-        help="Technically this should be --target",
-    )
-
-    generalGroup.add_argument(
-        "--python-version",
-        metavar="<version>",
-        help="Range of python versions. It can also be a single version or 'latest'",
-    )
-    generalGroup.add_argument(
-        "--pip",
-        default=os.path.join(os.path.dirname(rez_pip.data.__file__), "pip.pyz"),
-        metavar="<path>",
-        help="Standalone pip (https://pip.pypa.io/en/stable/installation/#standalone-zip-application) (default: bundled).",
-    )
-
-    # Manually define just to keep the style consistent (capital letters, dot, etc.)
-    generalGroup.add_argument(
-        "-h", "--help", action="help", help="Show this help message and exit."
-    )
-
-    debugGroup = parser.add_argument_group(title="debug options")
-    debugGroup.add_argument(
-        "-l",
-        "--log-level",
-        default="info",
-        choices=["info", "debug", "warning", "error"],
-        help="Logging level.",
-    )
-
-    debugGroup.add_argument(
-        "--keep-tmp-dirs",
-        action="store_true",
-        help="Keep some temporary directory at the end of the process for further inspection.",
-    )
-
-    parser.usage = f"""
-
-  %(prog)s [options] <package(s)>
-  %(prog)s <package(s)> [-- [pip options]]
-"""
-    knownArgs = []
-    pipArgs = []
-    if "--" in sys.argv:
-        # anything after -- will be passed as is to pip.
-        splitIndex = sys.argv[1:].index("--")
-        knownArgs = sys.argv[1:][:splitIndex]
-        pipArgs = sys.argv[1:][splitIndex + 1 :]
+if typing.TYPE_CHECKING:
+    if sys.version_info >= (3, 8):
+        from typing import Literal
     else:
-        knownArgs = sys.argv[1:]
+        from typing_extensions import Literal
 
-    args = parser.parse_args(knownArgs)
+import installer
+import installer.utils
+import installer.records
+import installer.scripts
+import installer.sources
+import installer.destinations
 
-    return args, pipArgs
+import rez_pip.pip
 
+_LOG = logging.getLogger(__name__)
 
-def _run(args: argparse.Namespace, pipArgs: typing.List[str], pipWorkArea: str) -> None:
-    if not args.pip.endswith(".pyz"):
-        raise rez_pip.exceptions.RezPipError(
-            f"[bold red]{args.pip!r} does not look like a valid zipapp. A zipapp should end with '.pyz'.[/]\n\n"
-            "  [grey74]Standalone pip documentation[/]: https://pip.pypa.io/en/stable/installation/#standalone-zip-application\n"
-            "  [grey74]zipapp documentation[/]: https://docs.python.org/3/library/zipapp.html"
+if typing.TYPE_CHECKING:
+    LauncherKind = Literal["posix", "win-ia32", "win-amd64", "win-arm", "win-arm64"]
+    ScriptSection = Literal["console", "gui"]
+
+
+def isWheelPure(source: installer.sources.WheelSource) -> bool:
+    stream = source.read_dist_info("WHEEL")
+    metadata = installer.utils.parse_metadata_file(stream)
+    return typing.cast(str, metadata["Root-Is-Purelib"]) == "true"
+
+
+# Taken from https://github.com/pypa/installer/blob/main/src/installer/__main__.py#L49
+def getSchemeDict(name: str, target: str) -> typing.Dict[str, str]:
+    vars = {}
+    vars["base"] = vars["platbase"] = installed_base = target
+
+    schemeDict = sysconfig.get_paths(vars=vars)
+    # calculate 'headers' path, not currently in sysconfig - see
+    # https://bugs.python.org/issue44445. This is based on what distutils does.
+    # TODO: figure out original vs normalised distribution names
+    schemeDict["headers"] = os.path.join(
+        sysconfig.get_path("include", vars={"installed_base": installed_base}),
+        name,
+    )
+
+    if target:  # In practice this will always be set.
+        schemeDict["purelib"] = os.path.join(target, "python")
+        schemeDict["platlib"] = os.path.join(target, "python")
+        schemeDict["headers"] = os.path.join(target, "headers", name)
+        schemeDict["scripts"] = os.path.join(target, "scripts")
+        # Potentiall handle data?
+    return schemeDict
+
+
+def installWheel(
+    package: rez_pip.pip.PackageInfo,
+    wheelPath: pathlib.Path,
+    targetPath: str,
+) -> typing.Tuple[importlib_metadata.Distribution, bool]:
+    # TODO: Technically, target should be optional. We will always want to install in "pip install --target"
+    #       mode. So right now it's a CLI option for debugging purposes.
+
+    destination = CustomWheelDestination(
+        getSchemeDict(package.name, targetPath),
+        # TODO: Use Python from rez package, or simply use "/usr/bin/env python"?
+        interpreter=sys.executable,
+        script_kind=installer.utils.get_launcher_kind(),
+    )
+
+    isPure = True
+    _LOG.debug(f"Installing {wheelPath} into {targetPath!r}")
+    with installer.sources.WheelFile.open(wheelPath) as source:
+        isPure = isWheelPure(source)
+
+        installer.install(
+            source=source,
+            destination=destination,
+            # Additional metadata that is generated by the installation tool.
+            additional_metadata={
+                "INSTALLER": f"rez-pip {importlib_metadata.version(__package__)}".encode(
+                    "utf-8"
+                ),
+            },
         )
 
-    if not os.path.exists(args.pip):
-        raise rez_pip.exceptions.RezPipError(f"zipapp at {args.pip!r} does not exists")
+    targetPathPython = os.path.join(targetPath, "python")
 
-    if not args.packages and not args.requirement:
-        raise rez_pip.exceptions.RezPipError(
-            "no packages were passed and --requirements was not used. At least one of the must be passed."
+    # That's kind of dirty, but using any other method returns inconsistent results.
+    # For example, importlib.metadata.Distribution.discover(path=['/path']) sometimes
+    # won't find the freshly intalled package, even if it exists and everything.
+    path = os.path.join(
+        targetPathPython,
+        f"{package.name.replace('-', '_')}-{package.version}.dist-info",
+    )
+    dist = importlib_metadata.Distribution.at(path)
+
+    if not dist.files:
+        path = os.path.join(
+            targetPathPython,
+            # Some packages like sphinx will have have a sphinx.dist-info instead of Sphinx.dist-info.
+            f"{package.name.replace('-', '_').lower()}-{package.version}.dist-info",
         )
+        dist = importlib_metadata.Distribution.at(path)
+        if not dist.files:
+            raise RuntimeError(f"{path!r} does not exist!")
+
+    return dist, isPure
+
+
+# TODO: Document where this code comes from.
+class CustomWheelDestination(installer.destinations.SchemeDictionaryDestination):
+    # Exactly the same as SchemeDictionaryDestination, but uses our custom Script class.
+    def write_script(
+        self, name: str, module: str, attr: str, section: "ScriptSection"
+    ) -> installer.records.RecordEntry:
+        """Write a script to invoke an entrypoint.
+        :param name: name of the script
+        :param module: module path, to load the entry point from
+        :param attr: final attribute access, for the entry point
+        :param section: Denotes the "entry point section" where this was specified.
+            Valid values are ``"gui"`` and ``"console"``.
+        :type section: str
+        - Generates a launcher using :any:`Script.generate`.
+        - Writes to the "scripts" scheme.
+        - Uses :py:meth:`SchemeDictionaryDestination.write_to_fs` for the
+          filesystem interaction.
+        """
+        script = Script(name, module, attr, section)
+        script_name, data = script.generate(self.interpreter, self.script_kind)
+
+        with io.BytesIO(data) as stream:
+            entry = self.write_to_fs(
+                installer.utils.Scheme("scripts"),
+                script_name,
+                stream,
+                is_executable=True,
+            )
 
-    pythonVersions = rez_pip.rez.getPythonExecutables(
-        args.python_version, packageFamily="python"
-    )
-
-    for pythonVersion, pythonExecutable in pythonVersions.items():
-        wheelsDir = os.path.join(pipWorkArea, "wheels")
-        os.mkdir(wheelsDir)
-
-        installedWheelsDir = os.path.join(pipWorkArea, "installed")
-        os.mkdir(installedWheelsDir)
-
-        with rich.get_console().status(
-            f"[bold]Resolving dependencies for {rich.markup.escape(', '.join(args.packages))} (python-{pythonVersion})"
-        ):
-            packages = rez_pip.pip.get_packages(
-                args.packages,
-                args.pip,
-                pythonVersion,
-                pythonExecutable,
-                args.requirement or [],
-                args.constraint or [],
-                pipArgs,
+            path = self._path_with_destdir(
+                installer.utils.Scheme("scripts"), script_name
             )
+            mode = os.stat(path).st_mode
+            mode |= (mode & 0o444) >> 2
+            os.chmod(path, mode)
+
+            return entry
+
+
+_SCRIPT_TEMPLATE = """\
+# -*- coding: utf-8 -*-
+import re
+import sys
+from {module} import {import_name}
+if __name__ == "__main__":
+    sys.argv[0] = re.sub(r"(-script\\.pyw|\\.exe)?$", "", sys.argv[0])
+    sys.exit({func_path}())
+"""
 
-        _LOG.info(f"Resolved {len(packages)} dependencies")
 
-        # TODO: Should we postpone downloading to the last minute if we can?
-        _LOG.info("[bold]Downloading...")
-        wheels = rez_pip.download.downloadPackages(packages, wheelsDir)
-        _LOG.info(f"[bold]Downloaded {len(wheels)} wheels")
-
-        dists: typing.Dict[importlib_metadata.Distribution, bool] = {}
-
-        with rich.get_console().status(
-            f"[bold]Installing wheels into {installedWheelsDir!r}"
-        ):
-            for package, wheel in zip(packages, wheels):
-                _LOG.info(f"[bold]Installing {package.name}-{package.version} wheel")
-                dist, isPure = rez_pip.install.installWheel(
-                    package, pathlib.Path(wheel), installedWheelsDir
-                )
-
-                dists[dist] = isPure
-
-        distNames = [dist.name for dist in dists.keys()]
-
-        with rich.get_console().status("[bold]Creating rez packages..."):
-            for dist in dists:
-                isPure = dists[dist]
-                rez_pip.rez.createPackage(
-                    dist,
-                    isPure,
-                    rez.vendor.version.version.Version(pythonVersion),
-                    distNames,
-                    installedWheelsDir,
-                    args.install_path,
-                )
-
-
-def run() -> None:
-    args, pipArgs = parseArgs()
-
-    handler = rich.logging.RichHandler(show_time=False, markup=True, show_path=False)
-    handler.setFormatter(logging.Formatter(fmt="%(message)s"))
-    _LOG.addHandler(handler)
-    _LOG.setLevel(args.log_level.upper())
-
-    pipWorkArea = tempfile.mkdtemp(prefix="rez-pip-target")
-
-    try:
-        _run(args, pipArgs, pipWorkArea)
-    except rez_pip.exceptions.RezPipError as exc:
-        rich.get_console().print(exc, soft_wrap=True)
-        sys.exit(1)
-    finally:
-        if not args.keep_tmp_dirs:
-            _LOG.info(f"Removing {pipWorkArea}")
-            shutil.rmtree(pipWorkArea)
+# TODO: Document where this code comes from.
+class Script(installer.scripts.Script):
+    def generate(
+        self, executable: str, kind: "LauncherKind"
+    ) -> typing.Tuple[str, bytes]:
+        """Generate a launcher for this script.
+        :param executable: Path to the executable to invoke.
+        :param kind: Which launcher template should be used.
+            Valid values are ``"posix"``, ``"win-ia32"``, ``"win-amd64"`` and
+            ``"win-arm"``.
+        :type kind: str
+        :raises InvalidScript: if no appropriate template is available.
+        :return: The name and contents of the launcher file.
+        """
+        launcher = self._get_launcher_data(kind)
+        # shebang = _build_shebang(executable, forlauncher=bool(launcher))
+        # TODO: Should we instead just pass that value to WheelDestination?
+        shebang = b"#!/usr/bin/env python"
+        code = _SCRIPT_TEMPLATE.format(
+            module=self.module,
+            import_name=self.attr.split(".")[0],
+            func_path=self.attr,
+        ).encode("utf-8")
+
+        if launcher is None:
+            return (self.name, shebang + b"\n" + code)
+
+        stream = io.BytesIO()
+        with zipfile.ZipFile(stream, "w") as zf:
+            zf.writestr("__main__.py", code)
+        name = f"{self.name}.exe"
+        data = launcher + shebang + b"\n" + stream.getvalue()
+        return (name, data)
```

### Comparing `rez_pip-0.1.0/src/rez_pip/download.py` & `rez_pip-0.2.0/src/rez_pip/download.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import typing
 import asyncio
+import hashlib
 import logging
 
 import rich
 import aiohttp
 import rich.progress
 
 import rez_pip.pip
@@ -44,79 +45,105 @@
                 tasks[package.name] = progress.add_task(package.name)
 
             # Then create the "total" progress bar. This ensures that total is at the bottom.
             mainTask = progress.add_task(f"[bold]Total (0/{len(packages)})", total=0)
 
             for package in packages:
                 items.append(
-                    download(
+                    _download(
                         package, dest, session, progress, tasks[package.name], mainTask
                     )
                 )
 
             wheels = await asyncio.gather(*items)
 
     if not all(wheels):
         raise RuntimeError("Some wheels failed to be downloaded")
 
     return wheels
 
 
-async def download(
+def getSHA256(path: str) -> str:
+    buf = bytearray(2**18)  # Reusable buffer to reduce allocations.
+    view = memoryview(buf)
+
+    digestobj = hashlib.new("sha256")
+
+    with open(path, "rb") as fd:
+        while True:
+            size = fd.readinto(buf)
+            if size == 0:
+                break  # EOF
+            digestobj.update(view[:size])
+
+    return digestobj.hexdigest()
+
+
+async def _download(
     package: rez_pip.pip.PackageInfo,
     target: str,
     session: aiohttp.ClientSession,
     progress: rich.progress.Progress,
     taskID: rich.progress.TaskID,
     mainTaskID: rich.progress.TaskID,
 ) -> typing.Optional[str]:
-    _LOG.debug(
-        f"Downloading {package.name}-{package.version} from {package.download_info.url}"
-    )
-
-    async with session.get(
-        package.download_info.url,
-        headers={
-            "Content-Type": "application/octet-stream",
-            "User-Agent": "rez-pip/0.1.0",
-        },
-    ) as response:
-        size = int(response.headers.get("content-length", 0))
-        progress.update(taskID, total=size)
-
-        async with _lock:
-            mainTask = [task for task in progress.tasks if task.id == mainTaskID][0]
-
-            progress.update(
-                mainTaskID,
-                total=typing.cast(int, mainTask.total) + size,
-            )
+    wheelName: str = os.path.basename(package.download_info.url)
+    wheelPath = os.path.join(target, wheelName)
 
-        if response.status != 200:
-            _LOG.error(
-                f"failed to download {package.download_info.url}: {response.status} - {response.reason}, {response.request_info}"
-            )
-            return None
+    # TODO: Handle case where sha256 doesn't exist. We should also support the other supported
+    # hash types.
+    if (
+        os.path.exists(wheelPath)
+        and getSHA256(wheelPath) == package.download_info.archive_info.hashes["sha256"]
+    ):
+        _LOG.info(f"{wheelName} found in cache at {wheelPath!r}. Skipping download.")
+    else:
+        _LOG.debug(
+            f"Downloading {package.name}-{package.version} from {package.download_info.url}"
+        )
+
+        async with session.get(
+            package.download_info.url,
+            headers={
+                "Content-Type": "application/octet-stream",
+                "User-Agent": "rez-pip/0.1.0",
+            },
+        ) as response:
+            size = int(response.headers.get("content-length", 0))
+            progress.update(taskID, total=size)
+
+            async with _lock:
+                mainTask = [task for task in progress.tasks if task.id == mainTaskID][0]
+
+                progress.update(
+                    mainTaskID,
+                    total=typing.cast(int, mainTask.total) + size,
+                )
 
-        wheelName: str = os.path.basename(package.download_info.url)
-        wheelPath = os.path.join(target, wheelName)
-        with open(wheelPath, "wb") as fd:
-            async for chunk, asd in response.content.iter_chunks():
-                if not chunk:
-                    break
-                progress.update(taskID, advance=len(chunk))
-                progress.update(mainTaskID, advance=len(chunk))
-                fd.write(chunk)
+            if response.status != 200:
+                _LOG.error(
+                    f"failed to download {package.download_info.url}: {response.status} - {response.reason}, {response.request_info}"
+                )
+                return None
+
+            with open(wheelPath, "wb") as fd:
+                async for chunk, asd in response.content.iter_chunks():
+                    if not chunk:
+                        break
+                    progress.update(taskID, advance=len(chunk))
+                    progress.update(mainTaskID, advance=len(chunk))
+                    fd.write(chunk)
+
+            _LOG.info(
+                f"Downloaded {package.name}-{package.version} to {wheelPath!r} ({os.stat(wheelPath).st_size} bytes)"
+            )
 
     progress.update(taskID, visible=False)
 
     total = len(progress.tasks) - 1
     async with _lock:
         completedItems = [task for task in progress.tasks if not task.visible]
         progress.update(
             mainTaskID, description=f"[bold]Total ({len(completedItems)}/{total})"
         )
-    _LOG.info(
-        f"Downloaded {package.name}-{package.version} to {wheelPath!r} ({os.stat(wheelPath).st_size} bytes)"
-    )
 
     return wheelPath
```

### Comparing `rez_pip-0.1.0/src/rez_pip/utils.py` & `rez_pip-0.2.0/src/rez_pip/utils.py`

 * *Files identical despite different names*

### Comparing `rez_pip-0.1.0/src/rez_pip/data/pip.pyz` & `rez_pip-0.2.0/src/rez_pip/data/pip.pyz`

 * *Files identical despite different names*

### Comparing `rez_pip-0.1.0/tests/test_integration.py` & `rez_pip-0.2.0/tests/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 @pytest.mark.skipif(
     platform.system() == "Darwin" and not os.environ.get("CI"),
     reason="Skipping when running locally on macOS",
 )
 @pytest.mark.integration
 def test_python_packages(pythonRezPackage: str, rezRepo: str):
-    """Test that the python rez packages created by createPythonRezPackages are functional"""
+    """Test that the python rez packages created by the pythonRezPackage fixture are functional"""
 
     package = rez.packages.get_package("python", pythonRezPackage, paths=[rezRepo])
     assert package
 
     ctx = rez.resolved_context.ResolvedContext(
         [package.qualified_name], package_paths=[rezRepo]
     )
```

### Comparing `rez_pip-0.1.0/tests/test_utils.py` & `rez_pip-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rez_pip-0.1.0/LICENSE` & `rez_pip-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rez_pip-0.1.0/README.md` & `rez_pip-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 ## TODOs
 
 * [x] Install packages without using pip
 * [x] Specify Python version to use
 * [ ] Better logs and CLI experience
     * [x] Use logging
     * [x] Progress bars for download?
-* [ ] Confirm that Python 2 is supported
-* [ ] Confirm that the theory works as expected
-* [ ] Windows support
+* [x] Confirm that Python 2 is supported
+    * It is not...
+* [x] Confirm that the theory works as expected
+* [x] Windows support
 * [ ] Hook into rez
     * [x] Install each package in a different `--target`
     * [x] Create rez package
     * [x] Copy distribution files to rez package.
     * [ ] Make it available as a rez plugin/sub-command
     * [ ] Discover Python package using rez and use that when available. I think it's still fine to support non-rezified Python interpreters though.
     * [ ] Only download+convert package if it's not already in the rez repositories.
     * etc
 * [x] Accept multiple package names as input
-* [ ] Accept requirements files as input
-* [ ] Accept whee files as input
+* [x] Accept requirements files as input
+* [ ] Accept wheel files as input
 * [ ] Properly support platform tags (wheels tags) so that GLIBC is respected, min macOS is also supported.
 * [ ] Correctly handle Requires-Python metadata.
 * [ ] Review all TODOs in the code.
 * What whould we do with `rez.system` and `rez.vendor.version`?
 * [ ] Gather a list of problematic packages from GitHub and test against them.
 * [ ] Go through GitHub issues and summarize what needs to be covered by the new rez-pip.
 * [ ] Support abi3 wheels (to avoid having to re-install C extensions for every python version).
```

### Comparing `rez_pip-0.1.0/pyproject.toml` & `rez_pip-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rez-pip"
-version = "0.1.0"
+version = "0.2.0"
 description = "Modern rez-pip"
 authors = [
     { name="Jean-Christophe Morin", email="jean_christophe_morin@hotmail.com" },
 ]
 license = { file="LICENSE" }
 readme = "README.md"
 requires-python = ">=3.7"
@@ -26,23 +26,25 @@
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "Natural Language :: English"
 ]
 keywords = []
 
 [project.urls]
 Homepage = "https://github.com/JeanChristopheMorinPerso/rez-pip"
 Tracker = "https://github.com/JeanChristopheMorinPerso/rez-pip/issues"
+Documentation = "https://rez-pip.readthedocs.io"
 
 [project.scripts]
-rez-pip2 = "rez_pip.__main__:run"
+rez-pip2 = "rez_pip.cli:run"
 
 [tool.hatch.build.targets.sdist]
 # Ensure the sdist includes a setup.py for older pip versions
 # support-legacy = true
 exclude = [".github"]
```

### Comparing `rez_pip-0.1.0/PKG-INFO` & `rez_pip-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: rez-pip
-Version: 0.1.0
+Version: 0.2.0
 Summary: Modern rez-pip
 Project-URL: Homepage, https://github.com/JeanChristopheMorinPerso/rez-pip
 Project-URL: Tracker, https://github.com/JeanChristopheMorinPerso/rez-pip/issues
+Project-URL: Documentation, https://rez-pip.readthedocs.io
 Author-email: Jean-Christophe Morin <jean_christophe_morin@hotmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -212,14 +213,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: aiohttp
 Requires-Dist: dataclasses-json
 Requires-Dist: importlib-metadata>=4.6; python_version < '3.10'
 Requires-Dist: installer>=0.7.0
 Requires-Dist: packaging>=23.1
 Requires-Dist: rez
@@ -234,28 +236,29 @@
 ## TODOs
 
 * [x] Install packages without using pip
 * [x] Specify Python version to use
 * [ ] Better logs and CLI experience
     * [x] Use logging
     * [x] Progress bars for download?
-* [ ] Confirm that Python 2 is supported
-* [ ] Confirm that the theory works as expected
-* [ ] Windows support
+* [x] Confirm that Python 2 is supported
+    * It is not...
+* [x] Confirm that the theory works as expected
+* [x] Windows support
 * [ ] Hook into rez
     * [x] Install each package in a different `--target`
     * [x] Create rez package
     * [x] Copy distribution files to rez package.
     * [ ] Make it available as a rez plugin/sub-command
     * [ ] Discover Python package using rez and use that when available. I think it's still fine to support non-rezified Python interpreters though.
     * [ ] Only download+convert package if it's not already in the rez repositories.
     * etc
 * [x] Accept multiple package names as input
-* [ ] Accept requirements files as input
-* [ ] Accept whee files as input
+* [x] Accept requirements files as input
+* [ ] Accept wheel files as input
 * [ ] Properly support platform tags (wheels tags) so that GLIBC is respected, min macOS is also supported.
 * [ ] Correctly handle Requires-Python metadata.
 * [ ] Review all TODOs in the code.
 * What whould we do with `rez.system` and `rez.vendor.version`?
 * [ ] Gather a list of problematic packages from GitHub and test against them.
 * [ ] Go through GitHub issues and summarize what needs to be covered by the new rez-pip.
 * [ ] Support abi3 wheels (to avoid having to re-install C extensions for every python version).
```

