# Comparing `tmp/pydoctrace-0.1.0.tar.gz` & `tmp/pydoctrace-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoctrace-0.1.0.tar", max compression
+gzip compressed data, was "pydoctrace-0.1.2.tar", max compression
```

## Comparing `pydoctrace-0.1.0.tar` & `pydoctrace-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-01-07 00:29:11.921070 pydoctrace-0.1.0/LICENSE
--rw-r--r--   0        0        0     7728 2023-02-07 18:49:21.974705 pydoctrace-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-01-07 00:20:47.901184 pydoctrace-0.1.0/pydoctrace/__init__.py
--rw-r--r--   0        0        0     1594 2023-01-17 01:11:34.380327 pydoctrace-0.1.0/pydoctrace/doctrace.py
--rw-r--r--   0        0        0      372 2023-01-14 23:47:24.212945 pydoctrace-0.1.0/pydoctrace/domain/context.py
--rw-r--r--   0        0        0      471 2023-01-17 01:37:21.079318 pydoctrace-0.1.0/pydoctrace/domain/sequence.py
--rw-r--r--   0        0        0     3466 2023-01-17 01:37:42.077908 pydoctrace-0.1.0/pydoctrace/exporters/__init__.py
--rw-r--r--   0        0        0     5493 2023-02-07 00:02:27.413547 pydoctrace-0.1.0/pydoctrace/exporters/plantuml.py
--rw-r--r--   0        0        0     9589 2023-02-07 19:03:04.982659 pydoctrace-0.1.0/pydoctrace/tracer.py
--rw-r--r--   0        0        0     2070 2023-02-05 22:57:32.358147 pydoctrace-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8558 1970-01-01 00:00:00.000000 pydoctrace-0.1.0/setup.py
--rw-r--r--   0        0        0     8471 1970-01-01 00:00:00.000000 pydoctrace-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-01-07 00:29:11.921070 pydoctrace-0.1.2/LICENSE
+-rw-r--r--   0        0        0     8478 2023-07-03 23:25:40.931298 pydoctrace-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-02-07 19:22:30.896275 pydoctrace-0.1.2/pydoctrace/__init__.py
+-rw-r--r--   0        0        0     1594 2023-07-03 23:24:23.300209 pydoctrace-0.1.2/pydoctrace/doctrace.py
+-rw-r--r--   0        0        0      372 2023-02-07 19:22:30.897275 pydoctrace-0.1.2/pydoctrace/domain/context.py
+-rw-r--r--   0        0        0      471 2023-02-07 19:22:30.898275 pydoctrace-0.1.2/pydoctrace/domain/sequence.py
+-rw-r--r--   0        0        0     3466 2023-07-03 23:24:23.300209 pydoctrace-0.1.2/pydoctrace/exporters/__init__.py
+-rw-r--r--   0        0        0     5493 2023-07-03 23:24:23.300209 pydoctrace-0.1.2/pydoctrace/exporters/plantuml.py
+-rw-r--r--   0        0        0     9598 2023-07-03 23:24:23.300209 pydoctrace-0.1.2/pydoctrace/tracer.py
+-rw-r--r--   0        0        0     2069 2023-07-03 23:26:11.279551 pydoctrace-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     9221 1970-01-01 00:00:00.000000 pydoctrace-0.1.2/PKG-INFO
```

### Comparing `pydoctrace-0.1.0/LICENSE` & `pydoctrace-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoctrace-0.1.0/README.md` & `pydoctrace-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/lucsorel/pydoctrace/main.svg)](https://results.pre-commit.ci/latest/github/lucsorel/pydoctrace/main)
+
+`pydoctrace` uses [pre-commit hooks](https://pre-commit.com/) and [pre-commit.ci continuous integration](https://pre-commit.ci/) to enforce commit messages, code formatting and linting for quality and consistency sake.
+See the [code conventions](#code-conventions) section if you would like to contribute to the project.
+
 # pydoctrace
 
 Generate sequence diagrams by tracing Python code execution.
 
 Here are the sequence diagrams produced by 2 different implementations of the `factorial` function (*n * n-1 * n-2 * ... * 1*).
 One which loops, another one that is recursive:
 
@@ -37,17 +42,17 @@
 
     return value * factorial_recursive(value - 1)
 ```
 
 </td>
 </tr>
 <tr>
-<td valign="top"><pre>tests.modules.factorial.factorial_reduce_multiply.puml</pre>
+<td valign="top"><code>tests.modules.factorial.factorial_reduce_multiply.puml</code><br />
 <img src="https://www.plantuml.com/plantuml/svg/rP0nYof148Jp_XMDgUYweZwHnqCqUDaXNEY1Z3kzEZZRlVJsW88__WAvKmurCBhDXgcYwgkUD-RKKXNHgB6cNubFaPf-wGeJ3IvUNnibdmhQL2bQgEC9caFWsgchS277bVC-y0xpmSt_ogc58jIExKiVtyXlOhHmnM6dajWl9OhYKfIR40y_RQAUz69v3yJiO1yyOIbYMpa2hANt3piFHdpmmnKTO3523RkzpJ069Xpb0AyauLE2gwtRlNH6AhyhftSmnW1AbfGnlwDEu7m-_pRGOLj09wsvwAWjfFbmq1RKFyzGrtzxFNo5T_OWTmfGYXWf_YScTKOUjoVCilhafJ1r1MKPp8bzgY9y0W00" /></td>
-<td valign="top"><pre>tests.modules.factorial.factorial_recursive.puml</pre>
+<td valign="top"><code>tests.modules.factorial.factorial_recursive.puml</code><br />
 <img src="https://www.plantuml.com/plantuml/svg/xP31QYf144Nt_HM5Mz5nv3qJ90JHHNP1oD90AAThjB6dIgghWu8Vdu2OI8o8PEkkwNkuzr2ZPAYMcmX6oLAt4PyZfMwDbOa6ZD-lDwKgQmhlvD8gy1eL6nZBPehU1rv0sJlwdw9QgC8QsGxv_wFuMOp6MAqMAfdzHA8eJ4GvXRZwYObwqZto4eWPtJ9uWbh4vh9nRYQTHsYTqN_bN_nRZiK8D2oMDeGOc63Wt7KLSFKejDlxtKZrORRitLHkAdzIKRAi3ELfUEzskzqNq3y5FXkFYS55el_l8bBsU-UPsKEdS-KbXd1tfj7L8aOAJyIaQEHXleMYM6-zLAPOKL6u4R7FJNGV" /></td>
 </tr>
 </tbody>
 </table>
 
 ## Installation
 
@@ -119,14 +124,16 @@
 
 ```sh
 poetry run pytest -v --cov=pydoctrace --cov-branch --cov-report term-missing --cov-fail-under 50
 ```
 
 # Changelog
 
+* `0.1.2`: added github actions for the automated tests and interaction with pre-commit.ci for the code linting
+* `0.1.1`: [deleted release] added github actions for the automated tests and interaction with pre-commit.ci for the code linting
 * `0.1.0`: ✨ first release, PlantUML exporter; diagram files are saved in the current working directory
 
 # Licence
 
 Unless stated otherwise all works are licensed under the [MIT license](http://spdx.org/licenses/MIT.html), a copy of which is included [here](LICENSE).
 
 # Contributions
```

### Comparing `pydoctrace-0.1.0/pydoctrace/doctrace.py` & `pydoctrace-0.1.2/pydoctrace/doctrace.py`

 * *Files identical despite different names*

### Comparing `pydoctrace-0.1.0/pydoctrace/exporters/__init__.py` & `pydoctrace-0.1.2/pydoctrace/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctrace-0.1.0/pydoctrace/exporters/plantuml.py` & `pydoctrace-0.1.2/pydoctrace/exporters/plantuml.py`

 * *Files identical despite different names*

### Comparing `pydoctrace-0.1.0/pydoctrace/tracer.py` & `pydoctrace-0.1.2/pydoctrace/tracer.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     '''
     Traces the execution of a callable object and pushes events to the given exporter.
 
     The implementation of the tracing functions are based on the documentation of:
     - sys.settrace: https://docs.python.org/3/library/sys.html#sys.settrace
     - execution frames: https://docs.python.org/3/reference/datamodel.html#frame-objects
 
-    Useful calls when implementing or debugging features (the contents are added as comments in the exported diagram):
+    Useful calls when implementing or debugging features (the contents are added as PlantUML comments in the exported diagram):
     self.exporter.write_raw_content(f"\n' {event} {frame=} {arg=}\n")
     self.exporter.write_raw_content(f"' {frame.f_back=}\n")
     '''
     def __init__(self, exporter: Exporter):
         self.exporter = exporter
         self.callers_stack: List[Call] = deque()
         self.error_to_handle_with_line: TracedError = None
```

### Comparing `pydoctrace-0.1.0/pyproject.toml` & `pydoctrace-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydoctrace"
-version = "0.1.0"
+version = "0.1.2"
 description = "Generate sequence diagrams by tracing Python code execution"
 keywords = ["sequence diagram", "documentation", "tracing", "doc-as-code", "PlantUML"]
 readme = "README.md"
 repository = "https://github.com/lucsorel/pydoctrace"
 authors = ["Luc Sorel-Giffo"]
 maintainers = ["Luc Sorel-Giffo"]
 license = "MIT"
@@ -13,15 +13,15 @@
 python = "^3.8"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.lint.dependencies]
-pre-commit = "^2.21.0"
+pre-commit = "^3.3.3"
 
 [tool.pytest.ini_options]
 console_output_style = "count"
 
 [tool.isort]
 # maintain consistency with other quality tools
 line_length = 120
```

### Comparing `pydoctrace-0.1.0/setup.py` & `pydoctrace-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,216 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pydoctrace
+Version: 0.1.2
+Summary: Generate sequence diagrams by tracing Python code execution
+Home-page: https://github.com/lucsorel/pydoctrace
+License: MIT
+Keywords: sequence diagram,documentation,tracing,doc-as-code,PlantUML
+Author: Luc Sorel-Giffo
+Maintainer: Luc Sorel-Giffo
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/lucsorel/pydoctrace
+Description-Content-Type: text/markdown
 
-packages = \
-['pydoctrace', 'pydoctrace.domain', 'pydoctrace.exporters']
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/lucsorel/pydoctrace/main.svg)](https://results.pre-commit.ci/latest/github/lucsorel/pydoctrace/main)
 
-package_data = \
-{'': ['*']}
+`pydoctrace` uses [pre-commit hooks](https://pre-commit.com/) and [pre-commit.ci continuous integration](https://pre-commit.ci/) to enforce commit messages, code formatting and linting for quality and consistency sake.
+See the [code conventions](#code-conventions) section if you would like to contribute to the project.
 
-setup_kwargs = {
-    'name': 'pydoctrace',
-    'version': '0.1.0',
-    'description': 'Generate sequence diagrams by tracing Python code execution',
-    'long_description': '# pydoctrace\n\nGenerate sequence diagrams by tracing Python code execution.\n\nHere are the sequence diagrams produced by 2 different implementations of the `factorial` function (*n * n-1 * n-2 * ... * 1*).\nOne which loops, another one that is recursive:\n\n<table>\n<tbody>\n<tr>\n<td valign="bottom">\n\n```python\nfrom pydoctrace.doctrace import trace_to_puml\n\n@trace_to_puml\ndef factorial_reduce_multiply(value: int) -> int:\n    if value <= 1:\n        return value\n\n    def multiply(agg: int, value: int) -> int:\n        return agg * value\n\n    return reduce(multiply, range(1, value + 1), 1)\n```\n\n</td>\n<td valign="bottom">\n\n```python\nfrom pydoctrace.doctrace import trace_to_puml\n\n@trace_to_puml\ndef factorial_recursive(value: int) -> int:\n    if value <= 1:\n        return value\n\n    return value * factorial_recursive(value - 1)\n```\n\n</td>\n</tr>\n<tr>\n<td valign="top"><pre>tests.modules.factorial.factorial_reduce_multiply.puml</pre>\n<img src="https://www.plantuml.com/plantuml/svg/rP0nYof148Jp_XMDgUYweZwHnqCqUDaXNEY1Z3kzEZZRlVJsW88__WAvKmurCBhDXgcYwgkUD-RKKXNHgB6cNubFaPf-wGeJ3IvUNnibdmhQL2bQgEC9caFWsgchS277bVC-y0xpmSt_ogc58jIExKiVtyXlOhHmnM6dajWl9OhYKfIR40y_RQAUz69v3yJiO1yyOIbYMpa2hANt3piFHdpmmnKTO3523RkzpJ069Xpb0AyauLE2gwtRlNH6AhyhftSmnW1AbfGnlwDEu7m-_pRGOLj09wsvwAWjfFbmq1RKFyzGrtzxFNo5T_OWTmfGYXWf_YScTKOUjoVCilhafJ1r1MKPp8bzgY9y0W00" /></td>\n<td valign="top"><pre>tests.modules.factorial.factorial_recursive.puml</pre>\n<img src="https://www.plantuml.com/plantuml/svg/xP31QYf144Nt_HM5Mz5nv3qJ90JHHNP1oD90AAThjB6dIgghWu8Vdu2OI8o8PEkkwNkuzr2ZPAYMcmX6oLAt4PyZfMwDbOa6ZD-lDwKgQmhlvD8gy1eL6nZBPehU1rv0sJlwdw9QgC8QsGxv_wFuMOp6MAqMAfdzHA8eJ4GvXRZwYObwqZto4eWPtJ9uWbh4vh9nRYQTHsYTqN_bN_nRZiK8D2oMDeGOc63Wt7KLSFKejDlxtKZrORRitLHkAdzIKRAi3ELfUEzskzqNq3y5FXkFYS55el_l8bBsU-UPsKEdS-KbXd1tfj7L8aOAJyIaQEHXleMYM6-zLAPOKL6u4R7FJNGV" /></td>\n</tr>\n</tbody>\n</table>\n\n## Installation\n\nUse your favorite dependency manager to install `pydoctrace`:\n\n```sh\n# using pip\npip install pydoctrace\n\n# using poetry\npoetry add pydoctrace\n\n# using pipenv\npipenv install pydoctrace\n```\n\n## Purposes and mechanisms\n\nThe purpose of `pydoctrace` is to document the execution of some code to illustrate the behavior and the structure of the code base.\n\n- the documentation produced is a sequence diagram;\nwhich lets you see how the functions are called, how the values are returned and how the errors are handled\n- with one of the provided decorators (depending on the export format you want), decorate the function whose execution you want to document\n- run your code, when the execution hits the decorated function, the execution is traced and the sequence diagram will be drawn in the format of your choice\n\n`pydoctrace` is a pure Python tool relying on no other 3rd-party library to work.\nThe project involves development libraries for testing and documentation purposes.\n\n### Doc-tracing\n\nThis approach, which I called "doc-tracing" (tracing code execution for documentation purposes), is meant to be complementary of other approaches which generate documentation from static code analysis.\nStatic code analysis reads the source code to detect and document data structures (classes, dataclasses, named tuples, enumeration, etc.), functions names and signatures (parameters name and types, returned value types).\n\nUseful as it is, static code analysis does not help much to understand how the code pieces work together; doc-tracing attempts to complement this approach by producing documentation while the code runs.\nSome use cases:\n\n- you start working on a legacy codebase: study the behavior of a particular function by temporarily tracing its executions\n- you finished a user story, document its implementation by tracing the execution of some **integration tests** (*"given ... when ... then ..."*) to illustrate how right cases and errors are handled.\n- generally, the sequence diagrams illustrate how the modules and functions interacts; and as such, **they help discussing architecture**\n- tracing code execution can also be useful when teaching computer programming to illustrate how algorithms work\n\n\n### How is the code execution traced?\n\nWhen a function decorated by `pydoctrace` is called:\n\n1. a context manager is created\n2. during which a **tracing function** is passed to [sys.settrace](https://docs.python.org/3/library/sys.html#sys.settrace), which is called when different events happens in the execution stack:\n    - when functions are called\n    - when values are returned\n    - when exceptions are raised or handled\n3. the sequence diagram is drawn and exported in a file alongside the code execution so that its memory footprint is minimal\n4. once the decorated function stops its execution, the tracing function is removed from the code execution\n\n⚠️ **Caveat**: `pydoctrace` uses the `sys.settrace` API, which is meant to be used by debuggers.\nTherefore, a warning is emitted when `pydoctrace` is used in a debug mode (and does not trace the decorated function anymore).\n\n# Tests\n\n```sh\n# directly with poetry\npoetry run pytest -v\n\n# in an activated virtual environment\npytest -v\n```\n\nCode coverage (with [missed branch statements](https://pytest-cov.readthedocs.io/en/latest/config.html?highlight=--cov-branch)):\n\n```sh\npoetry run pytest -v --cov=pydoctrace --cov-branch --cov-report term-missing --cov-fail-under 50\n```\n\n# Changelog\n\n* `0.1.0`: ✨ first release, PlantUML exporter; diagram files are saved in the current working directory\n\n# Licence\n\nUnless stated otherwise all works are licensed under the [MIT license](http://spdx.org/licenses/MIT.html), a copy of which is included [here](LICENSE).\n\n# Contributions\n\n* [Luc Sorel-Giffo](https://github.com/lucsorel)\n\n## Pull requests\n\nPull-requests are welcome and will be processed on a best-effort basis.\n\nPull requests must follow the guidelines enforced by the `pre-commit` hooks:\n\n- commit messages must follow the Angular conventions enforced by the `commitlint` hook\n- code formatting must follow the conventions enforced by the `isort` and `yapf` hooks\n- code linting should not detect code smells in your contributions, this is checked by the `ruff` hook\n\n## Code conventions\n\nThe code conventions are described and enforced by [pre-commit hooks](https://pre-commit.com/hooks.html) to maintain consistency across the code base.\nThe hooks are declared in the [.pre-commit-config.yaml](.pre-commit-config.yaml) file.\n\nSet the git hooks (pre-commit and commit-msg types):\n\n```sh\npoetry run pre-commit install --hook-type pre-commit --hook-type commit-msg\n```\n\nBefore committing, you can check your changes with:\n\n```sh\n# put all your changes in the git staging area\ngit add -A\n\n# all hooks\npoetry run pre-commit run --all-files\n\n# a specific hook\npoetry run pre-commit run ruff --all-files\n```\n\n### Commit messages\n\nPlease, follow the [conventions of the Angular team](https://github.com/angular/angular/blob/main/CONTRIBUTING.md#-commit-message-format) for commit messages.\nWhen merging your pull-request, the new version of the project will be derived from the messages.\n\n### Code formatting\n\nThis project uses `isort` and `yapf` to format the code.\nThe guidelines are expressed in their respective sections in the [pyproject.toml](pyproject.toml) file.\n\n### Best practices\n\nThis project uses the `ruff` linter, which is configured in its section in the [pyproject.toml](pyproject.toml) file.\n\n# Similar tools and bibliography\n\n- https://stackoverflow.com/questions/45238329/it-is-possible-to-generate-sequence-diagram-from-python-code\n- https://github.com/gaogaotiantian/viztracer\n- https://9to5answer.com/how-to-generate-a-sequence-diagram-from-java-source-code\n- https://medium.com/javarevisited/how-to-generate-sequence-diagrams-in-intellij-e2bb7cec2b0b\n',
-    'author': 'Luc Sorel-Giffo',
-    'author_email': 'None',
-    'maintainer': 'Luc Sorel-Giffo',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/lucsorel/pydoctrace',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
-}
+# pydoctrace
 
+Generate sequence diagrams by tracing Python code execution.
+
+Here are the sequence diagrams produced by 2 different implementations of the `factorial` function (*n * n-1 * n-2 * ... * 1*).
+One which loops, another one that is recursive:
+
+<table>
+<tbody>
+<tr>
+<td valign="bottom">
+
+```python
+from pydoctrace.doctrace import trace_to_puml
+
+@trace_to_puml
+def factorial_reduce_multiply(value: int) -> int:
+    if value <= 1:
+        return value
+
+    def multiply(agg: int, value: int) -> int:
+        return agg * value
+
+    return reduce(multiply, range(1, value + 1), 1)
+```
+
+</td>
+<td valign="bottom">
+
+```python
+from pydoctrace.doctrace import trace_to_puml
+
+@trace_to_puml
+def factorial_recursive(value: int) -> int:
+    if value <= 1:
+        return value
+
+    return value * factorial_recursive(value - 1)
+```
+
+</td>
+</tr>
+<tr>
+<td valign="top"><code>tests.modules.factorial.factorial_reduce_multiply.puml</code><br />
+<img src="https://www.plantuml.com/plantuml/svg/rP0nYof148Jp_XMDgUYweZwHnqCqUDaXNEY1Z3kzEZZRlVJsW88__WAvKmurCBhDXgcYwgkUD-RKKXNHgB6cNubFaPf-wGeJ3IvUNnibdmhQL2bQgEC9caFWsgchS277bVC-y0xpmSt_ogc58jIExKiVtyXlOhHmnM6dajWl9OhYKfIR40y_RQAUz69v3yJiO1yyOIbYMpa2hANt3piFHdpmmnKTO3523RkzpJ069Xpb0AyauLE2gwtRlNH6AhyhftSmnW1AbfGnlwDEu7m-_pRGOLj09wsvwAWjfFbmq1RKFyzGrtzxFNo5T_OWTmfGYXWf_YScTKOUjoVCilhafJ1r1MKPp8bzgY9y0W00" /></td>
+<td valign="top"><code>tests.modules.factorial.factorial_recursive.puml</code><br />
+<img src="https://www.plantuml.com/plantuml/svg/xP31QYf144Nt_HM5Mz5nv3qJ90JHHNP1oD90AAThjB6dIgghWu8Vdu2OI8o8PEkkwNkuzr2ZPAYMcmX6oLAt4PyZfMwDbOa6ZD-lDwKgQmhlvD8gy1eL6nZBPehU1rv0sJlwdw9QgC8QsGxv_wFuMOp6MAqMAfdzHA8eJ4GvXRZwYObwqZto4eWPtJ9uWbh4vh9nRYQTHsYTqN_bN_nRZiK8D2oMDeGOc63Wt7KLSFKejDlxtKZrORRitLHkAdzIKRAi3ELfUEzskzqNq3y5FXkFYS55el_l8bBsU-UPsKEdS-KbXd1tfj7L8aOAJyIaQEHXleMYM6-zLAPOKL6u4R7FJNGV" /></td>
+</tr>
+</tbody>
+</table>
+
+## Installation
+
+Use your favorite dependency manager to install `pydoctrace`:
+
+```sh
+# using pip
+pip install pydoctrace
+
+# using poetry
+poetry add pydoctrace
+
+# using pipenv
+pipenv install pydoctrace
+```
+
+## Purposes and mechanisms
+
+The purpose of `pydoctrace` is to document the execution of some code to illustrate the behavior and the structure of the code base.
+
+- the documentation produced is a sequence diagram;
+which lets you see how the functions are called, how the values are returned and how the errors are handled
+- with one of the provided decorators (depending on the export format you want), decorate the function whose execution you want to document
+- run your code, when the execution hits the decorated function, the execution is traced and the sequence diagram will be drawn in the format of your choice
+
+`pydoctrace` is a pure Python tool relying on no other 3rd-party library to work.
+The project involves development libraries for testing and documentation purposes.
+
+### Doc-tracing
+
+This approach, which I called "doc-tracing" (tracing code execution for documentation purposes), is meant to be complementary of other approaches which generate documentation from static code analysis.
+Static code analysis reads the source code to detect and document data structures (classes, dataclasses, named tuples, enumeration, etc.), functions names and signatures (parameters name and types, returned value types).
+
+Useful as it is, static code analysis does not help much to understand how the code pieces work together; doc-tracing attempts to complement this approach by producing documentation while the code runs.
+Some use cases:
+
+- you start working on a legacy codebase: study the behavior of a particular function by temporarily tracing its executions
+- you finished a user story, document its implementation by tracing the execution of some **integration tests** (*"given ... when ... then ..."*) to illustrate how right cases and errors are handled.
+- generally, the sequence diagrams illustrate how the modules and functions interacts; and as such, **they help discussing architecture**
+- tracing code execution can also be useful when teaching computer programming to illustrate how algorithms work
+
+
+### How is the code execution traced?
+
+When a function decorated by `pydoctrace` is called:
+
+1. a context manager is created
+2. during which a **tracing function** is passed to [sys.settrace](https://docs.python.org/3/library/sys.html#sys.settrace), which is called when different events happens in the execution stack:
+    - when functions are called
+    - when values are returned
+    - when exceptions are raised or handled
+3. the sequence diagram is drawn and exported in a file alongside the code execution so that its memory footprint is minimal
+4. once the decorated function stops its execution, the tracing function is removed from the code execution
+
+⚠️ **Caveat**: `pydoctrace` uses the `sys.settrace` API, which is meant to be used by debuggers.
+Therefore, a warning is emitted when `pydoctrace` is used in a debug mode (and does not trace the decorated function anymore).
+
+# Tests
+
+```sh
+# directly with poetry
+poetry run pytest -v
+
+# in an activated virtual environment
+pytest -v
+```
+
+Code coverage (with [missed branch statements](https://pytest-cov.readthedocs.io/en/latest/config.html?highlight=--cov-branch)):
+
+```sh
+poetry run pytest -v --cov=pydoctrace --cov-branch --cov-report term-missing --cov-fail-under 50
+```
+
+# Changelog
+
+* `0.1.2`: added github actions for the automated tests and interaction with pre-commit.ci for the code linting
+* `0.1.1`: [deleted release] added github actions for the automated tests and interaction with pre-commit.ci for the code linting
+* `0.1.0`: ✨ first release, PlantUML exporter; diagram files are saved in the current working directory
+
+# Licence
+
+Unless stated otherwise all works are licensed under the [MIT license](http://spdx.org/licenses/MIT.html), a copy of which is included [here](LICENSE).
+
+# Contributions
+
+* [Luc Sorel-Giffo](https://github.com/lucsorel)
+
+## Pull requests
+
+Pull-requests are welcome and will be processed on a best-effort basis.
+
+Pull requests must follow the guidelines enforced by the `pre-commit` hooks:
+
+- commit messages must follow the Angular conventions enforced by the `commitlint` hook
+- code formatting must follow the conventions enforced by the `isort` and `yapf` hooks
+- code linting should not detect code smells in your contributions, this is checked by the `ruff` hook
+
+## Code conventions
+
+The code conventions are described and enforced by [pre-commit hooks](https://pre-commit.com/hooks.html) to maintain consistency across the code base.
+The hooks are declared in the [.pre-commit-config.yaml](.pre-commit-config.yaml) file.
+
+Set the git hooks (pre-commit and commit-msg types):
+
+```sh
+poetry run pre-commit install --hook-type pre-commit --hook-type commit-msg
+```
+
+Before committing, you can check your changes with:
+
+```sh
+# put all your changes in the git staging area
+git add -A
+
+# all hooks
+poetry run pre-commit run --all-files
+
+# a specific hook
+poetry run pre-commit run ruff --all-files
+```
+
+### Commit messages
+
+Please, follow the [conventions of the Angular team](https://github.com/angular/angular/blob/main/CONTRIBUTING.md#-commit-message-format) for commit messages.
+When merging your pull-request, the new version of the project will be derived from the messages.
+
+### Code formatting
+
+This project uses `isort` and `yapf` to format the code.
+The guidelines are expressed in their respective sections in the [pyproject.toml](pyproject.toml) file.
+
+### Best practices
+
+This project uses the `ruff` linter, which is configured in its section in the [pyproject.toml](pyproject.toml) file.
+
+# Similar tools and bibliography
+
+- https://stackoverflow.com/questions/45238329/it-is-possible-to-generate-sequence-diagram-from-python-code
+- https://github.com/gaogaotiantian/viztracer
+- https://9to5answer.com/how-to-generate-a-sequence-diagram-from-java-source-code
+- https://medium.com/javarevisited/how-to-generate-sequence-diagrams-in-intellij-e2bb7cec2b0b
 
-setup(**setup_kwargs)
```

