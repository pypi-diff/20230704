# Comparing `tmp/fancyflags-1.1.tar.gz` & `tmp/fancyflags-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fancyflags-1.1.tar", last modified: Sat Nov 27 16:32:54 2021, max compression
+gzip compressed data, was "fancyflags-1.2.tar", last modified: Tue Jul  4 13:07:15 2023, max compression
```

## Comparing `fancyflags-1.1.tar` & `fancyflags-1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 alimuldal (390555) primarygroup (89939)        0 2021-11-27 16:32:54.000000 fancyflags-1.1/
--rw-r-----   0 alimuldal (390555) primarygroup (89939)    11358 2021-09-16 16:36:42.000000 fancyflags-1.1/LICENSE
--rw-r--r--   0 alimuldal (390555) primarygroup (89939)      758 2021-11-27 16:32:54.000000 fancyflags-1.1/PKG-INFO
--rw-r--r--   0 alimuldal (390555) primarygroup (89939)    10531 2021-10-12 22:20:15.000000 fancyflags-1.1/README.md
-drwxr-xr-x   0 alimuldal (390555) primarygroup (89939)        0 2021-11-27 16:32:54.000000 fancyflags-1.1/fancyflags/
--rw-r--r--   0 alimuldal (390555) primarygroup (89939)     1943 2021-10-12 22:05:04.000000 fancyflags-1.1/fancyflags/__init__.py
--rw-r-----   0 alimuldal (390555) primarygroup (89939)     4579 2021-09-16 16:36:42.000000 fancyflags-1.1/fancyflags/_argument_parsers.py
--rw-r-----   0 alimuldal (390555) primarygroup (89939)     4579 2021-09-16 16:36:42.000000 fancyflags-1.1/fancyflags/_argument_parsers_test.py
--rw-r--r--   0 alimuldal (390555) primarygroup (89939)     6424 2021-11-26 18:03:52.000000 fancyflags-1.1/fancyflags/_auto.py
--rw-r--r--   0 alimuldal (390555) primarygroup (89939)     6780 2021-11-26 18:03:52.000000 fancyflags-1.1/fancyflags/_auto_test.py
--rw-r-----   0 alimuldal (390555) primarygroup (89939)     2985 2021-09-16 16:36:42.000000 fancyflags-1.1/fancyflags/_define_auto.py
--rw-r--r--   0 alimuldal (390555) primarygroup (89939)     5082 2021-11-27 15:34:04.000000 fancyflags-1.1/fancyflags/_define_auto_test.py
--rw-r-----   0 alimuldal (390555) primarygroup (89939)    16577 2021-09-16 16:36:42.000000 fancyflags-1.1/fancyflags/_definitions.py
--rw-r-----   0 alimuldal (390555) primarygroup (89939)    14107 2021-09-16 16:36:42.000000 fancyflags-1.1/fancyflags/_definitions_test.py
--rw-r--r--   0 alimuldal (390555) primarygroup (89939)     7078 2021-11-26 18:03:52.000000 fancyflags-1.1/fancyflags/_flags.py
--rw-r-----   0 alimuldal (390555) primarygroup (89939)     2620 2021-09-16 16:36:42.000000 fancyflags-1.1/fancyflags/_flags_test.py
--rw-r-----   0 alimuldal (390555) primarygroup (89939)     4218 2021-09-16 16:36:42.000000 fancyflags-1.1/fancyflags/_flagsaver_test.py
--rw-r--r--   0 alimuldal (390555) primarygroup (89939)      914 2021-11-27 16:27:48.000000 fancyflags-1.1/fancyflags/_metadata.py
-drwxr-xr-x   0 alimuldal (390555) primarygroup (89939)        0 2021-11-27 16:32:54.000000 fancyflags-1.1/fancyflags.egg-info/
--rw-r--r--   0 alimuldal (390555) primarygroup (89939)      758 2021-11-27 16:32:54.000000 fancyflags-1.1/fancyflags.egg-info/PKG-INFO
--rw-r--r--   0 alimuldal (390555) primarygroup (89939)      551 2021-11-27 16:32:54.000000 fancyflags-1.1/fancyflags.egg-info/SOURCES.txt
--rw-r--r--   0 alimuldal (390555) primarygroup (89939)        1 2021-11-27 16:32:54.000000 fancyflags-1.1/fancyflags.egg-info/dependency_links.txt
--rw-r--r--   0 alimuldal (390555) primarygroup (89939)        8 2021-11-27 16:32:54.000000 fancyflags-1.1/fancyflags.egg-info/requires.txt
--rw-r--r--   0 alimuldal (390555) primarygroup (89939)       11 2021-11-27 16:32:54.000000 fancyflags-1.1/fancyflags.egg-info/top_level.txt
--rw-r--r--   0 alimuldal (390555) primarygroup (89939)       38 2021-11-27 16:32:54.000000 fancyflags-1.1/setup.cfg
--rw-r--r--   0 alimuldal (390555) primarygroup (89939)     1670 2021-11-27 15:34:04.000000 fancyflags-1.1/setup.py
+drwxr-sr-x   0 root         (0)     1002        0 2023-07-04 13:07:15.831546 fancyflags-1.2/
+-rw-rw-r--   0 root         (0)     1002    11358 2023-07-04 13:02:51.000000 fancyflags-1.2/LICENSE
+-rw-r--r--   0 root         (0)     1002      712 2023-07-04 13:07:15.831546 fancyflags-1.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1002    11045 2023-07-04 13:02:51.000000 fancyflags-1.2/README.md
+drwxr-sr-x   0 root         (0)     1002        0 2023-07-04 13:07:15.827546 fancyflags-1.2/fancyflags/
+-rw-rw-r--   0 root         (0)     1002     2010 2023-07-04 13:02:51.000000 fancyflags-1.2/fancyflags/__init__.py
+-rw-rw-r--   0 root         (0)     1002     5836 2023-07-04 13:02:51.000000 fancyflags-1.2/fancyflags/_argument_parsers.py
+-rw-rw-r--   0 root         (0)     1002     6704 2023-07-04 13:02:51.000000 fancyflags-1.2/fancyflags/_argument_parsers_test.py
+-rw-rw-r--   0 root         (0)     1002     8162 2023-07-04 13:02:51.000000 fancyflags-1.2/fancyflags/_auto.py
+-rw-rw-r--   0 root         (0)     1002     9895 2023-07-04 13:02:51.000000 fancyflags-1.2/fancyflags/_auto_test.py
+-rw-rw-r--   0 root         (0)     1002     3216 2023-07-04 13:02:51.000000 fancyflags-1.2/fancyflags/_define_auto.py
+-rw-rw-r--   0 root         (0)     1002     7177 2023-07-04 13:02:51.000000 fancyflags-1.2/fancyflags/_define_auto_test.py
+-rw-rw-r--   0 root         (0)     1002    17875 2023-07-04 13:02:51.000000 fancyflags-1.2/fancyflags/_definitions.py
+-rw-rw-r--   0 root         (0)     1002    21803 2023-07-04 13:02:51.000000 fancyflags-1.2/fancyflags/_definitions_test.py
+-rw-rw-r--   0 root         (0)     1002     6622 2023-07-04 13:02:51.000000 fancyflags-1.2/fancyflags/_flags.py
+-rw-rw-r--   0 root         (0)     1002     2653 2023-07-04 13:02:51.000000 fancyflags-1.2/fancyflags/_flags_test.py
+-rw-rw-r--   0 root         (0)     1002     4326 2023-07-04 13:02:51.000000 fancyflags-1.2/fancyflags/_flagsaver_test.py
+-rw-rw-r--   0 root         (0)     1002      914 2023-07-04 13:02:51.000000 fancyflags-1.2/fancyflags/_metadata.py
+drwxr-sr-x   0 root         (0)     1002        0 2023-07-04 13:07:15.831546 fancyflags-1.2/fancyflags.egg-info/
+-rw-r--r--   0 root         (0)     1002      712 2023-07-04 13:07:15.000000 fancyflags-1.2/fancyflags.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1002      551 2023-07-04 13:07:15.000000 fancyflags-1.2/fancyflags.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1002        1 2023-07-04 13:07:15.000000 fancyflags-1.2/fancyflags.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1002        8 2023-07-04 13:07:15.000000 fancyflags-1.2/fancyflags.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1002       11 2023-07-04 13:07:15.000000 fancyflags-1.2/fancyflags.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1002       38 2023-07-04 13:07:15.831546 fancyflags-1.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1002     1801 2023-07-04 13:02:51.000000 fancyflags-1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fancyflags-1.1/LICENSE` & `fancyflags-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fancyflags-1.1/PKG-INFO` & `fancyflags-1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Metadata-Version: 2.1
 Name: fancyflags
-Version: 1.1
+Version: 1.2
 Summary: A Python library for defining dictionary-valued flags.
-Home-page: UNKNOWN
 Author: DeepMind
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `fancyflags-1.1/README.md` & `fancyflags-1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 # fancyflags
 
-<!--* freshness: { owner: 'ydoron' reviewed: '2021-10-12' } *-->
+<!--* freshness: { owner: 'ydoron' reviewed: '2022-07-18' } *-->
 
 ![PyPI Python version](https://img.shields.io/pypi/pyversions/fancyflags)
 ![PyPI version](https://badge.fury.io/py/fancyflags.svg)
 
-TIP: Already a fancyflags user? Check out our [usage tips](#tips)!
+## Introduction
 
-The main feature of `fancyflags` is a nested dict flag, with familiar "dot"
-overrides for fields. These dict flags:
+`fancyflags` is a Python library that extends
+[`absl.flags`](https://github.com/abseil/abseil-py) with additional structured
+flag types.
 
-*   Can be overridden with “dot” notation, similar to
-    [`config_flags`](https://github.com/google/ml_collections#usage).
-*   Are typed and validated like standard flags, catching errors before they
-    propagate into your program.
-*   Are easy to mix and match with standard flags, without adding extra files to
-    your codebase.
-*   Can be unpacked into constructor/function calls, e.g.
-    `replay(**FLAGS.replay)`.
+`fancyflags` provides flags corresponding to structures such as
+[dicts](#dict-flags), [dataclasses, and (somewhat) arbitrary callables](#auto).
+
+These flags are typed and validated like regular `absl` flags, catching errors
+before they propagate into your program. To override values, users can access
+familiar "dotted" flag names.
+
+TIP: Already a `fancyflags` user? Check out our [usage tips](#tips)!
+
+## A short note on design philosophy:
+
+`fancyflags` promotes mixing with regular `absl` flags. In many cases a few
+regular `absl` flags are all you need!
+
+`fancyflags` does not require you to modify library code: it should only be used
+in your "main" file
+
+`fancyflags` is not a dependency injection framework, and avoids
+programming-language-like power features. We prefer that users write regular
+Python for wiring up their code, because it's explicit, simple to understand,
+and allows static analysis tools to identify problems.
 
 ## Installation
 
 `fancyflags` can be installed from PyPI using `pip`:
 
 ```shell
 pip install fancyflags
@@ -35,15 +49,15 @@
 
 or alternatively by checking out a local copy of our repository and running:
 
 ```shell
 pip install /path/to/local/fancyflags/
 ```
 
-## Quickstart
+## Dict flags
 
 If we have a class `Replay`, with arguments `capacity`, `priority_exponent` and
 others, we can define a corresponding dict flag in our main script
 
 ```python
 import fancyflags as ff
 
@@ -55,15 +69,15 @@
     removal_strategy=ff.Enum("fifo", ["rand", "fifo", "max_value"])
 )
 ```
 
 and `**unpack` the values directly into the `Replay` constructor
 
 ```python
-replay_lib.Replay(**REPLAY_FLAG.value)
+replay_lib.Replay(**_REPLAY_FLAG.value)
 ```
 
 `ff.DEFINE_dict` creates a flag named `replay`, with a default value of
 
 ```python
 {
     "capacity": 1000000,
@@ -151,19 +165,19 @@
     exponents=dict(
         priority=ff.Float(0.6),  # Help string: "replay.exponents.priority"
         importance_sampling=ff.Float(0.4, "Importance sampling coefficient."),
     )
 )
 ```
 
-## "Auto" flags for functions and other structures.
+## "Auto" flags for functions and other structures {#auto}
 
-`fancyflags` also provides `ff.DEFINE_auto` which automatically generates a dict
-flag declaration corresponding to the signature of a given callable. The return
-value will also carry the correct type information.
+`fancyflags` also provides `ff.DEFINE_auto` which automatically generates a flag
+declaration corresponding to the signature of a given callable. The return value
+will also carry the correct type information.
 
 For example the callable could be a constructor
 
 ```python
 _REPLAY = ff.DEFINE_auto('replay', replay_lib.Replay)
 ```
 
@@ -219,15 +233,15 @@
 
 ## Notes on using `flagsaver`
 
 abseil-py's [flagsaver](https://github.com/abseil/abseil-py/blob/master/absl/testing/flagsaver.py)
 module is useful for safely overriding flag values in test code. Here's how to
 make it work well with fancyflags.
 
-### Making dotted names work with `flagsaver` keyword arguments.
+### Making dotted names work with `flagsaver` keyword arguments
 
 Since `flagsaver` relies on keyword arguments, overriding a flag with a dot in
 its name will result in a `SyntaxError`:
 
 ```python
 # Invalid Python syntax.
 flagsaver.flagsaver(replay.capacity=100, replay.priority_exponent=0.5)
@@ -286,28 +300,29 @@
 `ff.Float`          | `flags.DEFINE_float`
 `ff.Sequence`       | `ff.DEFINE_sequence`
 `ff.String`         | `flags.DEFINE_string`
 `ff.StringList`     | `flags.DEFINE_list`
 `ff.MultiEnum`      | `ff.DEFINE_multi_enum`
 `ff.MultiEnumClass` | `flags.DEFINE_multi_enum_class`
 `ff.MultiString`    | `flags.DEFINE_multi_string`
+`ff.DateTime`       | -
 
 ### Defining a new `ff.Item`
 
 Given a `flags.ArgumentParser`, we can define an `ff.Item` in a few lines of
 code.
 
 For example, if we wanted to define an `ff.Item` that corresponded to
 `flags.DEFINE_spaceseplist`, we would look for the parser that this definition
 uses, and write:
 
 ```python
 class SpaceSepList(ff.Item):
 
-  def __init__(self, help_string)
+  def __init__(self, default, help_string)
     parser = flags.WhitespaceSeparatedListParser()
     super(SpaceSepList, self).__init__(default, help_string, parser)
 
 ```
 
 Note that custom `ff.Item` definitions do not _need_ to be added to the
 fancyflags library to work.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fancyflags-1.1/fancyflags/__init__.py` & `fancyflags-1.2/fancyflags/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,29 +14,31 @@
 # ============================================================================
 """An extended flags library. The main component is a nested dict flag."""
 
 # pylint: disable=g-bad-import-order,g-import-not-at-top
 
 # Add current module to disclaimed module ids.
 from absl import flags
+
 flags.disclaim_key_flags()
 
 from fancyflags._metadata import __version__
 
 # Define flags based on a dictionary or sequence.
 from fancyflags._definitions import DEFINE_dict
 from fancyflags._definitions import DEFINE_sequence
 from fancyflags._definitions import define_flags
 
 # Automatically build fancyflags defs from a callable signature.
 from fancyflags._auto import auto
 from fancyflags._define_auto import DEFINE_auto
 
-# Currently supported types inside the dict.
+# `Item` definitions for supported types.
 from fancyflags._definitions import Boolean
+from fancyflags._definitions import DateTime
 from fancyflags._definitions import Enum
 from fancyflags._definitions import EnumClass
 from fancyflags._definitions import Float
 from fancyflags._definitions import Integer
 from fancyflags._definitions import MultiEnum
 from fancyflags._definitions import MultiEnumClass
 from fancyflags._definitions import MultiString
@@ -44,7 +46,9 @@
 from fancyflags._definitions import String
 from fancyflags._definitions import StringList
 
 # Class for adding new flag types.
 from fancyflags._definitions import Item
 
 # usage_logging: import
+
+# experimental: import
```

### Comparing `fancyflags-1.1/fancyflags/_argument_parsers.py` & `fancyflags-1.2/fancyflags/_argument_parsers.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,28 +11,31 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or  implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """Argument parsers."""
 
 import ast
+import datetime
 import enum
 
 from absl import flags
 
 BASIC_SEQUENCE_TYPES = (list, tuple)
 
 # We assume a sequence contains only these types. Python has no primitive types.
 SIMPLE_TYPES = (bool, float, int, str)
 
 NOT_A_SIMPLE_TYPE_MESSAGE = """
 Input list contains unsupported type {{}}, however each element in a sequence
 must be a {} or {}.
-""".format(", ".join(type_.__name__ for type_ in SIMPLE_TYPES[:-1]),
-           SIMPLE_TYPES[-1].__name__)
+""".format(
+    ", ".join(type_.__name__ for type_ in SIMPLE_TYPES[:-1]),
+    SIMPLE_TYPES[-1].__name__,
+)
 
 _EMPTY_STRING_ERROR_MESSAGE = """
 Empty sequences should be given explicitly as [] or () and not as an empty
 string"""
 
 
 class SequenceParser(flags.ArgumentParser):
@@ -58,19 +61,26 @@
     if argument is None:
       return []
     elif isinstance(argument, BASIC_SEQUENCE_TYPES):
       result = argument[:]
     elif isinstance(argument, str):
       if not argument:
         raise ValueError(_EMPTY_STRING_ERROR_MESSAGE)
-      result = ast.literal_eval(argument)
+      try:
+        result = ast.literal_eval(argument)
+      except (ValueError, SyntaxError) as e:
+        raise ValueError(
+            f'Failed to parse "{argument}" as a python literal.'
+        ) from e
+
       if not isinstance(result, BASIC_SEQUENCE_TYPES):
         raise TypeError(
             "Input string should represent a list or tuple, however it "
-            "evaluated as a {}.".format(type(result).__name__))
+            "evaluated as a {}.".format(type(result).__name__)
+        )
     else:
       raise TypeError("Unsupported type {}.".format(type(argument).__name__))
 
     # Make sure the result is a flat sequence of simple types.
     for value in result:
       if not isinstance(value, SIMPLE_TYPES):
         raise TypeError(NOT_A_SIMPLE_TYPE_MESSAGE.format(type(value).__name__))
@@ -100,15 +110,14 @@
 
   def parse(self, arguments):
     """Determines validity of arguments.
 
     Args:
       arguments: list, tuple, or enum of flag values. Each value may be any type
 
-
     Returns:
       The input list, tuple or enum if valid.
 
     Raises:
       TypeError: If the input type is not supported.
       ValueError: Raised if an argument element didn't match anything in enum.
     """
@@ -120,19 +129,50 @@
       result = arguments
     elif isinstance(arguments, str):
       result = ast.literal_eval(arguments)
 
       if not isinstance(result, BASIC_SEQUENCE_TYPES):
         raise TypeError(
             "Input string should represent a list or tuple, however it "
-            "evaluated as a {}.".format(type(result).__name__))
+            "evaluated as a {}.".format(type(result).__name__)
+        )
     else:
       raise TypeError("Unsupported type {}.".format(type(arguments).__name__))
 
     if not all(arg in self.enum_values for arg in result):
-      raise ValueError("Argument values should be one of <{}>".format(
-          "|".join(str(value) for value in self.enum_values)))
+      raise ValueError(
+          "Argument values should be one of <{}>".format(
+              "|".join(str(value) for value in self.enum_values)
+          )
+      )
     else:
       return result
 
   def flag_type(self):
     return "multi enum"
+
+
+class PossiblyNaiveDatetimeParser(flags.ArgumentParser):
+  """Parses an ISO format datetime string into a datetime.datetime."""
+
+  def parse(self, value) -> datetime.datetime:
+    if isinstance(value, datetime.datetime):
+      return value
+
+    # Handle ambiguous cases such as 2000-01-01+01:00, where the part after the
+    # '+' sign looks like timezone info but is actually just the time.
+    if value[10:11] in ("+", "-"):
+      # plus/minus as separator between date and time (can be any character)
+      raise ValueError(
+          f"datetime value {value!r} uses {value[10]!r} as separator "
+          "between date and time (excluded to avoid confusion between "
+          "time and offset). Use any other character instead, e.g. "
+          f"{value[:10] + 'T' + value[11:]!r}"
+      )
+
+    try:
+      return datetime.datetime.fromisoformat(value)
+    except ValueError as e:
+      raise ValueError(f"invalid datetime value {value!r}: {e}") from None
+
+  def flag_type(self) -> str:
+    return "datetime.datetime"
```

### Comparing `fancyflags-1.1/fancyflags/_auto_test.py` & `fancyflags-1.2/fancyflags/_define_auto_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,207 +8,205 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or  implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
-"""Tests for fancyflags.auto."""
+"""Tests for fancyflags._define_auto."""
 
-# Test that `auto` can still correctly infer parameter types when postponed
-# evaluation of type annotations (PEP 563) is enabled.
-from __future__ import annotations
-
-import abc
-import enum
-from typing import List, Optional, Sequence, Tuple
+import copy
+import dataclasses
+from typing import Sequence
 
 from absl import flags
 from absl.testing import absltest
-import fancyflags as ff
-from fancyflags import _auto
+from fancyflags import _define_auto
+from fancyflags import _flags
 
-FLAGS = flags.FLAGS
 
-
-class MyEnum(enum.Enum):
-  ZERO = 0
-  ONE = 1
-
-
-class AutoTest(absltest.TestCase):
-
-  def test_works_fn(self):
-
-    # pylint: disable=unused-argument
-    def my_function(
-        str_: str = 'foo',
-        int_: int = 10,
-        float_: float = 1.0,
-        bool_: bool = False,
-        list_int: List[int] = [1, 2, 3],
-        tuple_str: Tuple[str] = ('foo',),
-        sequence_bool: Sequence[bool] = [True, False],
-        optional_int: Optional[int] = None,
-        optional_float: Optional[float] = None,
-        optional_list_int: Optional[List[int]] = None,
-    ):  # pylint: disable=dangerous-default-value
-      pass
-    # pylint: enable=unused-argument
-    expected_settings = {
-        'str_': 'foo',
-        'int_': 10,
-        'float_': 1.0,
-        'bool_': False,
-        'list_int': [1, 2, 3],
-        'tuple_str': ('foo',),
-        'sequence_bool': [True, False],
-        'optional_int': None,
-        'optional_float': None,
-        'optional_list_int': None,
-    }
-    ff_dict = ff.auto(my_function)
-    self.assertCountEqual(expected_settings, ff_dict)
-    ff.DEFINE_dict('my_function_settings', **ff_dict)
-    self.assertEqual(FLAGS.my_function_settings, expected_settings)
-
-  def test_works_enum_fn(self):
-
-    # pylint: disable=unused-argument
-    def my_function(
-        str_: str = 'foo',
-        int_: int = 10,
-        enum_: MyEnum = MyEnum.ZERO
+@dataclasses.dataclass
+class Point:
+  x: float = 0.0
+  y: float = 0.0
+  label: str = ''
+  enable: bool = False
+
+
+def greet(greeting: str = 'Hello', targets: Sequence[str] = ('world',)) -> str:
+  return greeting + ' ' + ', '.join(targets)  # pytype: disable=unsupported-operands
+
+
+class DefineAutoTest(absltest.TestCase):
+
+  def test_dataclass(self):
+    flag_values = flags.FlagValues()
+    flag_holder = _define_auto.DEFINE_auto(
+        'point', Point, flag_values=flag_values
+    )
+    flag_values((
+        './program',
+        '--point.x=2.0',
+        '--point.y=-1.5',
+        '--point.label=p',
+        '--nopoint.enable',
+    ))
+    expected = Point(2.0, -1.5, 'p', False)
+    self.assertEqual(expected, flag_holder.value())
+
+  def test_dataclass_nodefaults(self):
+    # Given a class constructor with non-default (required) argument(s)...
+
+    @dataclasses.dataclass
+    class MySettings:
+      foo: str
+      bar: int = 3
+
+    # If we define auto flags for it...
+    flag_values = flags.FlagValues()
+    flag_holder = _define_auto.DEFINE_auto(
+        'thing', MySettings, flag_values=flag_values
+    )
+
+    # Then the corresponding flag is required: not passing it should error.
+    with self.assertRaisesRegex(flags.IllegalFlagValueError, 'thing.foo'):
+      flag_values(('./program', ''))
+
+    # Passing the required flag should work as normal.
+    flag_values(('./program', '--thing.foo=hello'))
+    expected = MySettings('hello', 3)
+    self.assertEqual(expected, flag_holder.value())
+
+  def test_function(self):
+    flag_values = flags.FlagValues()
+    flag_holder = _define_auto.DEFINE_auto(
+        'greet', greet, flag_values=flag_values
+    )
+    flag_values((
+        './program',
+        '--greet.greeting=Hi there',
+        "--greet.targets=('Alice', 'Bob')",
+    ))
+    expected = 'Hi there Alice, Bob'
+    self.assertEqual(expected, flag_holder.value())
+
+  def test_override_kwargs(self):
+    flag_values = flags.FlagValues()
+    flag_holder = _define_auto.DEFINE_auto(
+        'point', Point, flag_values=flag_values
+    )
+    flag_values((
+        './program',
+        '--point.x=2.0',
+        '--point.y=-1.5',
+        '--point.label=p',
+        '--point.enable',
+    ))
+    expected = Point(3.0, -1.5, 'p', True)
+    # Here we override one of the arguments.
+    self.assertEqual(expected, flag_holder.value(x=3.0))
+
+  def test_overriding_top_level_auto_flag_fails(self):
+    flag_values = flags.FlagValues()
+    _define_auto.DEFINE_auto('point', Point, flag_values=flag_values)
+    with self.assertRaisesRegex(
+        flags.IllegalFlagValueError, "Can't override an auto flag directly"
     ):
-      pass
-    # pylint: enable=unused-argument
-    expected_settings = {
-        'str_': 'foo',
-        'int_': 10,
-        'enum_': MyEnum.ZERO,
-    }
-    ff_dict = ff.auto(my_function)
-    self.assertCountEqual(expected_settings, ff_dict)
-
-  def test_works_class(self):
-
-    class MyClass:
-
-      # pylint: disable=unused-argument
-      def __init__(
-          self,
-          str_: str = 'foo',
-          int_: int = 10,
-          float_: float = 1.0,
-          bool_: bool = False,
-          list_int: List[int] = [1, 2, 3],
-          tuple_str: Tuple[str] = ('foo',),
-          sequence_bool: Sequence[bool] = [True, False],
-          optional_int: Optional[int] = None,
-          optional_float: Optional[float] = None,
-          optional_list_int: Optional[List[int]] = None,
-      ):  # pylint: disable=dangerous-default-value
-        pass
-      # pylint: enable=unused-argument
-    expected_settings = {
-        'str_': 'foo',
-        'int_': 10,
-        'float_': 1.0,
-        'bool_': False,
-        'list_int': [1, 2, 3],
-        'tuple_str': ('foo',),
-        'sequence_bool': [True, False],
-        'optional_int': None,
-        'optional_float': None,
-        'optional_list_int': None,
-    }
-    ff_dict = ff.auto(MyClass)
-    self.assertCountEqual(expected_settings, ff_dict)
-    ff.DEFINE_dict('my_class_settings', **ff_dict)
-    self.assertEqual(FLAGS.my_class_settings, expected_settings)
-
-  def test_works_metaclass(self):
-
-    # This replicates an issue with Sonnet v2 modules, where the constructor
-    # arguments are hidden by the metaclass.
-    class MyMetaclass(abc.ABCMeta):
-
-      def __call__(cls, *args, **kwargs):
-        del args, kwargs
-
-    class MyClass(metaclass=MyMetaclass):
-
-      def __init__(self,
-                   a: int = 10,
-                   b: float = 1.0,
-                   c: Sequence[int] = (1, 2, 3)):
-        del a, b, c
-
-    ff_dict = ff.auto(MyClass)
-    self.assertEqual(['a', 'b', 'c'], list(ff_dict))
-
-    ff.DEFINE_dict('my_meta_class_settings', **ff_dict)
-    self.assertEqual(FLAGS.my_meta_class_settings['a'], 10)
-    self.assertEqual(FLAGS.my_meta_class_settings['b'], 1.0)
-    self.assertEqual(FLAGS.my_meta_class_settings['c'], (1, 2, 3))
-
-  def test_error_if_missing_default_value(self):
-    def my_function(a: int, b: float = 1.0, c: Sequence[int] = (1, 2, 3)):
-      del a, b, c
-
-    with self.assertRaisesWithLiteralMatch(
-        ValueError, _auto._MISSING_DEFAULT_VALUE.format(name='a')):
-      ff.auto(my_function)
-
-  def test_error_if_missing_type_annotation(self):
-    def my_function(a: int = 10, b=1.0, c: Sequence[int] = (1, 2, 3)):
-      del a, b, c
-
-    with self.assertRaisesWithLiteralMatch(
-        TypeError, _auto._MISSING_TYPE_ANNOTATION.format(name='b')):
-      ff.auto(my_function)
-
-  def test_error_if_unsupported_type(self):
-
-    def my_function(a: int = 10,
-                    b: float = 1.0,
-                    c: Sequence[object] = (1, 2, 3)):
-      del a, b, c
-
-    with self.assertRaisesWithLiteralMatch(
-        TypeError,
-        _auto._UNSUPPORTED_ARGUMENT_TYPE.format(
-            name='c', annotation=Sequence[object])):
-      ff.auto(my_function)
-
-  def test_no_error_if_nonstrict_unsupported_type(self):
-
-    def my_function(a: int = 10,
-                    b: float = 1.0,
-                    c: Sequence[object] = (1, 2, 3)):
-      del a, b, c
+      flag_values(('./program', '--point=2.0'))
 
-    return_dict = ff.auto(my_function, strict=False)
-    self.assertSetEqual(set(return_dict.keys()), {'a', 'b'})
+  def test_basic_serialization(self):
+    flag_values = flags.FlagValues()
+    _define_auto.DEFINE_auto('point', Point, flag_values=flag_values)
+
+    # Accessing flag_holder.value would raise an error here, since flags haven't
+    # been parsed yet. For consistency we access the value via flag_values
+    # throughout the test, rather than through a returned `FlagHolder`.
+    initial_point_value = copy.deepcopy(flag_values['point'].value())
+
+    # Parse flags, then serialize.
+    flag_values((
+        './program',
+        '--point.x=1.2',
+        '--point.y=3.5',
+        '--point.label=p',
+        '--point.enable=True',
+    ))
+
+    self.assertEqual(flag_values['point'].serialize(), _flags._EMPTY)
+    self.assertEqual(flag_values['point.x'].serialize(), '--point.x=1.2')
+    self.assertEqual(flag_values['point.label'].serialize(), '--point.label=p')
+    self.assertEqual(flag_values['point.enable'].serialize(), '--point.enable')
+
+    parsed_point_value = copy.deepcopy(flag_values['point'].value())
+
+    self.assertEqual(
+        parsed_point_value, Point(x=1.2, y=3.5, label='p', enable=True)
+    )
+    self.assertNotEqual(parsed_point_value, initial_point_value)
+
+    # Test a round trip.
+    serialized_args = [
+        flag_values[name].serialize()
+        for name in flag_values
+        if name.startswith('point.')
+    ]
+
+    flag_values.unparse_flags()  # Reset to defaults
+    self.assertEqual(flag_values['point'].value(), initial_point_value)
+
+    flag_values(['./program'] + serialized_args)
+    self.assertEqual(flag_values['point'].value(), parsed_point_value)
+
+  def test_disclaimed_module(self):
+    flag_values = flags.FlagValues()
+    _ = _define_auto.DEFINE_auto(
+        'greet', greet, 'help string', flag_values=flag_values
+    )
+    defining_module = flag_values.find_module_defining_flag('greet')
+
+    # The defining module should be the calling module, not the module where
+    # the flag is defined. Otherwise the help for a module's flags will not be
+    # printed unless the user uses --helpfull.
+    self.assertIn('_define_auto_test', defining_module)
+
+  def test_help_strings(self):
+    flag_values = flags.FlagValues()
+
+    # Should default to module.name, since the `greet` docstring is empty.
+    _define_auto.DEFINE_auto('greet', greet, flag_values=flag_values)
+    # Should use the custom help string.
+    _define_auto.DEFINE_auto(
+        'point', Point, help_string='custom', flag_values=flag_values
+    )
+
+    self.assertEqual(flag_values['greet'].help, f'{greet.__module__}.greet')
+    self.assertEqual(flag_values['point'].help, 'custom')
+
+  def test_manual_nostrict_overrides_no_default(self):
+    # Given a function without type hints...
+    def my_function(a):
+      return a + 1  # pytype: disable=unsupported-operands
+
+    # If we define an auto flag using this function in non-strict mode...
+    flag_values = flags.FlagValues()
+    flag_holder = _define_auto.DEFINE_auto(
+        'foo', my_function, flag_values=flag_values, strict=False
+    )
 
-  def test_error_if_not_callable(self):
+    # Calling the function without arguments should error.
+    flag_values(('./program', ''))
     with self.assertRaises(TypeError):
-      ff.auto(3)  # pytype: disable=wrong-arg-types
+      flag_holder.value()  # pytype: disable=missing-parameter
+
+    # Calling with arguments should work fine.
+    self.assertEqual(flag_holder.value(a=2), 3)  # pytype: disable=wrong-arg-types
+
+  def test_skip_params(self):
+    flag_values = flags.FlagValues()
+    _define_auto.DEFINE_auto(
+        'greet', greet, flag_values=flag_values, skip_params=('targets',)
+    )
+    self.assertNotIn('greet.targets', flag_values)
 
-  # TODO(b/178129474): Improve support for typing.Sequence subtypes.
-  @absltest.expectedFailure
-  def test_supports_tuples_with_more_than_one_element(self):
-
-    def my_function(three_ints: Tuple[int, int, int] = (1, 2, 3),
-                    zero_or_more_strings: Tuple[str, ...] = ('foo', 'bar')):
-      del three_ints, zero_or_more_strings
-    expected_settings = {
-        'three_ints': (1, 2, 3),
-        'zero_or_more_strings': ('foo', 'bar'),
-    }
-    ff_dict = ff.auto(my_function)
-    self.assertCountEqual(expected_settings, ff_dict)
-    ff.DEFINE_dict('my_function_settings', **ff_dict)
-    self.assertEqual(FLAGS.my_function_settings, expected_settings)
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `fancyflags-1.1/fancyflags/_define_auto.py` & `fancyflags-1.2/fancyflags/_define_auto.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,34 +10,36 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or  implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """Automatic flags via ff.auto-compatible callables."""
 
-from typing import Optional, TypeVar
+from typing import Callable, Collection, Optional, TypeVar
 
 from absl import flags
 from fancyflags import _auto
 from fancyflags import _definitions
 from fancyflags import _flags
 
-# TODO(jaslanides): Bound this by Callable once our LSP supports it.
-_T = TypeVar('_T')
+_F = TypeVar('_F', bound=Callable)
 
 # Add current module to disclaimed module ids.
 flags.disclaim_key_flags()
 
 
 def DEFINE_auto(  # pylint: disable=invalid-name
     name: str,
-    fn: _T,
+    fn: _F,
     help_string: Optional[str] = None,
     flag_values: flags.FlagValues = flags.FLAGS,
-) -> _flags.TypedFlagHolder[_T]:
+    *,
+    strict: bool = True,
+    skip_params: Collection[str] = (),
+) -> flags.FlagHolder[_F]:
   """Defines a flag for an `ff.auto`-compatible constructor or callable.
 
   Automatically defines a set of dotted `ff.Item` flags corresponding to the
   constructor arguments and their default values.
 
   Overriding the value of a dotted flag will update the arguments used to invoke
   `fn`. This flag's value returns a callable `fn` with these values as bound
@@ -66,29 +68,31 @@
 
   Args:
     name: The name for the top-level flag.
     fn: An `ff.auto`-compatible `Callable`.
     help_string: Optional help string for this flag. If not provided, this will
       default to '{fn's module}.{fn's name}'.
     flag_values: An optional `flags.FlagValues` instance.
+    strict: Whether to skip flag definitions for arguments without type hints,
+      or for arguments with unknown types.
+    skip_params: Optional parameter names to skip defining flags for.
 
   Returns:
     A `flags.FlagHolder`.
   """
-  arguments = _auto.auto(fn)
+  arguments = _auto.auto(fn, strict=strict, skip_params=skip_params)
   # Define the individual flags.
   defaults = _definitions.define_flags(name, arguments, flag_values=flag_values)
   help_string = help_string or f'{fn.__module__}.{fn.__name__}'
   # Define a holder flag.
-  holder = flags.DEFINE_flag(
+  return flags.DEFINE_flag(
       flag=_flags.AutoFlag(
           fn,
           defaults,
           name=name,
           default=None,
           parser=flags.ArgumentParser(),
           serializer=None,
-          help_string=help_string),
+          help_string=help_string,
+      ),
       flag_values=flag_values,
   )
-
-  return _flags.TypedFlagHolder(holder)
```

### Comparing `fancyflags-1.1/fancyflags/_definitions.py` & `fancyflags-1.2/fancyflags/_definitions.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,22 +15,20 @@
 """Functionality for defining `Item`s and dict flags."""
 
 import collections
 import enum
 from typing import Any, Generic, Iterable, Mapping, Optional, Type, TypeVar, Union
 
 from absl import flags
-
 from fancyflags import _argument_parsers
 from fancyflags import _flags
-# internal imports: usage_logging
 
 _T = TypeVar("_T")
-_EnumType = TypeVar("_EnumType", bound=enum.Enum)
-_MappingType = TypeVar("_MappingType", bound=Mapping[str, Any])
+_EnumT = TypeVar("_EnumT", bound=enum.Enum)
+_MappingT = TypeVar("_MappingT", bound=Mapping[str, Any])
 
 SEPARATOR = "."
 
 _NOT_A_DICT_OR_ITEM = """
 DEFINE_dict only supports flat or nested dictionaries, and these must contain
 `ff.Item`s or `ff.MultiItems. Found type {} in this definition.
 """
@@ -76,79 +74,89 @@
   above:
 
   ```
   python script_name.py -- --image_settings.sizes.height=10
   ```
 
   Args:
-    *args: One or two positional arguments are expected:
-        1. A string containing the root name for this flag. This must be set.
-        2. Optionally, a `flags.FlagValues` object that will hold the Flags.
-           If not set, the usual global `flags.FLAGS` object will be used.
+    *args: One or two positional arguments are expected: 1. A string containing
+      the root name for this flag. This must be set. 2. Optionally, a
+      `flags.FlagValues` object that will hold the Flags. If not set, the usual
+      global `flags.FLAGS` object will be used.
     **kwargs: One or more keyword arguments, where the value is either an
       `ff.Item` such as `ff.String(...)` or `ff.Integer(...)` or a dict with the
       same constraints.
 
   Returns:
     A `FlagHolder` instance.
   """
   if not args:
-    raise ValueError("Please supply one positional argument containing the "
-                     "top-level flag name for the dict.")
+    raise ValueError(
+        "Please supply one positional argument containing the "
+        "top-level flag name for the dict."
+    )
 
   if not kwargs:
-    raise ValueError("Please supply at least one keyword argument defining a "
-                     "flag.""")
+    raise ValueError(
+        "Please supply at least one keyword argument defining a flag."
+    )
   if len(args) > 2:
-    raise ValueError("Please supply at most two positional arguments, the "
-                     "first containing the top-level flag name for the dict "
-                     "and, optionally and unusually, a second positional "
-                     "argument to override the flags.FlagValues instance to "
-                     "use.")
+    raise ValueError(
+        "Please supply at most two positional arguments, the "
+        "first containing the top-level flag name for the dict "
+        "and, optionally and unusually, a second positional "
+        "argument to override the flags.FlagValues instance to "
+        "use."
+    )
 
   if not isinstance(args[0], str):
-    raise ValueError("The first positional argument must be a string "
-                     "containing top-level flag name for the dict. Got a {}.".
-                     format(type(args[0]).__name__))
+    raise ValueError(
+        "The first positional argument must be a string "
+        "containing top-level flag name for the dict. Got a {}.".format(
+            type(args[0]).__name__
+        )
+    )
 
   if len(args) == 2:
     if not isinstance(args[1], flags.FlagValues):
-      raise ValueError("If supplying a second positional argument, this must "
-                       "be a flags.FlagValues instance. Got a {}. If you meant "
-                       "to define a flag, note these must be supplied as "
-                       "keyword arguments. ".format(type(args[1]).__name__))
+      raise ValueError(
+          "If supplying a second positional argument, this must "
+          "be a flags.FlagValues instance. Got a {}. If you meant "
+          "to define a flag, note these must be supplied as "
+          "keyword arguments. ".format(type(args[1]).__name__)
+      )
     flag_values = args[1]
   else:
     flag_values = flags.FLAGS
 
   flag_name = args[0]
 
   shared_dict = define_flags(flag_name, kwargs, flag_values=flag_values)
 
-  # usage_logging: dict
-
   # TODO(b/177672282): Can we persuade pytype to correctly infer the type of the
   #                    flagholder's .value attribute?
   # We register a dummy flag that returns `shared_dict` as a value.
   return flags.DEFINE_flag(
       _flags.DictFlag(
           shared_dict,
           name=flag_name,
           default=shared_dict,
           parser=flags.ArgumentParser(),
           serializer=None,
-          help_string="Unused help string."),
-      flag_values=flag_values)
+          help_string="Unused help string.",
+      ),
+      flag_values=flag_values,
+  )
 
 
 def define_flags(
     name: str,
-    name_to_item: _MappingType,
+    name_to_item: _MappingT,
     flag_values: flags.FlagValues = flags.FLAGS,
-) -> _MappingType:
+) -> _MappingT:
   """Defines dot-delimited flags from a flat or nested dict of `ff.Item`s.
 
   Args:
     name: The top-level name to prepend to each flag.
     name_to_item: A flat or nested dictionary, where each final value is an
       `ff.Item` such as `ff.String(...)` or `ff.Integer(...)`.
     flag_values: The `flags.FlagValues` instance to use. By default this is
@@ -167,23 +175,24 @@
   # We create flags for each leaf item (e.g. ff.Integer(...)).
 
   # These are the flags that users will actually interact with when overriding
   # flags from the command line, however they will not access directly in their
   # scripts. It is also the job of these flags to update the corresponding
   # values in `shared_dict`, whenever their own values change.
 
-  def recursively_define_flags(namespace, maybe_definition):
-    if isinstance(maybe_definition, dict):
-      for key, value in maybe_definition.items():
+  def recursively_define_flags(namespace, maybe_item):
+    if isinstance(maybe_item, collections.abc.Mapping):
+      for key, value in maybe_item.items():
         recursively_define_flags(namespace + (key,), value)
     else:
-      maybe_definition.define(namespace, {name: shared_dict}, flag_values)
+      assert isinstance(maybe_item, (Item, MultiItem))
+      maybe_item.define(namespace, {name: shared_dict}, flag_values)
 
   for key, value in name_to_item.items():
-    recursively_define_flags(namespace=(name, key), maybe_definition=value)
+    recursively_define_flags(namespace=(name, key), maybe_item=value)
 
   return shared_dict
 
 
 def _extract_defaults(name_to_item):
   """Converts a flat or nested dict into a flat or nested dict of defaults."""
 
@@ -204,39 +213,49 @@
 
   def __init__(
       self,
       default: Optional[_T],
       help_string: str,
       parser: flags.ArgumentParser,
       serializer: Optional[flags.ArgumentSerializer] = None,
+      *,
+      required: bool = False,
   ):
     """Initializes a new `Item`.
 
     Args:
       default: Default value of the flag that this instance will create.
       help_string: Help string for the flag that this instance will create. If
         `None`, then the dotted flag name will be used as the help string.
       parser: A `flags.ArgumentParser` used to parse command line input.
       serializer: An optional custom `flags.ArgumentSerializer`. By default, the
         flag defined by this class will use an instance of the base
         `flags.ArgumentSerializer`.
+      required: Whether or not this item is required. If True, the corresponding
+        abseil flag will be marked as required.
     """
     # Flags run the following lines of parsing code during initialization.
     # See Flag._set_default in absl/flags/_flag.py
 
     # It's useful to repeat it here so that users will see any errors when the
     # Item is initialized, rather than when define() is called later.
 
     # The only minor difference is that Flag._set_default calls Flag._parse,
     # which also catches and modifies the exception type.
     if default is None:
       self.default = default
     else:
+      if required:
+        # Mirror the strict behavior of abseil flags.
+        raise ValueError(
+            "If marking an Item as required, the default must be None."
+        )
       self.default = parser.parse(default)  # pytype: disable=wrong-arg-types
 
+    self.required = required
     self._help_string = help_string
     self._parser = parser
 
     if serializer is None:
       self._serializer = flags.ArgumentSerializer()
     else:
       self._serializer = serializer
@@ -249,17 +268,17 @@
   ) -> flags.FlagHolder[_T]:
     """Defines a flag that when parsed will update a shared dictionary.
 
     Args:
       namespace: A sequence of strings that define the name of this flag. For
         example, `("foo", "bar")` will correspond to a flag named `foo.bar`.
       shared_dict: A dictionary that is shared by the top level dict flag. When
-        the individual flag created by this method is parsed, it will also
-        write the parsed value into `shared_dict`. The `namespace` determines
-        the flat or nested key when storing the parsed value.
+        the individual flag created by this method is parsed, it will also write
+        the parsed value into `shared_dict`. The `namespace` determines the flat
+        or nested key when storing the parsed value.
       flag_values: The `flags.FlagValues` instance to use.
 
     Returns:
       A new flags.FlagHolder instance.
     """
     name = SEPARATOR.join(namespace)
     help_string = name if self._help_string is None else self._help_string
@@ -267,80 +286,108 @@
         _flags.ItemFlag(
             shared_dict,
             namespace,
             parser=self._parser,
             serializer=self._serializer,
             name=name,
             default=self.default,
-            help_string=help_string),
-        flag_values=flag_values)
+            help_string=help_string,
+        ),
+        flag_values=flag_values,
+        required=self.required,
+    )
 
 
 class Boolean(Item[bool]):
   """Matches behaviour of flags.DEFINE_boolean."""
 
-  def __init__(self,
-               default: Optional[bool],
-               help_string: Optional[str] = None):
-    super().__init__(default, help_string, flags.BooleanParser())
+  def __init__(
+      self,
+      default: Optional[bool],
+      help_string: Optional[str] = None,
+      *,
+      required: bool = False,
+  ):
+    super().__init__(
+        default,
+        help_string,
+        flags.BooleanParser(),
+        required=required,
+    )
 
 
 # TODO(b/177673597) Better document the different enum class options and
 #                   possibly recommend some over others.
 
 
 class Enum(Item[str]):
   """Matches behaviour of flags.DEFINE_enum."""
 
   def __init__(
       self,
       default: Optional[str],
       enum_values: Iterable[str],
       help_string: Optional[str] = None,
+      *,
       case_sensitive: bool = True,
+      required: bool = False,
   ):
     parser = flags.EnumParser(tuple(enum_values), case_sensitive)
-    super().__init__(default, help_string, parser)
+    super().__init__(default, help_string, parser, required=required)
 
 
-class EnumClass(Item[_EnumType]):
+class EnumClass(Item[_EnumT]):
   """Matches behaviour of flags.DEFINE_enum_class."""
 
   def __init__(
       self,
-      default: Optional[_EnumType],
-      enum_class: Type[_EnumType],
+      default: Optional[_EnumT],
+      enum_class: Type[_EnumT],
       help_string: Optional[str] = None,
+      *,
+      case_sensitive: bool = False,
+      required: bool = False,
   ):
-    parser = flags.EnumClassParser(enum_class)
+    parser = flags.EnumClassParser(enum_class, case_sensitive=case_sensitive)
     super().__init__(
-        default, help_string, parser,
-        flags.EnumClassSerializer(lowercase=False))
+        default,
+        help_string,
+        parser,
+        flags.EnumClassSerializer(lowercase=False),
+        required=required,
+    )
 
 
 class Float(Item[float]):
   """Matches behaviour of flags.DEFINE_float."""
 
   def __init__(
       self,
       default: Optional[float],
       help_string: Optional[str] = None,
+      *,
+      required: bool = False,
   ):
-    super().__init__(default, help_string, flags.FloatParser())
+    super().__init__(
+        default, help_string, flags.FloatParser(), required=required
+    )
 
 
 class Integer(Item[int]):
   """Matches behaviour of flags.DEFINE_integer."""
 
   def __init__(
       self,
       default: Optional[int],
       help_string: Optional[str] = None,
+      required: bool = False,
   ):
-    super().__init__(default, help_string, flags.IntegerParser())
+    super().__init__(
+        default, help_string, flags.IntegerParser(), required=required
+    )
 
 
 class Sequence(Item, Generic[_T]):
   r"""Defines a flag for a list or tuple of simple numeric types or strings.
 
   Here is an example of overriding a Sequence flag within a dict-flag named
   "settings" from the command line, with a list of values.
@@ -357,23 +404,57 @@
   ```
   """
 
   def __init__(
       self,
       default: Optional[Iterable[_T]],
       help_string: Optional[str] = None,
+      required: bool = False,
   ):
-    super().__init__(default, help_string, _argument_parsers.SequenceParser())
+    super().__init__(
+        default,
+        help_string,
+        _argument_parsers.SequenceParser(),
+        required=required,
+    )
 
 
 class String(Item[str]):
   """Matches behaviour of flags.DEFINE_string."""
 
-  def __init__(self, default: Optional[str], help_string: Optional[str] = None):
-    super().__init__(default, help_string, flags.ArgumentParser())
+  def __init__(
+      self,
+      default: Optional[str],
+      help_string: Optional[str] = None,
+      *,
+      required: bool = False,
+  ):
+    super().__init__(
+        default,
+        help_string,
+        flags.ArgumentParser(),
+        required=required,
+    )
+
+
+class DateTime(Item):
+
+  def __init__(
+      self,
+      default: Optional[str],
+      help_string: Optional[str] = None,
+      *,
+      required: bool = False,
+  ):
+    super(DateTime, self).__init__(
+        default,
+        help_string,
+        _argument_parsers.PossiblyNaiveDatetimeParser(),
+        required=required,
+    )
 
 
 class StringList(Item[Iterable[str]]):
   """A flag that implements the same behavior as absl.flags.DEFINE_list.
 
   Can be overwritten as --my_flag="a,list,of,commaseparated,strings"
   """
@@ -402,16 +483,17 @@
       help_string: str,
       parser: flags.ArgumentParser,
       serializer: Optional[flags.ArgumentSerializer] = None,
   ):
     if default is None:
       self.default = default
     else:
-      if (isinstance(default, collections.abc.Iterable) and
-          not isinstance(default, (str, bytes))):
+      if isinstance(default, collections.abc.Iterable) and not isinstance(
+          default, (str, bytes)
+      ):
         # Convert all non-string iterables to lists.
         default = list(default)
 
       if not isinstance(default, list):
         # Turn single items into single-value lists.
         default = [default]
 
@@ -438,16 +520,18 @@
         _flags.MultiItemFlag(
             shared_dict,
             namespace,
             parser=self._parser,
             serializer=self._serializer,
             name=name,
             default=self.default,
-            help_string=help_string),
-        flag_values=flag_values)
+            help_string=help_string,
+        ),
+        flag_values=flag_values,
+    )
 
 
 class MultiEnum(Item[_T]):
   """Defines a flag for lists of values of any type, matched to enum_values."""
 
   def __init__(
       self,
@@ -462,16 +546,16 @@
 
 
 class MultiEnumClass(MultiItem):
   """Matches behaviour of flags.DEFINE_multi_enum_class."""
 
   def __init__(
       self,
-      default: Union[None, _EnumType, Iterable[_EnumType]],
-      enum_class: Type[_EnumType],
+      default: Union[None, _EnumT, Iterable[_EnumT]],
+      enum_class: Type[_EnumT],
       help_string: Optional[str] = None,
   ):
     parser = flags.EnumClassParser(enum_class)
     serializer = flags.EnumClassListSerializer(",", lowercase=False)
     super().__init__(default, help_string, parser, serializer)
 
 
@@ -494,25 +578,37 @@
     help: str,
     flag_values=flags.FLAGS,
     **args,
 ) -> flags.FlagHolder[_T]:
   """Defines flag for MultiEnum."""
   parser = _argument_parsers.MultiEnumParser(enum_values)
   serializer = flags.ArgumentSerializer()
-  # usage_logging: multi_enum
-  return flags.DEFINE(parser, name, default, help, flag_values, serializer,
-                      **args,)
+  return flags.DEFINE(
+      parser,
+      name,
+      default,
+      help,
+      flag_values,
+      serializer,
+      **args,
+  )
 
 
 def DEFINE_sequence(  # pylint: disable=invalid-name,redefined-builtin
     name: str,
     default: Optional[Iterable[_T]],
     help: str,
     flag_values=flags.FLAGS,
     **args,
 ) -> flags.FlagHolder[Iterable[_T]]:
   """Defines a flag for a list or tuple of simple types. See `Sequence` docs."""
   parser = _argument_parsers.SequenceParser()
   serializer = flags.ArgumentSerializer()
-  # usage_logging: sequence
-  return flags.DEFINE(parser, name, default, help, flag_values, serializer,
-                      **args,)
+  return flags.DEFINE(
+      parser,
+      name,
+      default,
+      help,
+      flag_values,
+      serializer,
+      **args,
+  )
```

### Comparing `fancyflags-1.1/fancyflags/_flags.py` & `fancyflags-1.2/fancyflags/_flags.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """Flag classes for defining dict, Item, MultiItem and Auto flags."""
 
 import copy
 import functools
-from typing import Generic, TypeVar
 
 from absl import flags
 
 _EMPTY = ""
-_T = TypeVar("_T")
 
 
 class DictFlag(flags.Flag):
   """Implements the shared dict mechanism. See also `ItemFlag`."""
 
   def __init__(self, shared_dict, *args, **kwargs):
     self._shared_dict = shared_dict
@@ -43,41 +41,50 @@
     #    flags, e.g. to pass values between processes, so we accept a dummy
     #    empty serialized value for these cases. It's unlikely users will try to
     #    set the dict flag to an empty string from the command line.
     if value is self._shared_dict or value == _EMPTY:
       return self._shared_dict
     raise flags.IllegalFlagValueError(
         "Can't override a dict flag directly. Did you mean to override one of "
-        "its `Item`s instead?")
+        "its `Item`s instead?"
+    )
 
   def serialize(self):
     # When serializing flags, we return a sentinel value that the `DictFlag`
     # will ignore when parsing. The value of this flag is determined by the
     # corresponding `Item` flags for serialization and deserialization.
     return _EMPTY
 
   def flag_type(self):
     return "dict"
 
+
 # TODO(b/170423907): Pytype doesn't correctly infer that these have type
 #                    `property`.
-_flag_value_property = flags.Flag.value  # type: property  # pytype: disable=annotation-type-mismatch
+_flag_value_property = flags.Flag.value  # type: property  # pytype: disable=annotation-type-mismatch,unbound-type-param
 _multi_flag_value_property = flags.MultiFlag.value  # type: property  # pytype: disable=annotation-type-mismatch
 
 
 class ItemFlag(flags.Flag):
   """Updates a shared dict whenever its own value changes.
 
   See also the `DictFlag` and `ff.Item` classes for usage.
   """
 
-  def __init__(self, shared_dict, namespace, *args, **kwargs):
+  def __init__(self, shared_dict, namespace, parser, *args, **kwargs):
     self._shared_dict = shared_dict
     self._namespace = namespace
-    super().__init__(*args, **kwargs)
+    super().__init__(
+        *args,
+        parser=parser,
+        # absl treats boolean flags as a special case in order to support the
+        # alternative `--foo`/`--nofoo` syntax.
+        boolean=isinstance(parser, flags.BooleanParser),
+        **kwargs
+    )
 
   # `super().value = value` doesn't work, see https://bugs.python.org/issue14965
   @_flag_value_property.setter
   def value(self, value):
     _flag_value_property.fset(self, value)
     self._update_shared_dict()
 
@@ -154,46 +161,19 @@
     #    flags, e.g. to pass values between processes, so we accept a dummy
     #    empty serialized value for these cases. It's unlikely users will try to
     #    set the auto flag to an empty string from the command line.
     if value is None or value == _EMPTY:
       return None
     raise flags.IllegalFlagValueError(
         "Can't override an auto flag directly. Did you mean to override one of "
-        "its `Item`s instead?")
+        "its `Item`s instead?"
+    )
 
   def serialize(self):
     # When serializing a `FlagHolder` container, we must return *some* value for
     # this flag. We return an empty value that the `AutoFlag` will ignore when
     # parsing. The value of this flag is instead determined by the
     # corresponding `Item` flags for serialization and deserialization.
     return _EMPTY
 
   def flag_type(self):
     return "auto"
-
-
-class TypedFlagHolder(flags.FlagHolder, Generic[_T]):
-  """A typed wrapper for a FlagHolder.
-
-  This is necessary until either Pytype supports PEP-562 (b/170419518), or
-  abseil-py drops Python 2 support (b/182444583) and moves their type hints
-  into the source.
-  """
-
-  def __init__(self, flag_holder: flags.FlagHolder[_T]):
-    self._flag_holder = flag_holder
-
-  @property
-  def value(self) -> _T:
-    return self._flag_holder.value
-
-  @property
-  def default(self) -> _T:
-    return self._flag_holder.default
-
-  @property
-  def name(self) -> str:
-    return self._flag_holder.name
-
-  @property
-  def present(self) -> bool:
-    return self._flag_holder.present
```

### Comparing `fancyflags-1.1/fancyflags/_flags_test.py` & `fancyflags-1.2/fancyflags/_flags_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,18 @@
         _flags.ItemFlag(
             shared_dict,
             namespace,
             parser=flags.ArgumentParser(),
             serializer=flags.ArgumentSerializer(),
             name='a.b',
             default='bar',
-            help_string='help string'),
-        flag_values=flag_values)
+            help_string='help string',
+        ),
+        flag_values=flag_values,
+    )
 
     flag_values['a.b'].value = 'new_value'
     with self.subTest(name='setter'):
       self.assertEqual(shared_dict, {'a': {'b': 'new_value'}})
 
     flag_values(('./program', '--a.b=override'))
     with self.subTest(name='override_parse'):
@@ -56,20 +58,23 @@
         _flags.MultiItemFlag(
             shared_dict,
             namespace,
             parser=flags.ArgumentParser(),
             serializer=flags.ArgumentSerializer(),
             name='a.b',
             default=['foo', 'bar'],
-            help_string='help string'),
-        flag_values=flag_values)
+            help_string='help string',
+        ),
+        flag_values=flag_values,
+    )
 
     flag_values['a.b'].value = ['new', 'value']
     with self.subTest(name='setter'):
       self.assertEqual(shared_dict, {'a': {'b': ['new', 'value']}})
 
     flag_values(('./program', '--a.b=override1', '--a.b=override2'))
     with self.subTest(name='override_parse'):
       self.assertEqual(shared_dict, {'a': {'b': ['override1', 'override2']}})
 
+
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `fancyflags-1.1/fancyflags/_flagsaver_test.py` & `fancyflags-1.2/fancyflags/_flagsaver_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,35 +31,38 @@
 
 FLAGS = flags.FLAGS
 
 
 class FlagSaverTest(absltest.TestCase):
 
   def test_flagsaver_with_context_overrides(self):
-    with flagsaver.flagsaver(**{
-        "string_flag": "new value",
-        "test_dict_flag.dict.nested": -1.0,
-    }):
+    with flagsaver.flagsaver(
+        **{
+            "string_flag": "new value",
+            "test_dict_flag.dict.nested": -1.0,
+        }
+    ):
       self.assertEqual("new value", FLAGS.string_flag)
       self.assertEqual(-1.0, FLAGS.test_dict_flag["dict"]["nested"])
       self.assertEqual(4, FLAGS.test_dict_flag["unnested"])
       FLAGS.string_flag = "another value"
 
     self.assertEqual("unchanged", FLAGS.string_flag)
     self.assertEqual(1.0, FLAGS.test_dict_flag["dict"]["nested"])
 
   def test_flagsaver_with_decorator_overrides(self):
+    # Modeled after test_decorator_with_overrides in
+    # https://github.com/abseil/abseil-py/blob/master/absl/testing/tests/flagsaver_test.py  # pylint: disable=line-too-long
 
-  # Modeled after test_decorator_with_overrides in
-  # https://github.com/abseil/abseil-py/blob/master/absl/testing/tests/flagsaver_test.py  # pylint: disable=line-too-long
-
-    @flagsaver.flagsaver(**{
-        "string_flag": "new value",
-        "test_dict_flag.dict.nested": -1.0,
-    })
+    @flagsaver.flagsaver(
+        **{
+            "string_flag": "new value",
+            "test_dict_flag.dict.nested": -1.0,
+        }
+    )
     def mutate_flags():
       return FLAGS.string_flag, FLAGS.test_dict_flag["dict"]["nested"]
 
     # Values should be overridden in the function.
     self.assertEqual(("new value", -1.0), mutate_flags())
 
     # But unchanged here.
@@ -67,32 +70,36 @@
     self.assertEqual(1.0, FLAGS.test_dict_flag["dict"]["nested"])
 
   def test_flagsaver_with_context_overrides_twice(self):
     # Checking that the flat -> dict flag sync works again after restoration.
     # This might fail if the underlying absl functions copied the dict as part
     # of restoration.
 
-    with flagsaver.flagsaver(**{
-        "string_flag": "new value",
-        "test_dict_flag.dict.nested": -1.0,
-    }):
+    with flagsaver.flagsaver(
+        **{
+            "string_flag": "new value",
+            "test_dict_flag.dict.nested": -1.0,
+        }
+    ):
       self.assertEqual("new value", FLAGS.string_flag)
       self.assertEqual(-1.0, FLAGS.test_dict_flag["dict"]["nested"])
       self.assertEqual(4, FLAGS.test_dict_flag["unnested"])
       FLAGS.string_flag = "another value"
 
     self.assertEqual("unchanged", FLAGS.string_flag)
     self.assertEqual(1.0, FLAGS.test_dict_flag["dict"]["nested"])
 
     # Same again!
 
-    with flagsaver.flagsaver(**{
-        "string_flag": "new value",
-        "test_dict_flag.dict.nested": -1.0,
-    }):
+    with flagsaver.flagsaver(
+        **{
+            "string_flag": "new value",
+            "test_dict_flag.dict.nested": -1.0,
+        }
+    ):
       self.assertEqual("new value", FLAGS.string_flag)
       self.assertEqual(-1.0, FLAGS.test_dict_flag["dict"]["nested"])
       self.assertEqual(4, FLAGS.test_dict_flag["unnested"])
       FLAGS.string_flag = "another value"
 
     self.assertEqual("unchanged", FLAGS.string_flag)
     self.assertEqual(1.0, FLAGS.test_dict_flag["dict"]["nested"])
@@ -105,9 +112,10 @@
       FLAGS["test_dict_flag.dict.nested"].value = -1.0
       FLAGS.test_dict_flag["unnested"] = -1.0
     self.assertEqual("unchanged", FLAGS.string_flag)  # Works.
     self.assertEqual(1.0, FLAGS.test_dict_flag["dict"]["nested"])  # Works.
     # TODO(b/177927157) Fix this behaviour.
     self.assertEqual(4, FLAGS.test_dict_flag["unnested"])  # Broken.
 
+
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `fancyflags-1.1/fancyflags/_metadata.py` & `fancyflags-1.2/fancyflags/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # ============================================================================
 """Package metadata.
 
 This is kept in a separate module so that it can be imported from setup.py, at
 a time when the package dependencies may not have been installed yet.
 """
 
-__version__ = '1.1'  # https://www.python.org/dev/peps/pep-0440/
+__version__ = '1.2'  # https://www.python.org/dev/peps/pep-0440/
```

### Comparing `fancyflags-1.1/fancyflags.egg-info/PKG-INFO` & `fancyflags-1.2/fancyflags.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Metadata-Version: 2.1
 Name: fancyflags
-Version: 1.1
+Version: 1.2
 Summary: A Python library for defining dictionary-valued flags.
-Home-page: UNKNOWN
 Author: DeepMind
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `fancyflags-1.1/fancyflags.egg-info/SOURCES.txt` & `fancyflags-1.2/fancyflags.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fancyflags-1.1/setup.py` & `fancyflags-1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,33 +10,40 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or  implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """Install script for fancyflags."""
 
-import imp
-from setuptools import find_packages
-from setuptools import setup
+from importlib import util
+import setuptools
 
-setup(
+
+def _get_version():
+  spec = util.spec_from_file_location('_metadata', 'fancyflags/_metadata.py')
+  mod = util.module_from_spec(spec)
+  spec.loader.exec_module(mod)
+  return mod.__version__
+
+
+setuptools.setup(
     name='fancyflags',
-    version=imp.load_source('_metadata', 'fancyflags/_metadata.py').__version__,
+    version=_get_version(),
     description='A Python library for defining dictionary-valued flags.',
     author='DeepMind',
     license='Apache License, Version 2.0',
-    packages=find_packages(),
+    packages=setuptools.find_packages(),
     install_requires=['absl-py'],
     tests_require=['pytest'],
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
     ],
 )
```

