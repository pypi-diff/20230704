# Comparing `tmp/ome_types-0.4.0a1.tar.gz` & `tmp/ome_types-0.4.0a2.tar.gz`

## Comparing `ome_types-0.4.0a1.tar` & `ome_types-0.4.0a2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    16554 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_autogen/__init__.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_autogen/__main__.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_autogen/_config.py
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_autogen/_generator.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_autogen/_transformer.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_autogen/_util.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_autogen/main.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/__init__.py
--rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/_conversion.py
--rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/ome-2016-06.xsd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/py.typed
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/units.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/_mixins/__init__.py
--rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/_mixins/_base_type.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/_mixins/_bin_data.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/_mixins/_instrument.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/_mixins/_ome.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/_mixins/_reference.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/_mixins/_structured_annotations.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/model/__init__.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/model/_color.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/model/_shape_union.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/model/_user_sequence.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/model/simple_types.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/__init__.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/bindings.py
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/compat.py
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/hooks/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/hooks/class_type.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/hooks/cli.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/LICENSE
--rw-r--r--   0        0        0     9347 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/README.md
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/hatch_build.py
--rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/pyproject.toml
--rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/PKG-INFO
+-rw-r--r--   0        0        0    16554 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_autogen/__init__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_autogen/__main__.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_autogen/_config.py
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_autogen/_generator.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_autogen/_transformer.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_autogen/_util.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_autogen/main.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/__init__.py
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/_conversion.py
+-rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/ome-2016-06.xsd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/py.typed
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/units.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/_mixins/__init__.py
+-rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/_mixins/_base_type.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/_mixins/_bin_data.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/_mixins/_instrument.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/_mixins/_ome.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/_mixins/_reference.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/_mixins/_structured_annotations.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/model/__init__.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/model/_color.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/model/_shape_union.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/model/_user_sequence.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/ome_types/model/simple_types.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/xsdata_pydantic_basemodel/__init__.py
+-rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/xsdata_pydantic_basemodel/bindings.py
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/xsdata_pydantic_basemodel/compat.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/xsdata_pydantic_basemodel/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/xsdata_pydantic_basemodel/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/xsdata_pydantic_basemodel/hooks/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/xsdata_pydantic_basemodel/hooks/class_type.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/src/xsdata_pydantic_basemodel/hooks/cli.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/LICENSE
+-rw-r--r--   0        0        0     9347 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/README.md
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/hatch_build.py
+-rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/pyproject.toml
+-rw-r--r--   0        0        0    11104 2020-02-02 00:00:00.000000 ome_types-0.4.0a2/PKG-INFO
```

### Comparing `ome_types-0.4.0a1/CHANGELOG.md` & `ome_types-0.4.0a2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/src/ome_autogen/_config.py` & `ome_types-0.4.0a2/src/ome_autogen/_config.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/src/ome_autogen/_generator.py` & `ome_types-0.4.0a2/src/ome_autogen/_generator.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, NamedTuple
 
 from xsdata.formats.dataclass.filters import Filters
 from xsdata.formats.dataclass.generator import DataclassGenerator
-from xsdata_pydantic_basemodel.generator import PydanticBaseFilters
 
 from ome_autogen import _util
+from xsdata_pydantic_basemodel.generator import PydanticBaseFilters
 
 if TYPE_CHECKING:
     from xsdata.codegen.models import Attr, Class
     from xsdata.codegen.resolver import DependenciesResolver
     from xsdata.models.config import GeneratorConfig
```

### Comparing `ome_types-0.4.0a1/src/ome_autogen/_transformer.py` & `ome_types-0.4.0a2/src/ome_autogen/_transformer.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 from xsdata.codegen.handlers import RenameDuplicateAttributes
 from xsdata.codegen.transformer import SchemaTransformer
 
 if TYPE_CHECKING:
     from xsdata.codegen.models import Class
 
 
-UNWANTED_HANDLERS = (
-    # we don't need RenameDuplicateAttributes because we inject
-    # proper enum names in our _generator.py
-    (RenameDuplicateAttributes, None),
-)
+# we don't need RenameDuplicateAttributes because we inject
+# proper enum names in our _generator.py
+UNWANTED_HANDLERS = [(RenameDuplicateAttributes, None)]
 
 
 class OMETransformer(SchemaTransformer):
     # overriding to remove the certain handlers
     def analyze_classes(self, classes: list[Class]) -> list[Class]:
         """Analyzer the given class list and simplify attributes and extensions."""
         # xsdata makes this particular class hard to extend/modify
```

### Comparing `ome_types-0.4.0a1/src/ome_autogen/_util.py` & `ome_types-0.4.0a2/src/ome_autogen/_util.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/src/ome_autogen/main.py` & `ome_types-0.4.0a2/src/ome_autogen/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,53 +24,59 @@
 ]
 
 
 def build_model(
     output_dir: Path | str = SRC_PATH,
     schema_file: Path | str = SCHEMA_FILE,
     target_package: str = OUTPUT_PACKAGE,
-    line_length: int = 88,
     ruff_ignore: list[str] = RUFF_IGNORE,
     do_formatting: bool = True,
     do_mypy: bool = DO_MYPY,
 ) -> None:
     """Convert the OME schema to a python model."""
     config = get_config(target_package)
     transformer = OMETransformer(print=False, config=config)
 
     _print_gray(f"Processing {getattr(schema_file ,'name', schema_file)}...")
     transformer.process_sources([Path(schema_file).resolve().as_uri()])
 
-    package_dir = Path(output_dir) / OUTPUT_PACKAGE.replace(".", "/")
+    package_dir = str(Path(output_dir) / OUTPUT_PACKAGE.replace(".", "/"))
     rmtree(package_dir, ignore_errors=True)
     with _util.cd(output_dir):  # xsdata doesn't support output path
         _print_gray("Writing Files...")
         transformer.process_classes()
 
     if do_formatting:
-        _print_gray("Running black and ruff ...")
+        _fix_formatting(package_dir, ruff_ignore)
 
-        black = ["black", str(package_dir), "-q", f"--line-length={line_length}"]
-        subprocess.check_call(black)  # noqa S
+    if do_mypy:
+        _check_mypy(package_dir)
 
-        ruff = ["ruff", "-q", "--fix", str(package_dir)]
-        ruff.extend(f"--ignore={ignore}" for ignore in ruff_ignore)
-        subprocess.check_call(ruff)  # noqa S
+    _print_green(f"OME python model created at {OUTPUT_PACKAGE}")
 
-    if do_mypy:
-        _print_gray("Running mypy ...")
 
-        mypy = ["mypy", str(package_dir), "--strict"]
+def _fix_formatting(package_dir: str, ruff_ignore: list[str] = RUFF_IGNORE) -> None:
+    _print_gray("Running black and ruff ...")
 
-        try:
-            subprocess.check_output(mypy, stderr=subprocess.STDOUT)  # noqa S
-        except subprocess.CalledProcessError as e:
-            raise RuntimeError(f"mypy errors:\n\n{e.output.decode()}") from e
+    black = ["black", package_dir, "-q", "--line-length=88"]
+    subprocess.check_call(black)  # noqa S
 
-    _print_green(f"OME python model created at {OUTPUT_PACKAGE}")
+    ruff = ["ruff", "-q", "--fix", package_dir]
+    ruff.extend(f"--ignore={ignore}" for ignore in ruff_ignore)
+    subprocess.check_call(ruff)  # noqa S
+
+
+def _check_mypy(package_dir: str) -> None:
+    _print_gray("Running mypy ...")
+
+    mypy = ["mypy", package_dir, "--strict"]
+    try:
+        subprocess.check_output(mypy, stderr=subprocess.STDOUT)  # noqa S
+    except subprocess.CalledProcessError as e:
+        raise RuntimeError(f"mypy errors:\n\n{e.output.decode()}") from e
 
 
 def _print_gray(text: str) -> None:
     if os.name != "nt":
         # UnicodeEncodeError: 'charmap' codec can't encode character '\u2713'
         text = f"\033[90m\033[1m{text}\033[0m"
     print(text)
```

### Comparing `ome_types-0.4.0a1/src/ome_types/__init__.py` & `ome_types-0.4.0a2/src/ome_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/src/ome_types/_conversion.py` & `ome_types-0.4.0a2/src/ome_types/_conversion.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,114 +1,174 @@
 from __future__ import annotations
 
+import importlib
+import operator
 import os
+import warnings
 from dataclasses import is_dataclass
 from pathlib import Path
 from struct import Struct
 from typing import TYPE_CHECKING, Any, cast
-from xml.etree import ElementTree as ET
+
+from ome_types.validation import validate_xml
+
+try:
+    from lxml import etree as ET
+except ImportError:  # pragma: no cover
+    from xml.etree import ElementTree as ET
 
 from xsdata.formats.dataclass.parsers.config import ParserConfig
-from xsdata.formats.dataclass.serializers.config import SerializerConfig
-from xsdata_pydantic_basemodel.bindings import XmlParser, XmlSerializer
+
+from xsdata_pydantic_basemodel.bindings import (
+    SerializerConfig,
+    XmlParser,
+    XmlSerializer,
+)
 
 if TYPE_CHECKING:
     import io
     from typing import TypedDict
 
     from xsdata.formats.dataclass.parsers.mixins import XmlHandler
-    from xsdata_pydantic_basemodel.bindings import XmlContext
 
+    from ome_types._mixins._base_type import OMEType
     from ome_types.model import OME
+    from xsdata_pydantic_basemodel.bindings import XmlContext
 
     class ParserKwargs(TypedDict, total=False):
         config: ParserConfig
         context: XmlContext
         handler: type[XmlHandler]
 
 
+__all__ = ["from_xml", "to_xml", "to_dict", "from_tiff", "tiff2xml"]
+
 OME_2016_06_URI = "http://www.openmicroscopy.org/Schemas/OME/2016-06"
-OME_2016_06_NS = f"{{{OME_2016_06_URI}}}OME"
+MODULES = {
+    OME_2016_06_URI: "ome_types._autogenerated.ome_2016_06",
+}
 
 
-def _get_ome(xml: str | bytes) -> type[OME]:
+def _get_ome_type(xml: str | bytes) -> type[OMEType]:
+    """Resolve a python model class for the root element of an OME XML document."""
     if isinstance(xml, str) and not xml.startswith("<"):
         root = ET.parse(xml).getroot()  # noqa: S314
     else:
+        if not isinstance(xml, bytes):
+            xml = xml.encode("utf-8")
         root = ET.fromstring(xml)  # noqa: S314
 
-    if root.tag == OME_2016_06_NS:
-        from ome_types.model import OME
+    *ns, localname = root.tag[1:].split("}", 1)
+    ns = next(iter(ns), None)
+
+    if not ns or ns not in MODULES:
+        raise ValueError(f"Unsupported OME schema tag {root.tag!r} in namespace {ns!r}")
 
-        return OME
-    raise ValueError(f"Unsupported OME schema tag {root.tag}")
+    mod = importlib.import_module(MODULES[ns])
+    try:
+        return getattr(mod, localname)
+    except AttributeError as e:
+        raise ValueError(
+            f"Could not find a class for {localname!r} in {mod.__name__}"
+        ) from e
 
 
 def to_dict(source: OME | Path | str | bytes) -> dict[str, Any]:
     if is_dataclass(source):
         raise NotImplementedError("dataclass -> dict is not supported yet")
+
     return from_xml(  # type: ignore[return-value]
         cast("Path | str | bytes", source),
         # the class_factory is what prevents class instantiation,
         # simply returning the params instead
         parser_kwargs={"config": ParserConfig(class_factory=lambda a, b: b)},
     )
 
 
-def _class_factory(cls: type, kwargs: Any) -> Any:
-    kwargs.setdefault("validation", "strict")
-    return cls(**kwargs)
-
-
 def from_xml(
     xml: Path | str | bytes,
     *,
-    validate: bool | None = None,  # TODO implement
-    parser: Any = None,  # TODO deprecate
+    validate: bool | None = None,
+    parser: Any = None,
     parser_kwargs: ParserKwargs | None = None,
 ) -> OME:
-    # if validate:
-    # raise NotImplementedError("validate=True is not supported yet")
+    if parser is not None:
+        warnings.warn(
+            "As of version 0.4.0, the parser argument is ignored. "
+            "lxml will be used if available in the environment, but you can "
+            "drop this keyword argument.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
+    if validate:
+        validate_xml(xml)
 
     if isinstance(xml, Path):
         xml = str(xml)
 
-    OME_type = _get_ome(xml)
-    parser_kwargs = {"config": ParserConfig(class_factory=_class_factory)}
-    _parser = XmlParser(**(parser_kwargs or {}))
+    # this cast is a lie... but it's by far the most common type that will
+    # come out of this function, and will be more useful to most users.
+    # For those who pass in an xml document that isn't just a root <OME> tag,
+    # they can cast the result to the correct type themselves.
+    OME_type = cast("type[OME]", _get_ome_type(xml))
+
+    parser_ = XmlParser(**(parser_kwargs or {}))
     if isinstance(xml, bytes):
-        return _parser.from_bytes(xml, OME_type)
+        return parser_.from_bytes(xml, OME_type)
     if os.path.isfile(xml):
-        return _parser.parse(xml, OME_type)
-    return _parser.from_string(xml, OME_type)
+        return parser_.parse(xml, OME_type)
+    return parser_.from_string(xml, OME_type)
 
 
 def to_xml(
     ome: OME,
-    ignore_defaults: bool = True,
+    *,
+    # exclude_defaults takes precendence over exclude_unset
+    # if a value equals the default, it will be excluded
+    exclude_defaults: bool = False,
+    # exclude_unset will exclude any value that is not explicitly set
+    # but will INCLUDE values that are set to their default
+    exclude_unset: bool = True,
     indent: int = 2,
+    include_namespace: bool | None = None,
     include_schema_location: bool = True,
+    canonicalize: bool = False,
+    validate: bool = False,
 ) -> str:
     config = SerializerConfig(
-        pretty_print=indent > 0,
+        pretty_print=(indent > 0) and not canonicalize,  # canonicalize does it for us
         pretty_print_indent=" " * indent,
-        ignore_default_attributes=ignore_defaults,
+        xml_declaration=False,
+        ignore_default_attributes=exclude_defaults,
+        ignore_unset_attributes=exclude_unset,
+        attribute_sort_key=operator.attrgetter("name") if canonicalize else None,
     )
     if include_schema_location:
         config.schema_location = f"{OME_2016_06_URI} {OME_2016_06_URI}/ome.xsd"
 
     serializer = XmlSerializer(config=config)
-    xml = serializer.render(ome, ns_map={None: OME_2016_06_URI})
-    # HACK: xsdata is always including <StructuredAnnotations/> because...
-    # 1. we override the default for OME.structured_annotations so that
-    #    it's always a present (if empty) list.  That was the v1 behavior
-    #    and it allows ome.structured_annotations.append(...) to always work.
-    # 2. xsdata thinks it's not nillable, and therefore always includes it
-    # ... we might be able to do it better, but this fixes it for now.
-    return xml.replace("<StructuredAnnotations/>", "")
+    if include_namespace is None:
+        include_namespace = canonicalize
+
+    ns_map = {"ome" if include_namespace else None: OME_2016_06_URI}
+    xml = serializer.render(ome, ns_map=ns_map)
+
+    if canonicalize:
+        xml = _canonicalize(xml, indent=" " * indent)
+    if validate:
+        validate_xml(xml)
+    return xml
+
+
+def _canonicalize(xml: str, indent: str) -> str:
+    from xml.dom import minidom
+
+    xml_out = ET.canonicalize(xml, strip_text=True)
+    return minidom.parseString(xml_out).toprettyxml(indent=indent)  # noqa: S318
 
 
 def from_tiff(
     path: Path | str,
     *,
     validate: bool | None = None,
     parser_kwargs: ParserKwargs | None = None,
@@ -126,14 +186,15 @@
 
 
 def _unpack(fh: io.BufferedReader, strct: Struct) -> int:
     return strct.unpack(fh.read(strct.size))[0]
 
 
 def tiff2xml(path: Path | str) -> bytes:
+    """Extract the OME-XML from a TIFF file."""
     with Path(path).open(mode="rb") as fh:
         head = fh.read(4)
         if head not in TIFF_TYPES:
             raise ValueError(f"{path!r} does not have a recognized TIFF header")
 
         offset_fmt, tagno_fmt, tagsize, codeformat = TIFF_TYPES[head]
         offset_size = offset_fmt.size
```

### Comparing `ome_types-0.4.0a1/src/ome_types/ome-2016-06.xsd` & `ome_types-0.4.0a2/src/ome_types/ome-2016-06.xsd`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/src/ome_types/validation.py` & `ome_types-0.4.0a2/src/ome_types/validation.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/src/ome_types/_mixins/_base_type.py` & `ome_types-0.4.0a2/src/ome_types/_mixins/_base_type.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/src/ome_types/_mixins/_bin_data.py` & `ome_types-0.4.0a2/src/ome_types/_mixins/_bin_data.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/src/ome_types/_mixins/_instrument.py` & `ome_types-0.4.0a2/src/ome_types/_mixins/_instrument.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/src/ome_types/_mixins/_ome.py` & `ome_types-0.4.0a2/src/ome_types/_mixins/_ome.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 
     @classmethod
     def from_tiff(cls, path: Path | str) -> OME:
         from ome_types._conversion import from_tiff
 
         return from_tiff(path)
 
-    def to_xml(self) -> str:
+    def to_xml(self, **kwargs: Any) -> str:
         from ome_types._conversion import to_xml
 
-        return to_xml(cast("OME", self))
+        return to_xml(cast("OME", self), **kwargs)
 
 
 def collect_ids(value: Any) -> dict[str, OMEType]:
     """Return a map of all model objects contained in value, keyed by id.
 
     Recursively walks all dataclass fields and iterates over lists. The base
     case is when value is neither a dataclass nor a list.
```

### Comparing `ome_types-0.4.0a1/src/ome_types/_mixins/_reference.py` & `ome_types-0.4.0a2/src/ome_types/_mixins/_reference.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/src/ome_types/_mixins/_structured_annotations.py` & `ome_types-0.4.0a2/src/ome_types/_mixins/_structured_annotations.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/src/ome_types/model/__init__.py` & `ome_types-0.4.0a2/src/ome_types/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/src/ome_types/model/_color.py` & `ome_types-0.4.0a2/src/ome_types/model/_color.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 RGBA = Tuple[int, int, int, float]
 ColorType = Union[Tuple[int, int, int], RGBA, str, int]
 
 
 class Color(color.Color):
     def __init__(self, val: ColorType = -1) -> None:
-        with suppress(ValueError):
+        with suppress(ValueError, TypeError):
             val = self._int2tuple(int(val))  # type: ignore
         super().__init__(val)  # type: ignore [arg-type]
 
     @classmethod
     def _int2tuple(cls, val: int) -> RGBA:
         return (val >> 24 & 255, val >> 16 & 255, val >> 8 & 255, (val & 255) / 255)
```

### Comparing `ome_types-0.4.0a1/src/ome_types/model/_shape_union.py` & `ome_types-0.4.0a2/src/ome_types/model/_shape_union.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/src/ome_types/model/_user_sequence.py` & `ome_types-0.4.0a2/src/ome_types/model/_user_sequence.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/src/ome_types/model/simple_types.py` & `ome_types-0.4.0a2/src/ome_types/model/simple_types.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/compat.py` & `ome_types-0.4.0a2/src/xsdata_pydantic_basemodel/compat.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/generator.py` & `ome_types-0.4.0a2/src/xsdata_pydantic_basemodel/generator.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/.gitignore` & `ome_types-0.4.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/LICENSE` & `ome_types-0.4.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/README.md` & `ome_types-0.4.0a2/README.md`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a1/pyproject.toml` & `ome_types-0.4.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 docs = [
   "numpydoc",
   "pygments",
   "sphinx==5.3.0",
   "sphinx-rtd-theme==1.1.1",
   "ipython",
 ]
-test = ["pytest", "pytest-cov", "xmlschema", "distributed"]
+test = ["pytest", "pytest-cov", "xmlschema"]
 
 # https://hatch.pypa.io/latest/plugins/build-hook/custom/
 [tool.hatch.build.targets.wheel.hooks.custom]
 # requirements to run the autogen script in hatch_build.py
 require-runtime-dependencies = true
 dependencies = ["black", "ruff", "xsdata[cli]>=23.6"]
```

### Comparing `ome_types-0.4.0a1/PKG-INFO` & `ome_types-0.4.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ome-types
-Version: 0.4.0a1
+Version: 0.4.0a2
 Summary: Python dataclasses for the OME data model
 Project-URL: Source, https://github.com/tlambert03/ome-types
 Project-URL: Tracker, https://github.com/tlambert03/ome-types/issues
 Project-URL: Documentation, https://ome-types.readthedocs.io/en/latest/
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: MIT
 License-File: LICENSE
@@ -34,15 +34,14 @@
 Provides-Extra: docs
 Requires-Dist: ipython; extra == 'docs'
 Requires-Dist: numpydoc; extra == 'docs'
 Requires-Dist: pygments; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme==1.1.1; extra == 'docs'
 Requires-Dist: sphinx==5.3.0; extra == 'docs'
 Provides-Extra: test
-Requires-Dist: distributed; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: xmlschema; extra == 'test'
 Description-Content-Type: text/markdown
 
 # ome-types
```

