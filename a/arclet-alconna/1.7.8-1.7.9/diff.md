# Comparing `tmp/arclet-alconna-1.7.8.tar.gz` & `tmp/arclet_alconna-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-1.7.8.tar", last modified: Fri Jun 30 14:54:00 2023, max compression
+gzip compressed data, was "arclet_alconna-1.7.9.tar", last modified: Mon Jul  3 11:17:47 2023, max compression
```

## Comparing `arclet-alconna-1.7.8.tar` & `arclet_alconna-1.7.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.8/LICENSE
--rw-r--r--   0        0        0     2810 2023-06-08 08:47:20.882466 arclet-alconna-1.7.8/pyproject.toml
--rw-r--r--   0        0        0     6644 2023-06-30 14:51:14.232836 arclet-alconna-1.7.8/README-EN.md
--rw-r--r--   0        0        0     1084 2023-06-30 14:50:29.541004 arclet-alconna-1.7.8/src/arclet/alconna/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 16:37:15.106361 arclet-alconna-1.7.8/src/arclet/alconna/_internal/__init__.py
--rw-r--r--   0        0        0    17705 2023-06-08 08:47:20.884468 arclet-alconna-1.7.8/src/arclet/alconna/_internal/_analyser.py
--rw-r--r--   0        0        0     8476 2023-05-25 16:37:15.107359 arclet-alconna-1.7.8/src/arclet/alconna/_internal/_argv.py
--rw-r--r--   0        0        0    23280 2023-06-08 08:47:20.884468 arclet-alconna-1.7.8/src/arclet/alconna/_internal/_handlers.py
--rw-r--r--   0        0        0    10053 2023-06-08 08:48:46.609460 arclet-alconna-1.7.8/src/arclet/alconna/_internal/_header.py
--rw-r--r--   0        0        0     1333 2023-06-08 08:47:20.886467 arclet-alconna-1.7.8/src/arclet/alconna/_internal/_util.py
--rw-r--r--   0        0        0     1543 2023-05-25 16:37:15.110384 arclet-alconna-1.7.8/src/arclet/alconna/action.py
--rw-r--r--   0        0        0    14606 2023-06-30 14:47:51.057920 arclet-alconna-1.7.8/src/arclet/alconna/args.py
--rw-r--r--   0        0        0     1499 2023-05-25 16:37:15.112359 arclet-alconna-1.7.8/src/arclet/alconna/argv.py
--rw-r--r--   0        0        0    15488 2023-06-08 08:47:20.888469 arclet-alconna-1.7.8/src/arclet/alconna/arparma.py
--rw-r--r--   0        0        0    13248 2023-05-25 16:37:15.114361 arclet-alconna-1.7.8/src/arclet/alconna/base.py
--rw-r--r--   0        0        0     2715 2023-06-08 08:47:20.889467 arclet-alconna-1.7.8/src/arclet/alconna/builtin.py
--rw-r--r--   0        0        0     4867 2023-05-25 16:37:15.116360 arclet-alconna-1.7.8/src/arclet/alconna/completion.py
--rw-r--r--   0        0        0     4465 2023-05-25 16:37:15.117360 arclet-alconna-1.7.8/src/arclet/alconna/config.py
--rw-r--r--   0        0        0    14029 2023-06-25 08:21:06.237281 arclet-alconna-1.7.8/src/arclet/alconna/core.py
--rw-r--r--   0        0        0     2014 2023-06-08 08:47:20.890468 arclet-alconna-1.7.8/src/arclet/alconna/duplication.py
--rw-r--r--   0        0        0     1009 2023-05-25 16:37:15.119359 arclet-alconna-1.7.8/src/arclet/alconna/exceptions.py
--rw-r--r--   0        0        0    11287 2023-05-25 16:37:15.120361 arclet-alconna-1.7.8/src/arclet/alconna/formatter.py
--rw-r--r--   0        0        0       99 2023-05-21 05:43:33.502836 arclet-alconna-1.7.8/src/arclet/alconna/i18n/.config.json
--rw-r--r--   0        0        0     3638 2023-05-21 05:43:33.503837 arclet-alconna-1.7.8/src/arclet/alconna/i18n/en-US.json
--rw-r--r--   0        0        0     3687 2023-05-21 05:43:33.504836 arclet-alconna-1.7.8/src/arclet/alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0    17039 2023-06-08 08:47:20.891468 arclet-alconna-1.7.8/src/arclet/alconna/manager.py
--rw-r--r--   0        0        0     1484 2023-05-25 16:37:15.122358 arclet-alconna-1.7.8/src/arclet/alconna/model.py
--rw-r--r--   0        0        0     1943 2023-05-25 16:37:15.123407 arclet-alconna-1.7.8/src/arclet/alconna/model.pyi
--rw-r--r--   0        0        0     3940 2023-05-25 16:37:15.124599 arclet-alconna-1.7.8/src/arclet/alconna/output.py
--rw-r--r--   0        0        0        0 2023-05-21 05:43:33.513926 arclet-alconna-1.7.8/src/arclet/alconna/py.typed
--rw-r--r--   0        0        0     5815 2023-05-25 16:37:15.125359 arclet-alconna-1.7.8/src/arclet/alconna/stub.py
--rw-r--r--   0        0        0     3586 2023-05-25 16:37:15.125704 arclet-alconna-1.7.8/src/arclet/alconna/typing.py
--rw-r--r--   0        0        0     3246 2023-05-25 16:37:15.127191 arclet-alconna-1.7.8/tests/analyser_test.py
--rw-r--r--   0        0        0     7583 2023-05-25 16:37:15.127710 arclet-alconna-1.7.8/tests/args_test.py
--rw-r--r--   0        0        0     2167 2023-05-25 16:37:15.128711 arclet-alconna-1.7.8/tests/base_test.py
--rw-r--r--   0        0        0     3119 2023-06-08 08:47:20.892467 arclet-alconna-1.7.8/tests/components_test.py
--rw-r--r--   0        0        0     1199 2023-05-25 16:37:15.130711 arclet-alconna-1.7.8/tests/config_test.py
--rw-r--r--   0        0        0    24318 2023-06-12 11:16:57.189124 arclet-alconna-1.7.8/tests/core_test.py
--rw-r--r--   0        0        0      505 2023-05-25 16:37:15.132710 arclet-alconna-1.7.8/tests/util_test.py
--rw-r--r--   0        0        0     7306 1970-01-01 00:00:00.000000 arclet-alconna-1.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet_alconna-1.7.9/LICENSE
+-rw-r--r--   0        0        0     6644 2023-06-30 14:51:14.232836 arclet_alconna-1.7.9/README-EN.md
+-rw-r--r--   0        0        0     2801 2023-07-03 11:17:47.667042 arclet_alconna-1.7.9/pyproject.toml
+-rw-r--r--   0        0        0     1084 2023-07-03 06:12:47.042021 arclet_alconna-1.7.9/src/arclet/alconna/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:37:15.106361 arclet_alconna-1.7.9/src/arclet/alconna/_internal/__init__.py
+-rw-r--r--   0        0        0    17705 2023-06-08 08:47:20.884468 arclet_alconna-1.7.9/src/arclet/alconna/_internal/_analyser.py
+-rw-r--r--   0        0        0     8476 2023-05-25 16:37:15.107359 arclet_alconna-1.7.9/src/arclet/alconna/_internal/_argv.py
+-rw-r--r--   0        0        0    23659 2023-07-03 10:08:02.741883 arclet_alconna-1.7.9/src/arclet/alconna/_internal/_handlers.py
+-rw-r--r--   0        0        0    10053 2023-06-08 08:48:46.609460 arclet_alconna-1.7.9/src/arclet/alconna/_internal/_header.py
+-rw-r--r--   0        0        0     1333 2023-06-08 08:47:20.886467 arclet_alconna-1.7.9/src/arclet/alconna/_internal/_util.py
+-rw-r--r--   0        0        0     1543 2023-05-25 16:37:15.110384 arclet_alconna-1.7.9/src/arclet/alconna/action.py
+-rw-r--r--   0        0        0    14368 2023-07-03 10:09:06.004205 arclet_alconna-1.7.9/src/arclet/alconna/args.py
+-rw-r--r--   0        0        0     1499 2023-05-25 16:37:15.112359 arclet_alconna-1.7.9/src/arclet/alconna/argv.py
+-rw-r--r--   0        0        0    15875 2023-07-03 05:59:27.899461 arclet_alconna-1.7.9/src/arclet/alconna/arparma.py
+-rw-r--r--   0        0        0    13248 2023-05-25 16:37:15.114361 arclet_alconna-1.7.9/src/arclet/alconna/base.py
+-rw-r--r--   0        0        0     2715 2023-06-08 08:47:20.889467 arclet_alconna-1.7.9/src/arclet/alconna/builtin.py
+-rw-r--r--   0        0        0     4867 2023-05-25 16:37:15.116360 arclet_alconna-1.7.9/src/arclet/alconna/completion.py
+-rw-r--r--   0        0        0     4465 2023-05-25 16:37:15.117360 arclet_alconna-1.7.9/src/arclet/alconna/config.py
+-rw-r--r--   0        0        0    14029 2023-06-25 08:21:06.237281 arclet_alconna-1.7.9/src/arclet/alconna/core.py
+-rw-r--r--   0        0        0     2014 2023-06-08 08:47:20.890468 arclet_alconna-1.7.9/src/arclet/alconna/duplication.py
+-rw-r--r--   0        0        0     1009 2023-05-25 16:37:15.119359 arclet_alconna-1.7.9/src/arclet/alconna/exceptions.py
+-rw-r--r--   0        0        0    11287 2023-05-25 16:37:15.120361 arclet_alconna-1.7.9/src/arclet/alconna/formatter.py
+-rw-r--r--   0        0        0       99 2023-05-21 05:43:33.502836 arclet_alconna-1.7.9/src/arclet/alconna/i18n/.config.json
+-rw-r--r--   0        0        0     3638 2023-05-21 05:43:33.503837 arclet_alconna-1.7.9/src/arclet/alconna/i18n/en-US.json
+-rw-r--r--   0        0        0     3687 2023-05-21 05:43:33.504836 arclet_alconna-1.7.9/src/arclet/alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0    17039 2023-06-08 08:47:20.891468 arclet_alconna-1.7.9/src/arclet/alconna/manager.py
+-rw-r--r--   0        0        0     1484 2023-05-25 16:37:15.122358 arclet_alconna-1.7.9/src/arclet/alconna/model.py
+-rw-r--r--   0        0        0     1943 2023-05-25 16:37:15.123407 arclet_alconna-1.7.9/src/arclet/alconna/model.pyi
+-rw-r--r--   0        0        0     3940 2023-05-25 16:37:15.124599 arclet_alconna-1.7.9/src/arclet/alconna/output.py
+-rw-r--r--   0        0        0        0 2023-05-21 05:43:33.513926 arclet_alconna-1.7.9/src/arclet/alconna/py.typed
+-rw-r--r--   0        0        0     5815 2023-05-25 16:37:15.125359 arclet_alconna-1.7.9/src/arclet/alconna/stub.py
+-rw-r--r--   0        0        0     3675 2023-07-03 10:09:05.989754 arclet_alconna-1.7.9/src/arclet/alconna/typing.py
+-rw-r--r--   0        0        0     3246 2023-05-25 16:37:15.127191 arclet_alconna-1.7.9/tests/analyser_test.py
+-rw-r--r--   0        0        0     7926 2023-07-03 10:11:35.779837 arclet_alconna-1.7.9/tests/args_test.py
+-rw-r--r--   0        0        0     2167 2023-05-25 16:37:15.128711 arclet_alconna-1.7.9/tests/base_test.py
+-rw-r--r--   0        0        0     3119 2023-06-08 08:47:20.892467 arclet_alconna-1.7.9/tests/components_test.py
+-rw-r--r--   0        0        0     1199 2023-05-25 16:37:15.130711 arclet_alconna-1.7.9/tests/config_test.py
+-rw-r--r--   0        0        0    24318 2023-07-03 07:08:28.901814 arclet_alconna-1.7.9/tests/core_test.py
+-rw-r--r--   0        0        0      505 2023-05-25 16:37:15.132710 arclet_alconna-1.7.9/tests/util_test.py
+-rw-r--r--   0        0        0     7473 1970-01-01 00:00:00.000000 arclet_alconna-1.7.9/PKG-INFO
```

### Comparing `arclet-alconna-1.7.8/LICENSE` & `arclet_alconna-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/pyproject.toml` & `arclet_alconna-1.7.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
-    "pdm-pep517>=1.0.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [project]
 name = "arclet-alconna"
 description = "A High-performance, Generality, Humane Command Line Arguments Parser Library."
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
@@ -34,15 +34,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
-version = "1.7.8"
+version = "1.7.9"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://arcletproject.github.io/docs/alconna/tutorial"
 repository = "https://github.com/ArcletProject/Alconna"
```

### Comparing `arclet-alconna-1.7.8/README-EN.md` & `arclet_alconna-1.7.9/README-EN.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/__init__.py` & `arclet_alconna-1.7.9/src/arclet/alconna/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 from .builtin import set_default
 from .model import OptionResult, SubcommandResult, HeadResult
 from .output import output_manager
 from .formatter import TextFormatter
 from .duplication import Duplication
 from .stub import ArgsStub, OptionStub, SubcommandStub
 
-__version__ = "1.7.8"
+__version__ = "1.7.9"
 
 # backward compatibility
 Arpamar = Arparma
 DataCollectionContainer = Argv
```

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/_internal/_analyser.py` & `arclet_alconna-1.7.9/src/arclet/alconna/_internal/_analyser.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/_internal/_argv.py` & `arclet_alconna-1.7.9/src/arclet/alconna/_internal/_argv.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/_internal/_handlers.py` & `arclet_alconna-1.7.9/src/arclet/alconna/_internal/_handlers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,233 +1,219 @@
 from __future__ import annotations
 
 import re
 from typing import TYPE_CHECKING, Any, Iterable
 
 from nepattern import AllParam, AnyOne, AnyString, BasePattern
 from nepattern.util import TPattern
-from tarina import Empty, lang
+from tarina import Empty, lang, split_once
 
 from ..action import Action
 from ..args import STRING, Arg, Args
 from ..base import Option, Subcommand
 from ..completion import Prompt, comp_ctx
 from ..config import config
 from ..exceptions import (
     ArgumentMissing, FuzzyMatchSuccess, ParamsUnmatched, PauseTriggered, SpecialOptionTriggered
 )
 from ..model import HeadResult, OptionResult, Sentence
 from ..output import output_manager
-from ..typing import KeyWordVar, MultiVar
+from ..typing import KWBool
 from ._header import Double, Header
 from ._util import levenshtein
 
 if TYPE_CHECKING:
     from ._analyser import Analyser, SubAnalyser
     from ._argv import Argv
 
-
-def _handle_keyword(
-    argv: Argv,
-    value: KeyWordVar,
-    may_arg: Any,
-    seps: tuple[str, ...],
-    result_dict: dict[str, Any],
-    default_val: Any,
-    optional: bool,
-    key: str | None = None,
-    fuzzy: bool = False,
-):
-    """处理关键字参数
-
-    Args:
-        argv (Argv): 命令行参数
-        value (KeyWordVar): 关键字参数
-        may_arg (Any): 可能的参数
-        seps (tuple[str, ...]): 分隔符
-        result_dict (dict[str, Any]): 结果字典
-        default_val (Any): 默认值
-        optional (bool): 是否可选
-        key (str | None, optional): 关键字. Defaults to None.
-        fuzzy (bool, optional): 是否模糊匹配. Defaults to False.
-    """
-    if _kwarg := re.match(fr'^([^{value.sep}]+){value.sep}(.*?)$', may_arg):
-        key = key or _kwarg[1]
-        if (_key := _kwarg[1]) != key:
-            argv.rollback(may_arg)
-            if fuzzy and levenshtein(_key, key) >= config.fuzzy_threshold:
-                raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=_key, target=key))
-            if default_val is None:
-                raise ParamsUnmatched(lang.require("fuzzy", "matched").format(source=_key, target=key))
-            result_dict[_key] = None if default_val is Empty else default_val
-            return
-        if not (_m_arg := _kwarg[2]):
-            _m_arg, _ = argv.next(seps)
-        res = value.base.exec(_m_arg, default_val)
-        if res.flag != 'valid':
+def step_varpos(argv: Argv, args: Args, result: dict[str, Any]):
+    value, arg = args.argument.var_positional
+    argv.context = arg
+    key = arg.name
+    default_val = arg.field.default
+    _result = []
+    kwonly_seps = tuple(arg.value.sep for arg in args.argument.keyword_only.values())  # type: ignore
+    loop = len(argv.release(arg.separators))
+    if value.length > 0:
+        loop = min(loop, value.length)
+    for _ in range(loop):
+        may_arg, _str = argv.next(arg.separators)
+        if _str and may_arg in argv.completion_names:
+            raise SpecialOptionTriggered("completion")
+        if not may_arg or (_str and may_arg in argv.param_ids):
             argv.rollback(may_arg)
-        if res.flag == 'error':
-            if optional:
-                return
-            raise ParamsUnmatched(*res.error.args)
-        result_dict[_kwarg[1]] = res._value  # type: ignore
-        return
-    argv.rollback(may_arg)
-    raise ParamsUnmatched(lang.require("args", "key_missing").format(target=may_arg, key=key))
-
-
-def _loop_kw(argv: Argv, _loop: int, seps: tuple[str, ...], value: MultiVar, default: Any):
-    """循环关键字参数"""
-    result = {}
-    for _ in range(_loop):
-        _m_arg, _m_str = argv.next(seps)
-        if not _m_arg:
-            continue
-        if _m_str and _m_arg in argv.param_ids:
-            argv.rollback(_m_arg)
             break
-        try:
-            _handle_keyword(argv, value.base, _m_arg, seps, result, default, False)  # type: ignore
-        except ParamsUnmatched:
-            break
-    if not result:
-        if value.flag == '+':
-            raise ParamsUnmatched
-        result = [default] if default else []
-    return result
-
-
-def _loop(
-    argv: Argv, _loop: int, seps: tuple[str, ...], value: MultiVar, default: Any, kw: KeyWordVar | None
-):
-    """循环参数"""
-    result = []
-    for _ in range(_loop):
-        _m_arg, _m_str = argv.next(seps)
-        if not _m_arg:
-            continue
-        if _m_str and (
-            _m_arg in argv.param_ids or
-            (kw and re.match(fr'^([^{kw.sep}]+){kw.sep}(.*?)$', _m_arg))
-        ):
-            argv.rollback(_m_arg)
+        if _str and split_once(may_arg.lstrip("-"), kwonly_seps, argv.filter_crlf)[0] in args.argument.keyword_only:
+            argv.rollback(may_arg)
             break
-        if (res := value.base.exec(_m_arg)).flag != 'valid':
-            argv.rollback(_m_arg)
+        if (res := value.base.exec(may_arg)).flag != 'valid':
+            argv.rollback(may_arg)
             break
-        result.append(res._value)  # type: ignore
-    if not result:
-        if value.flag == '+':
-            raise ParamsUnmatched
-        result = [default] if default else []
-    return tuple(result)
-
-
-def multi_arg_handler(argv: Argv, args: Args, arg: Arg, result_dict: dict[str, Any],):
-    """处理可变参数
+        _result.append(res._value)  # type: ignore
+    if not _result:
+        if default_val is not None:
+            _result = default_val if isinstance(default_val, Iterable) else ()
+        elif value.flag == '*':
+            _result = ()
+        else:
+            raise ArgumentMissing(lang.require("args", "missing").format(key=key))
+    result[key] = tuple(_result)
 
-    Args:
-        argv (Argv): 命令行参数
-        args (Args): 参数集合
-        arg (Arg): 参数单元
-        result_dict (dict[str, Any]): 结果字典
-    """
-    seps = arg.separators
-    value: MultiVar = arg.value  # type: ignore
-    key = arg.name
-    default = arg.field.default
-    kw = value.base.__class__ == KeyWordVar
-    _rest = len(args) - len(result_dict)
-    _all_count = len(argv.release(seps))
-    if not kw and not args.var_keyword or kw and not args.var_positional:
-        loop = _all_count - _rest + 1
-    elif not kw:
-        loop = _all_count - (_rest - 2*(args.var_keyword.flag == "*"))
-    else:
-        loop = _all_count - (_rest - 2*(args.var_positional.flag == "*"))
+def step_varkey(argv: Argv, args: Args, result: dict[str, Any]):
+    value, arg = args.argument.var_keyword
+    argv.context = arg
+    name = arg.name
+    default_val = arg.field.default
+    _result = {}
+    loop = len(argv.release(arg.separators))
     if value.length > 0:
         loop = min(loop, value.length)
-    result_dict[key] = (
-        _loop_kw(argv, loop, seps, value, default) if kw
-        else _loop(argv, loop, seps, value, default, value.base if kw else None)
-    )
-    if kw:
-        kwargs = result_dict[key]
-        if not isinstance(kwargs, dict):
-            kwargs = {key: kwargs}
-        result_dict[key] = kwargs
-    else:
-        varargs = result_dict[key]
-        if not isinstance(varargs, Iterable):
-            varargs = (varargs, )
-        elif not isinstance(varargs, tuple):
-            varargs = tuple(varargs)
-        result_dict[key] = varargs
+    for _ in range(loop):
+        may_arg, _str = argv.next(arg.separators)
+        if _str and may_arg in argv.completion_names:
+            raise SpecialOptionTriggered("completion")
+        if not may_arg or (_str and may_arg in argv.param_ids) or not _str:
+            argv.rollback(may_arg)
+            break
+        if value.base.sep in arg.separators:
+            key = may_arg.lstrip("-")
+            _m_arg, _ = argv.next(arg.separators)
+        elif _kwarg := re.match(fr'^(-*[^{value.base.sep}]+){value.base.sep}(.*?)$', may_arg):
+            key = _kwarg[1]
+            if not (_m_arg := _kwarg[2]):
+                _m_arg, _ = argv.next(arg.separators)
+        else:
+            argv.rollback(may_arg)
+            break
+        if (res := value.base.base.exec(_m_arg)).flag != 'valid':
+            argv.rollback(may_arg)
+            break
+        _result[key] = res._value  # type: ignore
+    if not _result:
+        if default_val is not None:
+            _result = default_val if isinstance(default_val, dict) else {}
+        elif value.flag == '*':
+            _result = {}
+        else:
+            raise ArgumentMissing(lang.require("args", "missing").format(key=name))
+    result[name] = _result
 
+def step_keyword(argv: Argv, args: Args, result: dict[str, Any]):
+    kwonly_seps = set()
+    for arg in args.argument.keyword_only.values():
+        kwonly_seps.update(arg.separators)
+    kwonly_seps1 = tuple(arg.value.sep for arg in args.argument.keyword_only.values())  # type: ignore
+    target = len(args.argument.keyword_only)
+    count = 0
+    while count < target:
+        may_arg, _str = argv.next(tuple(kwonly_seps))
+        if _str and may_arg in argv.completion_names:
+            raise SpecialOptionTriggered("completion")
+        if not may_arg or (_str and may_arg in argv.param_ids) or not _str:
+            argv.rollback(may_arg)
+            break
+        key, _m_arg = split_once(may_arg.lstrip("-"), kwonly_seps1, argv.filter_crlf)
+        if key not in args.argument.keyword_only:
+            argv.rollback(may_arg)
+            for arg in args.argument.keyword_only.values():
+                if arg.value.base.exec(key).flag == 'valid':  # type: ignore
+                    raise ParamsUnmatched(lang.require("args", "key_missing").format(target=key, key=arg.name))
+            for name in args.argument.keyword_only:
+                if levenshtein(key, name) >= config.fuzzy_threshold:
+                    raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=name, target=key))
+            raise ParamsUnmatched(lang.require("args", "key_not_found").format(name=key))
+        arg = args.argument.keyword_only[key]
+        value = arg.value.base  # type: ignore
+        default_val = arg.field.default
+        if not _m_arg:
+            if isinstance(value, KWBool):
+                _m_arg = key
+            else:
+                _m_arg, _ = argv.next(args.argument.keyword_only[key].separators)
+        res = (
+            value.invalidate(_m_arg, default_val)
+            if value.anti
+            else value.validate(_m_arg, default_val)
+        )
+        if res.flag != 'valid':
+            argv.rollback(_m_arg)
+        if res.flag == 'error':
+            if arg.optional:
+                count += 1
+                continue
+            raise ParamsUnmatched(*res.error.args)
+        result[key] = res._value  # noqa
+        count += 1
+
+
+    if count < target:
+        for key, arg in args.argument.keyword_only.items():
+            if key in result:
+                continue
+            if arg.field.default is not None:
+                result[key] = None if arg.field.default is Empty else arg.field.default
+            elif not arg.optional:
+                raise ArgumentMissing(lang.require("args", "missing").format(key=key))
 
 def analyse_args(argv: Argv, args: Args) -> dict[str, Any]:
     """
     分析 `Args` 部分
 
     Args:
         argv (Argv): 命令行参数
         args (Args): 目标 `Args`
 
     Returns:
         dict[str, Any]: 解析结果
     """
     result: dict[str, Any] = {}
-    for arg in args.argument:
+    for arg in args.argument.normal:
         argv.context = arg
         key = arg.name
         value = arg.value
         default_val = arg.field.default
         may_arg, _str = argv.next(arg.separators)
         if _str and may_arg in argv.completion_names:
             raise SpecialOptionTriggered("completion")
         if not may_arg or (_str and may_arg in argv.param_ids):
             argv.rollback(may_arg)
             if default_val is not None:
                 result[key] = None if default_val is Empty else default_val
-            elif value.__class__ is MultiVar and value.flag == '*':  # type: ignore
-                result[key] = ()
             elif not arg.optional:
                 raise ArgumentMissing(lang.require("args", "missing").format(key=key))
             continue
-        if value.__class__ is MultiVar:
-            argv.rollback(may_arg)
-            multi_arg_handler(argv, args, arg, result)  # type: ignore
-        elif value.__class__ is KeyWordVar:
-            _handle_keyword(
-                argv, value, may_arg, arg.separators,  # type: ignore
-                result, default_val, arg.optional, key, argv.fuzzy_match  # type: ignore
-            )
-        elif value == AllParam:
+        if value == AllParam:
             argv.rollback(may_arg)
             result[key] = argv.converter(argv.release(arg.separators))
             argv.current_index = argv.ndata
             return result
-        elif value == AnyOne or (value == STRING and _str):
+        if value == AnyOne or (value == STRING and _str):
             result[key] = may_arg
-        elif value == AnyString:
+            continue
+        if value == AnyString:
             result[key] = str(may_arg)
-        else:
-            res = (
-                value.invalidate(may_arg, default_val)
-                if value.anti
-                else value.validate(may_arg, default_val)
-            )
-            if res.flag != 'valid':
-                argv.rollback(may_arg)
-            if res.flag == 'error':
-                if arg.optional:
-                    continue
-                raise ParamsUnmatched(*res.error.args)
-            if not arg.anonymous:
-                result[key] = res._value  # type: ignore
+            continue
+        res = (
+            value.invalidate(may_arg, default_val)
+            if value.anti
+            else value.validate(may_arg, default_val)
+        )
+        if res.flag != 'valid':
+            argv.rollback(may_arg)
+        if res.flag == 'error':
+            if arg.optional:
+                continue
+            raise ParamsUnmatched(*res.error.args)
+        result[key] = res._value  # noqa
+    if args.argument.var_positional:
+        step_varpos(argv, args, result)
+    if args.argument.keyword_only:
+        step_keyword(argv, args, result)
+    if args.argument.var_keyword:
+        step_varkey(argv, args, result)
     argv.context = None
     return result
 
 
 def handle_option(argv: Argv, opt: Option) -> tuple[str, OptionResult]:
     """
     处理 `Option` 部分
```

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/_internal/_header.py` & `arclet_alconna-1.7.9/src/arclet/alconna/_internal/_header.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/_internal/_util.py` & `arclet_alconna-1.7.9/src/arclet/alconna/_internal/_util.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/action.py` & `arclet_alconna-1.7.9/src/arclet/alconna/action.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/args.py` & `arclet_alconna-1.7.9/src/arclet/alconna/args.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from typing import Any, Callable, Generic, Iterable, Sequence, TypeVar, Union
 
 from nepattern import AllParam, AnyOne, BasePattern, RawStr, UnionPattern, all_patterns, type_parser
 from tarina import Empty, get_signature, lang
 from typing_extensions import Self, TypeAlias
 
 from .exceptions import InvalidParam
-from .typing import KeyWordVar, MultiVar
+from .typing import KeyWordVar, MultiVar, KWBool
 
 
 def safe_dcls_kw(**kwargs):
     if sys.version_info < (3, 10):  # pragma: no cover
         kwargs.pop('slots')
     return kwargs
 
@@ -66,15 +66,14 @@
     """参数单元的注释"""
     flag: set[ArgFlag] = dc.field(compare=False, hash=False)
     """参数单元的标识"""
     separators: tuple[str, ...] = dc.field(compare=False, hash=False)
     """参数单元使用的分隔符"""
     optional: bool = dc.field(compare=False, hash=False)
     hidden: bool = dc.field(compare=False, hash=False)
-    anonymous: bool = dc.field(compare=False, hash=False)
 
     def __init__(
         self,
         name: str,
         value: TAValue[_T] | None = None,
         field: Field[_T] | _T | None = None,
         seps: str | Iterable[str] = " ",
@@ -114,15 +113,14 @@
             self.name = res["name"]
         if res := re.match(r"^(?P<name>.+?)(;)?(?P<flag>[?!/]+)", self.name):
             flags.extend(ArgFlag(c) for c in res["flag"])
             self.name = res["name"]
         self.flag = set(flags)
         self.optional = ArgFlag.OPTIONAL in self.flag
         self.hidden = ArgFlag.HIDDEN in self.flag
-        self.anonymous = self.name.startswith("_key_")
         if ArgFlag.ANTI in self.flag and self.value not in (AnyOne, AllParam):
             self.value = deepcopy(self.value).reverse()
 
     def __repr__(self):
         n, v = f"'{self.name}'", str(self.value)
         return (n if n == v else f"{n}: {v}") + (f" = '{self.field.display}'" if self.field.display is not None else "")
 
@@ -150,14 +148,23 @@
             Args: 参数集合
         """
         data: tuple[Arg, ...] | tuple[Any, ...] = item if isinstance(item, tuple) else (item,)
         if isinstance(data[0], Arg):
             return self(*data)
         return self(Arg(key, *data)) if key else self(Arg(*data))  # type: ignore
 
+NULL = {Empty: None, None: Empty}
+
+class _argument(list):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.normal: list[Arg[Any]] = []
+        self.var_positional: tuple[MultiVar, Arg[Any]] | None = None
+        self.var_keyword: tuple[MultiVar, Arg[Any]] | None = None
+        self.keyword_only: dict[str, Arg[Any]] = {}
 
 class Args(metaclass=ArgsMeta):
     """参数集合
 
     用于代表命令节点需求的一系列参数
 
     一般而言, 使用特殊方法 `__getitem__` 来构造参数集合, 例如:
@@ -166,24 +173,15 @@
         Args('name': str, 'age': int)
 
     也可以使用特殊方法 `__getattr__` 来构造参数集合, 例如:
 
         >>> Args.name[str]
         Args('name': str)
     """
-    argument: list[Arg[Any]]
-    """参数单元组"""
-    var_positional: MultiVar | None
-    """可变参数"""
-    var_keyword: MultiVar | None
-    """可变关键字参数"""
-    keyword_only: list[str]
-    """仅关键字参数的名称"""
-    optional_count: int
-    """可选参数的数量"""
+    argument: _argument
 
     @classmethod
     def from_callable(cls, target: Callable) -> tuple[Args, bool]:
         """从可调用函数中构造Args
 
         Args:
             target (Callable): 目标函数
@@ -196,24 +194,21 @@
         for param in get_signature(target):
             name = param.name
             if name in ["self", "cls"]:
                 method = True
                 continue
             anno = param.annotation
             de = param.default
-            NULL = {Empty: None, None: Empty}
             if anno == inspect.Signature.empty:
                 anno = type(de) if de not in NULL else AnyOne
             de = NULL.get(de, de)
             if param.kind == param.KEYWORD_ONLY:
                 if anno == bool:
-                    anno = BasePattern(f"(?:-*no)?-*{name}", 3, bool, lambda _, x: not x.lstrip("-").startswith('no'))
-                    _args.keyword_only.append(name)
-                else:
-                    anno = KeyWordVar(anno, sep=' ')
+                    anno = KWBool(f"(?:-*no)?-*{name}", 3, bool, lambda _, x: not x.lstrip("-").startswith('no'))
+                anno = KeyWordVar(anno)
             if param.kind == param.VAR_POSITIONAL:
                 anno = MultiVar(anno, "*")
             if param.kind == param.VAR_KEYWORD:
                 anno = MultiVar(KeyWordVar(anno), "*")
             _args.add(name, value=anno, default=de)
         return _args, method
 
@@ -223,25 +218,22 @@
 
         Args:
             *args (Arg): 参数单元
             separators (str | Iterable[str] | None, optional): 可选的为所有参数单元指定分隔符
             **kwargs (TAValue): 剩余的参数单元值
         """
         self._visit = set()
-        self.var_positional = None
-        self.var_keyword = None
-        self.keyword_only = []
         self.optional_count = 0
-        self.argument = list(args)
+        self.argument = _argument(args)
         self.argument.extend(Arg(k, type_parser(v), Field()) for k, v in kwargs.items())
         self.__check_vars__()
         if separators is not None:
             self.separate(*((separators,) if isinstance(separators, str) else tuple(separators)))
 
-    __slots__ = "var_positional", "var_keyword", "argument", "optional_count", "keyword_only", "_visit"
+    __slots__ = "argument", "optional_count", "_visit"
 
     def add(self, name: str, *, value: TAValue[Any], default: Any = None, flags: list[ArgFlag] | None = None) -> Self:
         """添加一个参数
 
         Args:
             name (str): 参数名称
             value (TAValue): 参数值
@@ -301,32 +293,33 @@
             _tmp.append(arg)
             _visit.add(arg.name)
             if arg.name in self._visit:
                 continue
             self._visit.add(arg.name)
             if isinstance(arg.value, MultiVar):
                 if isinstance(arg.value.base, KeyWordVar):
-                    if self.var_keyword:
+                    if self.argument.var_keyword:
                         raise InvalidParam(lang.require("args", "duplicate_kwargs"))
-                    self.var_keyword = arg.value
-                elif self.var_positional:
+                    self.argument.var_keyword = (arg.value, arg)
+                elif self.argument.var_positional:
                     raise InvalidParam(lang.require("args", "duplicate_varargs"))
-                else:
-                    self.var_positional = arg.value
-            if isinstance(arg.value, KeyWordVar):
-                if self.var_keyword or self.var_positional:
+                elif self.argument.keyword_only:
                     raise InvalidParam(lang.require("args", "exclude_mutable_args"))
-                self.keyword_only.append(arg.name)
-                if arg.value.sep in arg.separators:
-                    _tmp.insert(-1, Arg(f"_key_{arg.name}", value=f"re:-*{arg.name}"))
-                    _tmp[-1].value = arg.value.base
-            if arg.optional:
-                if self.var_keyword or self.var_positional:
+                else:
+                    self.argument.var_positional = (arg.value, arg)
+            elif isinstance(arg.value, KeyWordVar):
+                if self.argument.var_keyword:
                     raise InvalidParam(lang.require("args", "exclude_mutable_args"))
-                self.optional_count += 1
+                self.argument.keyword_only[arg.name] = arg
+            else:
+                self.argument.normal.append(arg)
+                if arg.optional:
+                    if self.argument.var_keyword or self.argument.var_positional:
+                        raise InvalidParam(lang.require("args", "exclude_mutable_args"))
+                    self.optional_count += 1
         self.argument.clear()
         self.argument.extend(_tmp)
         del _tmp
         del _visit
 
     def __len__(self):
         return len(self.argument)
@@ -358,15 +351,15 @@
 
         Returns:
             Self: 参数集合自身
         """
         if isinstance(other, Args):
             self.argument.extend(other.argument)
             self.__check_vars__()
-            self.keyword_only = list(set(self.keyword_only + other.keyword_only))
+            self.argument.keyword_only.update(other.argument.keyword_only)
             del other
         elif isinstance(other, Arg):
             self.argument.append(other)
             self.__check_vars__()
         elif isinstance(other, Sequence):
             self.__getitem__(tuple(other))
         return self
@@ -381,15 +374,15 @@
         return self
 
     def __eq__(self, other):
         return self.argument == other.argument
 
     def __repr__(self):
         return (
-            f"Args({', '.join([f'{arg}' for arg in self.argument if not arg.anonymous])})"
+            f"Args({', '.join([f'{arg}' for arg in self.argument])})"
             if self.argument else "Empty"
         )
 
     @property
     def empty(self) -> bool:
         """判断当前参数集合是否为空"""
         return not self.argument
```

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/argv.py` & `arclet_alconna-1.7.9/src/arclet/alconna/argv.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/arparma.py` & `arclet_alconna-1.7.9/src/arclet/alconna/arparma.py`

 * *Files 6% similar despite different names*

```diff
@@ -203,18 +203,29 @@
             target (Callable[..., T]): 要调用的函数
             **additional (Any): 附加参数
         Returns:
             T: 函数返回值
         Raises:
             RuntimeError: 如果 Arparma 未匹配, 则抛出 RuntimeError
         """
-        if self.matched:
-            names = {p.name for p in get_signature(target)}
-            return target(**{k: v for k, v in {**self.all_matched_args, **additional}.items() if k in names})
-        raise RuntimeError
+        if not self.matched:
+            raise RuntimeError("No matched")
+        pos_args = []
+        kw_args = {}
+        data = {**self.all_matched_args, **additional}
+        for p in get_signature(target):
+            if p.kind == p.POSITIONAL_ONLY:
+                pos_args.append(data[p.name])
+            elif p.kind == p.VAR_POSITIONAL:
+                pos_args.extend(data[p.name])
+            elif p.kind == p.VAR_KEYWORD:
+                kw_args = {**kw_args, **data[p.name]}
+            else:
+                kw_args[p.name] = data[p.name]
+        return target(*pos_args, **kw_args)
 
     def fail(self, exc: type[BaseException] | BaseException | str):
         """生成一个失败的 `Arparma`"""
         return Arparma(self._source, self.origin, False, self.header_match, error_info=exc)
 
     def __require__(self, parts: list[str]) -> tuple[dict[str, Any] | OptionResult | SubcommandResult | None, str]:
         """如果能够返回, 除开基本信息, 一定返回该path所在的dict"""
```

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/base.py` & `arclet_alconna-1.7.9/src/arclet/alconna/base.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/builtin.py` & `arclet_alconna-1.7.9/src/arclet/alconna/builtin.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/completion.py` & `arclet_alconna-1.7.9/src/arclet/alconna/completion.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/config.py` & `arclet_alconna-1.7.9/src/arclet/alconna/config.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/core.py` & `arclet_alconna-1.7.9/src/arclet/alconna/core.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/duplication.py` & `arclet_alconna-1.7.9/src/arclet/alconna/duplication.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/exceptions.py` & `arclet_alconna-1.7.9/src/arclet/alconna/exceptions.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/formatter.py` & `arclet_alconna-1.7.9/src/arclet/alconna/formatter.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/i18n/en-US.json` & `arclet_alconna-1.7.9/src/arclet/alconna/i18n/en-US.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/i18n/zh-CN.json` & `arclet_alconna-1.7.9/src/arclet/alconna/i18n/zh-CN.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/manager.py` & `arclet_alconna-1.7.9/src/arclet/alconna/manager.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/model.py` & `arclet_alconna-1.7.9/src/arclet/alconna/model.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/model.pyi` & `arclet_alconna-1.7.9/src/arclet/alconna/model.pyi`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/output.py` & `arclet_alconna-1.7.9/src/arclet/alconna/output.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/stub.py` & `arclet_alconna-1.7.9/src/arclet/alconna/stub.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/src/arclet/alconna/typing.py` & `arclet_alconna-1.7.9/src/arclet/alconna/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,8 +105,14 @@
     def __repr__(self):
         return self.alias
 
 
 Nargs = MultiVar
 Kw = _Kw()
 
-__all__ = ["DataCollection", "TDC", "MultiVar", "Nargs", "Kw", "KeyWordVar", "TPrefixes", "CommandMeta"]
+
+class KWBool(BasePattern):
+    """对布尔参数的包装"""
+    ...
+
+
+__all__ = ["DataCollection", "TDC", "MultiVar", "Nargs", "Kw", "KeyWordVar", "TPrefixes", "CommandMeta", "KWBool"]
```

### Comparing `arclet-alconna-1.7.8/tests/analyser_test.py` & `arclet_alconna-1.7.9/tests/analyser_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/tests/args_test.py` & `arclet_alconna-1.7.9/tests/args_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,25 +138,34 @@
         "foo": "abc",
         "bar": 123,
     }
     assert analyse_args(arg14, ["abc 123"], raise_exception=False) != {
         "foo": "abc",
         "bar": 123,
     }
-    arg14_1 = Args["--width;?", Kw[int], 1280]["--height?", Kw[int], 960]
+    arg14_1 = Args["width;?", Kw[int], 1280]["height?", Kw[int], 960]
     assert analyse_args(arg14_1, ["--width=960 --height=960"]) == {
-        "--width": 960,
-        "--height": 960,
+        "width": 960,
+        "height": 960,
+    }
+    assert analyse_args(arg14_1, ["--height=480 --width=960"]) == {
+        "width": 960,
+        "height": 480,
     }
     arg14_2 = Args.foo[str]["bar", KeyWordVar(int, " ")]["baz", KeyWordVar(bool, ":")]
     assert analyse_args(arg14_2, ["abc -bar 123 baz:false"]) == {
         "bar": 123,
         "baz": False,
         "foo": "abc",
     }
+    assert analyse_args(arg14_2, ["abc baz:false -bar 456"]) == {
+        "bar": 456,
+        "baz": False,
+        "foo": "abc",
+    }
 
 
 def test_pattern():
     test_type = BasePattern(
         "(.+?).py", MatchMode.REGEX_CONVERT, list, lambda _, x: x.split("/"), "test"
     )
     arg15 = Args().add("bar", value=test_type)
@@ -164,23 +173,25 @@
     assert analyse_args(arg15, ["abc/def.py"]) == {"bar": ["abc", "def"]}
     assert analyse_args(arg15, ["abc/def.mp3"], raise_exception=False) != {
         "bar": ["abc", "def"]
     }
 
 
 def test_callable():
-    def test(foo: str, bar: int, baz: bool = False):
+    def test(foo: str, bar: int, baz: bool = False, *, qux: bool, quux: str = ""):
         ...
 
     arg16, _ = Args.from_callable(test)
-    assert len(arg16.argument) == 3
-    assert analyse_args(arg16, ["abc 123 True"]) == {
+    assert len(arg16.argument) == 5
+    assert analyse_args(arg16, ["abc 123 True --qux quux=1"]) == {
         "foo": "abc",
         "bar": 123,
         "baz": True,
+        "qux": True,
+        "quux": "1",
     }
 
 
 def test_func_anno():
     from datetime import datetime
 
     def test(time: Union[int, str]) -> datetime:
```

### Comparing `arclet-alconna-1.7.8/tests/base_test.py` & `arclet_alconna-1.7.9/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/tests/components_test.py` & `arclet_alconna-1.7.9/tests/components_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/tests/config_test.py` & `arclet_alconna-1.7.9/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/tests/core_test.py` & `arclet_alconna-1.7.9/tests/core_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.8/PKG-INFO` & `arclet_alconna-1.7.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: arclet-alconna
-Version: 1.7.8
+Version: 1.7.9
 Summary: A High-performance, Generality, Humane Command Line Arguments Parser Library.
+Keywords: command argparse fast alconna cli command-line parsing optparse
+Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
-Keywords: command,argparse,fast,alconna,cli,command-line,parsing,optparse
-Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
-Requires-Python: >=3.8
+Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Typing :: Typed
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Project-URL: Documentation, https://arcletproject.github.io/docs/alconna/tutorial
+Project-URL: Repository, https://github.com/ArcletProject/Alconna
+Requires-Python: >=3.8
+Requires-Dist: typing-extensions>=4.5.0
+Requires-Dist: nepattern<0.6.0,>=0.5.8
+Requires-Dist: tarina>=0.3.3
+Requires-Dist: arclet-alconna-tools>=0.2.0; extra == "full"
 Provides-Extra: full
-Project-URL: documentation, https://arcletproject.github.io/docs/alconna/tutorial
-Project-URL: repository, https://github.com/ArcletProject/Alconna
 Description-Content-Type: text/markdown
 
 ![](https://socialify.git.ci/ArcletProject/Alconna/image?description=1&descriptionEditable=A%20High-performance%2C%20Generality%2C%20Humane%20Command%20Line%20Arguments%20Parser%20Library.&font=Inter&forks=1&issues=1&language=1&logo=https%3A%2F%2Farclet.top%2Fimg%2Farclet.png&name=1&owner=1&pattern=Brick%20Wall&stargazers=1&theme=Auto)
 <div align="center"> 
 
 # Alconna
 
@@ -252,8 +256,8 @@
 Alconna is licensed under the [MIT License](LICENSE).
 
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FArcletProject%2FAlconna.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FArcletProject%2FAlconna?ref=badge_large)
 
 ## Acknowledgement
 
 [JetBrains](https://www.jetbrains.com/): Support Authorize for [PyCharm](https://www.jetbrains.com/pycharm/)<br>
-[<img src="https://cdn.jsdelivr.net/gh/Kyomotoi/CDN@master/noting/jetbrains-variant-3.png" width="200"/>](https://www.jetbrains.com/)
+[<img src="https://cdn.jsdelivr.net/gh/Kyomotoi/CDN@master/noting/jetbrains-variant-3.png" width="200"/>](https://www.jetbrains.com/)
```

