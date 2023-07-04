# Comparing `tmp/pytest_codspeed-1.2.2.tar.gz` & `tmp/pytest_codspeed-2.0.0.tar.gz`

## Comparing `pytest_codspeed-1.2.2.tar` & `pytest_codspeed-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytest_codspeed-1.2.2/src/pytest_codspeed/__init__.py
--rw-r--r--   0        0        0     7126 2020-02-02 00:00:00.000000 pytest_codspeed-1.2.2/src/pytest_codspeed/plugin.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pytest_codspeed-1.2.2/src/pytest_codspeed/_wrapper/.gitignore
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 pytest_codspeed-1.2.2/src/pytest_codspeed/_wrapper/__init__.py
--rw-r--r--   0        0        0    26531 2020-02-02 00:00:00.000000 pytest_codspeed-1.2.2/src/pytest_codspeed/_wrapper/dist_callgrind_wrapper.c
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 pytest_codspeed-1.2.2/src/pytest_codspeed/_wrapper/wrapper.c
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pytest_codspeed-1.2.2/src/pytest_codspeed/_wrapper/wrapper.h
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pytest_codspeed-1.2.2/src/pytest_codspeed/_wrapper/wrapper.pyi
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 pytest_codspeed-1.2.2/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pytest_codspeed-1.2.2/LICENSE
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 pytest_codspeed-1.2.2/README.md
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 pytest_codspeed-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 pytest_codspeed-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/src/pytest_codspeed/__init__.py
+-rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/src/pytest_codspeed/plugin.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/src/pytest_codspeed/_wrapper/.gitignore
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/src/pytest_codspeed/_wrapper/__init__.py
+-rw-r--r--   0        0        0    26531 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/src/pytest_codspeed/_wrapper/dist_callgrind_wrapper.c
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/src/pytest_codspeed/_wrapper/wrapper.c
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/src/pytest_codspeed/_wrapper/wrapper.h
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/src/pytest_codspeed/_wrapper/wrapper.pyi
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/README.md
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/PKG-INFO
```

### Comparing `pytest_codspeed-1.2.2/src/pytest_codspeed/plugin.py` & `pytest_codspeed-2.0.0/src/pytest_codspeed/plugin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import gc
 import os
 import pkgutil
+import sys
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any, Callable, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 import pytest
 from _pytest.fixtures import FixtureManager
 
 from . import __version__
 from ._wrapper import get_lib
 
 if TYPE_CHECKING:
     from ._wrapper import LibType
 
 IS_PYTEST_BENCHMARK_INSTALLED = pkgutil.find_loader("pytest_benchmark") is not None
+SUPPORTS_PERF_TRAMPOLINE = sys.version_info >= (3, 12)
 
 
 @pytest.hookimpl(trylast=True)
 def pytest_addoption(parser: "pytest.Parser"):
     group = parser.getgroup("CodSpeed benchmarking")
     group.addoption(
         "--codspeed",
@@ -90,15 +92,18 @@
             fixture_manager._arg2fixturedefs["benchmark"] = list(
                 codspeed_benchmark_fixtures
             )
 
 
 @pytest.hookimpl(trylast=True)
 def pytest_report_header(config: "pytest.Config"):
-    out = [f"codspeed: {__version__}"]
+    out = [
+        f"codspeed: {__version__} "
+        f"(callgraph: {'enabled' if SUPPORTS_PERF_TRAMPOLINE  else 'not supported'})"
+    ]
     plugin = get_plugin(config)
     if plugin.is_codspeed_enabled and not plugin.should_measure:
         out.append(
             "\033[1m"
             "NOTICE: codspeed is enabled, but no performance measurement"
             " will be made since it's running in an unknown environment."
             "\033[0m"
@@ -107,27 +112,37 @@
         out.append(
             "\033[93mCodSpeed had to disable the following plugins: "
             f"{', '.join(plugin.disabled_plugins)}\033[0m"
         )
     return "\n".join(out)
 
 
-def should_benchmark_item(item: "pytest.Item") -> bool:
+def has_benchmark_fixture(item: "pytest.Item") -> bool:
+    item_fixtures = getattr(item, "fixturenames", [])
+    return "benchmark" in item_fixtures or "codspeed_benchmark" in item_fixtures
+
+
+def has_benchmark_marker(item: "pytest.Item") -> bool:
     return (
         item.get_closest_marker("codspeed_benchmark") is not None
         or item.get_closest_marker("benchmark") is not None
-        or "benchmark" in getattr(item, "fixturenames", [])
     )
 
 
+def should_benchmark_item(item: "pytest.Item") -> bool:
+    return has_benchmark_fixture(item) or has_benchmark_marker(item)
+
+
 @pytest.hookimpl()
 def pytest_sessionstart(session: "pytest.Session"):
     plugin = get_plugin(session.config)
     if plugin.is_codspeed_enabled:
         plugin.benchmark_count = 0
+        if plugin.should_measure and SUPPORTS_PERF_TRAMPOLINE:
+            sys.activate_stack_trampoline("perf")  # type: ignore
 
 
 @pytest.hookimpl(trylast=True)
 def pytest_collection_modifyitems(
     session: "pytest.Session", config: "pytest.Config", items: "List[pytest.Item]"
 ):
     plugin = get_plugin(config)
@@ -146,70 +161,115 @@
 def _run_with_instrumentation(
     lib: "LibType", nodeId: str, fn: Callable[..., Any], *args, **kwargs
 ):
     is_gc_enabled = gc.isenabled()
     if is_gc_enabled:
         gc.collect()
         gc.disable()
+
+    def __codspeed_root_frame__():
+        fn(*args, **kwargs)
+
+    if SUPPORTS_PERF_TRAMPOLINE:
+        # Warmup CPython performance map cache
+        __codspeed_root_frame__()
+
     lib.zero_stats()
     lib.start_instrumentation()
-    fn(*args, **kwargs)
+    __codspeed_root_frame__()
     lib.stop_instrumentation()
     lib.dump_stats_at(f"{nodeId}".encode("ascii"))
     if is_gc_enabled:
         gc.enable()
 
 
-@pytest.hookimpl(trylast=True)
-def pytest_runtest_call(item: "pytest.Item"):
+@pytest.hookimpl(tryfirst=True)
+def pytest_runtest_protocol(item: "pytest.Item", nextitem: Union["pytest.Item", None]):
     plugin = get_plugin(item.config)
-
     if not plugin.is_codspeed_enabled or not should_benchmark_item(item):
-        return  # Avoid running the test multiple times when codspeed is disabled
-    else:
-        plugin.benchmark_count += 1
-        if "benchmark" in getattr(item, "fixturenames", []):
-            # This is a benchmark fixture, so the measurement is done by the fixture
-            item.runtest()
-        elif not plugin.should_measure:
-            item.runtest()
-        else:
-            assert plugin.lib is not None
-            _run_with_instrumentation(plugin.lib, item.nodeid, item.runtest)
+        return (
+            None  # Defer to the default test protocol since no benchmarking is needed
+        )
 
+    if has_benchmark_fixture(item):
+        return None  # Instrumentation is handled by the fixture
 
-@pytest.hookimpl()
-def pytest_sessionfinish(session: "pytest.Session", exitstatus):
-    plugin = get_plugin(session.config)
-    if plugin.is_codspeed_enabled:
-        reporter = session.config.pluginmanager.get_plugin("terminalreporter")
-        count_suffix = "benchmarked" if plugin.should_measure else "benchmark tested"
-        reporter.write_sep(
-            "=",
-            f"{plugin.benchmark_count} {count_suffix}",
+    plugin.benchmark_count += 1
+    if not plugin.should_measure:
+        return None  # Benchmark counted but will be run in the default protocol
+
+    # Setup phase
+    reports = []
+    ihook = item.ihook
+    ihook.pytest_runtest_logstart(nodeid=item.nodeid, location=item.location)
+    setup_call = pytest.CallInfo.from_call(
+        lambda: ihook.pytest_runtest_setup(item=item, nextitem=nextitem), "setup"
+    )
+    setup_report = ihook.pytest_runtest_makereport(item=item, call=setup_call)
+    ihook.pytest_runtest_logreport(report=setup_report)
+    reports.append(setup_report)
+    # Run phase
+    if setup_report.passed and not item.config.getoption("setuponly"):
+        assert plugin.lib is not None
+        runtest_call = pytest.CallInfo.from_call(
+            lambda: _run_with_instrumentation(plugin.lib, item.nodeid, item.runtest),
+            "call",
         )
+        runtest_report = ihook.pytest_runtest_makereport(item=item, call=runtest_call)
+        ihook.pytest_runtest_logreport(report=runtest_report)
+        reports.append(runtest_report)
+
+    # Teardown phase
+    teardown_call = pytest.CallInfo.from_call(
+        lambda: ihook.pytest_runtest_teardown(item=item, nextitem=nextitem), "teardown"
+    )
+    teardown_report = ihook.pytest_runtest_makereport(item=item, call=teardown_call)
+    ihook.pytest_runtest_logreport(report=teardown_report)
+    reports.append(teardown_report)
+    ihook.pytest_runtest_logfinish(nodeid=item.nodeid, location=item.location)
 
+    return reports  # Deny further protocol hooks execution
 
-@pytest.fixture(scope="function")
-def codspeed_benchmark(request: "pytest.FixtureRequest") -> Callable:
-    plugin = get_plugin(request.config)
 
-    def run(func: Callable[..., Any], *args: Any, **kwargs: Any) -> Any:
+class BenchmarkFixture:
+    def __init__(self, request: "pytest.FixtureRequest"):
+        self.extra_info: Dict = {}
+
+        self._request = request
+
+    def __call__(self, func: Callable[..., Any], *args: Any, **kwargs: Any) -> Any:
+        plugin = get_plugin(self._request.config)
+        plugin.benchmark_count += 1
         if plugin.is_codspeed_enabled and plugin.should_measure:
             assert plugin.lib is not None
             _run_with_instrumentation(
-                plugin.lib, request.node.nodeid, func, *args, **kwargs
+                plugin.lib, self._request.node.nodeid, func, *args, **kwargs
             )
         else:
             func(*args, **kwargs)
 
-    return run
+
+@pytest.fixture(scope="function")
+def codspeed_benchmark(request: "pytest.FixtureRequest") -> Callable:
+    return BenchmarkFixture(request)
 
 
 if not IS_PYTEST_BENCHMARK_INSTALLED:
 
     @pytest.fixture(scope="function")
     def benchmark(codspeed_benchmark, request: "pytest.FixtureRequest"):
         """
         Compatibility with pytest-benchmark
         """
         return codspeed_benchmark
+
+
+@pytest.hookimpl()
+def pytest_sessionfinish(session: "pytest.Session", exitstatus):
+    plugin = get_plugin(session.config)
+    if plugin.is_codspeed_enabled:
+        reporter = session.config.pluginmanager.get_plugin("terminalreporter")
+        count_suffix = "benchmarked" if plugin.should_measure else "benchmark tested"
+        reporter.write_sep(
+            "=",
+            f"{plugin.benchmark_count} {count_suffix}",
+        )
```

### Comparing `pytest_codspeed-1.2.2/src/pytest_codspeed/_wrapper/__init__.py` & `pytest_codspeed-2.0.0/src/pytest_codspeed/_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_codspeed-1.2.2/src/pytest_codspeed/_wrapper/dist_callgrind_wrapper.c` & `pytest_codspeed-2.0.0/src/pytest_codspeed/_wrapper/dist_callgrind_wrapper.c`

 * *Files identical despite different names*

### Comparing `pytest_codspeed-1.2.2/.gitignore` & `pytest_codspeed-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_codspeed-1.2.2/LICENSE` & `pytest_codspeed-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_codspeed-1.2.2/README.md` & `pytest_codspeed-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 <div align="center">
 <h1>pytest-codspeed</h1>
 
 [![CI](https://github.com/CodSpeedHQ/pytest-codspeed/actions/workflows/ci.yml/badge.svg)](https://github.com/CodSpeedHQ/pytest-codspeed/actions/workflows/ci.yml)
 <a href="https://pypi.org/project/pytest-codspeed" target="_blank">
 <img src="https://img.shields.io/pypi/v/pytest-codspeed?color=%2334D058&label=pypi" alt="Package version">
 </a>
-<img src="https://img.shields.io/badge/python-3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11-informational.svg" alt="python-3.7-3.8-3.9-3.10-3.11">
+<img src="https://img.shields.io/badge/python-3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12-informational.svg" alt="python-3.7-3.8-3.9-3.10-3.11-3.12">
+[![Discord](https://img.shields.io/badge/chat%20on-discord-7289da.svg)](https://discord.com/invite/MxpaCfKSqF)
 
 Pytest plugin to create CodSpeed benchmarks
 
 </div>
 
 ## Requirements
```

### Comparing `pytest_codspeed-1.2.2/pyproject.toml` & `pytest_codspeed-2.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -24,54 +24,70 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Testing",
     "Topic :: System :: Benchmark",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
-dependencies = ["cffi ~= 1.15.1", "pytest>=3.8"]
+dependencies = [
+    "cffi ~= 1.15.1",
+    "pytest>=3.8",
+    "setuptools ~= 67.8.0; python_version >= '3.12'", # FIXME: remove when cffi supports directly python 3.12
+]
 
 [project.optional-dependencies]
-dev = [
-    "hatchling ~= 1.11.1",
-    "black ~= 22.3.0",
-    "isort ~=5.8.0",
-    "flake8 ~= 5.0.4",
-    "mypy ~= 0.961",
-    "pytest ~= 7.0",
-    "pytest-cov ~= 4.0.0",
-    "ruff ~= 0.0.100",
-]
-compatibility = ["pytest-benchmarks ~= 3.4.1"]
+lint = ["black ~= 23.3.0", "isort ~=5.12.0", "mypy ~= 1.3.0", "ruff ~= 0.0.275"]
+compat = ["pytest-benchmark ~= 4.0.0"]
+test = ["pytest ~= 7.0", "pytest-cov ~= 4.0.0"]
 
 [project.entry-points]
 pytest11 = { codspeed = "pytest_codspeed.plugin" }
 
+[tool.hatch.envs.default]
+python = "3.12"
+features = ["lint", "test", "compat"]
+
+[tool.hatch.envs.test]
+features = ["test"]
+
+[[tool.hatch.envs.test.matrix]]
+python = ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
+features = ["compat", "test"]
+
 [tool.hatch.version]
 path = "src/pytest_codspeed/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = ["/src"]
 
+[tool.mypy]
+python_version = "3.12"
+
 [tool.ruff]
 line-length = 88
+select = ["E", "F", "I", "C"]
 
 [tool.isort]
 line_length = 88
 multi_line_output = 3
 include_trailing_comma = true
 use_parentheses = true
 force_grid_wrap = 0
 float_to_top = true
 
+[tool.pytest.ini_options]
+addopts = "--ignore=tests/benchmarks --ignore=tests/examples"
+filterwarnings = ["ignore::DeprecationWarning:pytest_benchmark.utils.*:"]
+
 [tool.coverage.run]
 branch = true
 [tool.coverage.report]
 include = ["src/*", "tests/*"]
 omit = ["**/conftest.py"]
 exclude_lines = [
     "pragma: no cover",
```

### Comparing `pytest_codspeed-1.2.2/PKG-INFO` & `pytest_codspeed-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-codspeed
-Version: 1.2.2
+Version: 2.0.0
 Summary: Pytest plugin to create CodSpeed benchmarks
 Project-URL: Homepage, https://codspeed.io/
 Project-URL: Documentation, https://docs.codspeed.io/
 Project-URL: Source, https://github.com/CodSpeedHQ/pytest-codspeed
 Author-email: Arthur Pastel <arthur@codspeed.io>
 License: The MIT License (MIT)
         
@@ -36,42 +36,44 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Benchmark
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: cffi~=1.15.1
 Requires-Dist: pytest>=3.8
-Provides-Extra: compatibility
-Requires-Dist: pytest-benchmarks~=3.4.1; extra == 'compatibility'
-Provides-Extra: dev
-Requires-Dist: black~=22.3.0; extra == 'dev'
-Requires-Dist: flake8~=5.0.4; extra == 'dev'
-Requires-Dist: hatchling~=1.11.1; extra == 'dev'
-Requires-Dist: isort~=5.8.0; extra == 'dev'
-Requires-Dist: mypy~=0.961; extra == 'dev'
-Requires-Dist: pytest-cov~=4.0.0; extra == 'dev'
-Requires-Dist: pytest~=7.0; extra == 'dev'
-Requires-Dist: ruff~=0.0.100; extra == 'dev'
+Requires-Dist: setuptools~=67.8.0; python_version >= '3.12'
+Provides-Extra: compat
+Requires-Dist: pytest-benchmark~=4.0.0; extra == 'compat'
+Provides-Extra: lint
+Requires-Dist: black~=23.3.0; extra == 'lint'
+Requires-Dist: isort~=5.12.0; extra == 'lint'
+Requires-Dist: mypy~=1.3.0; extra == 'lint'
+Requires-Dist: ruff~=0.0.275; extra == 'lint'
+Provides-Extra: test
+Requires-Dist: pytest-cov~=4.0.0; extra == 'test'
+Requires-Dist: pytest~=7.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 <div align="center">
 <h1>pytest-codspeed</h1>
 
 [![CI](https://github.com/CodSpeedHQ/pytest-codspeed/actions/workflows/ci.yml/badge.svg)](https://github.com/CodSpeedHQ/pytest-codspeed/actions/workflows/ci.yml)
 <a href="https://pypi.org/project/pytest-codspeed" target="_blank">
 <img src="https://img.shields.io/pypi/v/pytest-codspeed?color=%2334D058&label=pypi" alt="Package version">
 </a>
-<img src="https://img.shields.io/badge/python-3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11-informational.svg" alt="python-3.7-3.8-3.9-3.10-3.11">
+<img src="https://img.shields.io/badge/python-3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12-informational.svg" alt="python-3.7-3.8-3.9-3.10-3.11-3.12">
+[![Discord](https://img.shields.io/badge/chat%20on-discord-7289da.svg)](https://discord.com/invite/MxpaCfKSqF)
 
 Pytest plugin to create CodSpeed benchmarks
 
 </div>
 
 ## Requirements
```

