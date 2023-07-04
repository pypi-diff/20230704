# Comparing `tmp/stamina-22.2.0.tar.gz` & `tmp/stamina-23.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Tue Jul  4 09:09:03 2023, max compression
```

## Comparing `stamina-22.2.0.tar` & `stamina-23.1.0.tar`

### file list

```diff
@@ -1,24 +1,39 @@
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 stamina-22.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 stamina-22.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 stamina-22.2.0/README.md
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 stamina-22.2.0/noxfile.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 stamina-22.2.0/typing_examples.py
--rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 stamina-22.2.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 stamina-22.2.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 stamina-22.2.0/.github/SECURITY.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 stamina-22.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 stamina-22.2.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 stamina-22.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 stamina-22.2.0/src/stamina/__init__.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 stamina-22.2.0/src/stamina/_config.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 stamina-22.2.0/src/stamina/_instrumentation.py
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 stamina-22.2.0/src/stamina/_sync.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stamina-22.2.0/src/stamina/py.typed
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 stamina-22.2.0/src/stamina/typing.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 stamina-22.2.0/tests/conftest.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 stamina-22.2.0/tests/test_config.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 stamina-22.2.0/tests/test_sync.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 stamina-22.2.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 stamina-22.2.0/LICENSE
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 stamina-22.2.0/pyproject.toml
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 stamina-22.2.0/PKG-INFO
+-rw-r--r--   0        0        0      579 2023-07-04 09:09:03.000000 stamina-23.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2023-07-04 09:09:03.000000 stamina-23.1.0/.python-version-default
+-rw-r--r--   0        0        0      221 2023-07-04 09:09:03.000000 stamina-23.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1881 2023-07-04 09:09:03.000000 stamina-23.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2311 2023-07-04 09:09:03.000000 stamina-23.1.0/README.md
+-rw-r--r--   0        0        0     3099 2023-07-04 09:09:03.000000 stamina-23.1.0/noxfile.py
+-rw-r--r--   0        0        0     5482 2023-07-04 09:09:03.000000 stamina-23.1.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     5974 2023-07-04 09:09:03.000000 stamina-23.1.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       18 2023-07-04 09:09:03.000000 stamina-23.1.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      865 2023-07-04 09:09:03.000000 stamina-23.1.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2023-07-04 09:09:03.000000 stamina-23.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     5644 2023-07-04 09:09:03.000000 stamina-23.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      749 2023-07-04 09:09:03.000000 stamina-23.1.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1610 2023-07-04 09:09:03.000000 stamina-23.1.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0        0        0      194 2023-07-04 09:09:03.000000 stamina-23.1.0/docs/api.rst
+-rw-r--r--   0        0        0       33 2023-07-04 09:09:03.000000 stamina-23.1.0/docs/changelog.md
+-rw-r--r--   0        0        0     2505 2023-07-04 09:09:03.000000 stamina-23.1.0/docs/conf.py
+-rw-r--r--   0        0        0      431 2023-07-04 09:09:03.000000 stamina-23.1.0/docs/index.md
+-rw-r--r--   0        0        0       40 2023-07-04 09:09:03.000000 stamina-23.1.0/docs/security.md
+-rw-r--r--   0        0        0     5409 2023-07-04 09:09:03.000000 stamina-23.1.0/docs/tutorial.md
+-rw-r--r--   0        0        0      573 2023-07-04 09:09:03.000000 stamina-23.1.0/src/stamina/__init__.py
+-rw-r--r--   0        0        0      822 2023-07-04 09:09:03.000000 stamina-23.1.0/src/stamina/_config.py
+-rw-r--r--   0        0        0     8654 2023-07-04 09:09:03.000000 stamina-23.1.0/src/stamina/_core.py
+-rw-r--r--   0        0        0     1621 2023-07-04 09:09:03.000000 stamina-23.1.0/src/stamina/_instrumentation.py
+-rw-r--r--   0        0        0        0 2023-07-04 09:09:03.000000 stamina-23.1.0/src/stamina/py.typed
+-rw-r--r--   0        0        0      516 2023-07-04 09:09:03.000000 stamina-23.1.0/src/stamina/typing.py
+-rw-r--r--   0        0        0        0 2023-07-04 09:09:03.000000 stamina-23.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      266 2023-07-04 09:09:03.000000 stamina-23.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     3341 2023-07-04 09:09:03.000000 stamina-23.1.0/tests/test_async.py
+-rw-r--r--   0        0        0      369 2023-07-04 09:09:03.000000 stamina-23.1.0/tests/test_config.py
+-rw-r--r--   0        0        0     1479 2023-07-04 09:09:03.000000 stamina-23.1.0/tests/test_instrumentation.py
+-rw-r--r--   0        0        0      346 2023-07-04 09:09:03.000000 stamina-23.1.0/tests/test_packaging.py
+-rw-r--r--   0        0        0     2643 2023-07-04 09:09:03.000000 stamina-23.1.0/tests/test_structlog.py
+-rw-r--r--   0        0        0     2370 2023-07-04 09:09:03.000000 stamina-23.1.0/tests/test_sync.py
+-rw-r--r--   0        0        0     2004 2023-07-04 09:09:03.000000 stamina-23.1.0/tests/typing/api.py
+-rw-r--r--   0        0        0      103 2023-07-04 09:09:03.000000 stamina-23.1.0/.gitignore
+-rw-r--r--   0        0        0     1101 2023-07-04 09:09:03.000000 stamina-23.1.0/LICENSE
+-rw-r--r--   0        0        0     4465 2023-07-04 09:09:03.000000 stamina-23.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3890 2023-07-04 09:09:03.000000 stamina-23.1.0/PKG-INFO
```

### Comparing `stamina-22.2.0/.github/CODE_OF_CONDUCT.md` & `stamina-23.1.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stamina-22.2.0/.github/workflows/codeql-analysis.yml` & `stamina-23.1.0/.github/workflows/codeql-analysis.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 name: CodeQL
 
 on:
   push:
     branches: [main]
   pull_request:
     # The branches below must be a subset of the branches above
@@ -20,15 +21,15 @@
       actions: read
       contents: read
       security-events: write
 
     strategy:
       fail-fast: false
       matrix:
-        language: ["python"]
+        language: [python]
 
     steps:
       - name: Checkout repository
         uses: actions/checkout@v3
 
       - name: Initialize CodeQL
         uses: github/codeql-action/init@v2
```

### Comparing `stamina-22.2.0/src/stamina/_config.py` & `stamina-23.1.0/src/stamina/_config.py`

 * *Files identical despite different names*

### Comparing `stamina-22.2.0/src/stamina/_instrumentation.py` & `stamina-23.1.0/src/stamina/_instrumentation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # SPDX-FileCopyrightText: 2022 Hynek Schlawack <hs@ox.cx>
 #
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
-from typing import Any
-
 
 try:
     import structlog
 
     logger = structlog.get_logger()
 except ImportError:
     logger = None
@@ -24,44 +22,44 @@
     )
 except ImportError:
     RETRY_COUNTER = None  # type: ignore[assignment]
 
 
 def count_retries(
     attempt: int,
-    backoff: float,
+    idle_for: float,
     exc: Exception,
     name: str,
-    args: Any,
-    kwargs: Any,
+    args: tuple[object, ...],
+    kwargs: dict[str, object],
 ) -> None:
     """
     Count and log retries for callable *name*.
     """
     RETRY_COUNTER.labels(
         callable=name, attempt=attempt, error_type=guess_name(exc.__class__)
     ).inc()
 
 
 def log_retries(
     attempt: int,
-    backoff: float,
+    idle_for: float,
     exc: Exception,
     name: str,
-    args: Any,
-    kwargs: Any,
+    args: tuple[object, ...],
+    kwargs: dict[str, object],
 ) -> None:
     logger.warning(
         "stamina.retry_scheduled",
         callable=name,
         attempt=attempt,
-        backoff=backoff,
+        slept=idle_for,
         error=repr(exc),
         args=tuple(repr(a) for a in args),
-        kwargs={k: v for k, v in kwargs.items()},
+        kwargs=dict(kwargs.items()),
     )
 
 
 INSTRUMENTS = []
 
 if RETRY_COUNTER:
     INSTRUMENTS.append(count_retries)
```

### Comparing `stamina-22.2.0/tests/test_sync.py` & `stamina-23.1.0/tests/test_sync.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,64 @@
 # SPDX-FileCopyrightText: 2022 Hynek Schlawack <hs@ox.cx>
 #
 # SPDX-License-Identifier: MIT
 
-from unittest.mock import Mock
+import datetime as dt
 
 import pytest
 import tenacity
 
 import stamina
 
-from stamina._sync import _make_stop
+from stamina._core import _make_stop
 
 
-@pytest.mark.parametrize("attempts,timeout", [(None, 1), (1, None)])
-def test_ok(attempts, timeout):
+@pytest.mark.parametrize("attempts", [None, 1])
+@pytest.mark.parametrize("timeout", [None, 1, dt.timedelta(days=1)])
+@pytest.mark.parametrize("duration", [1, dt.timedelta(days=1)])
+def test_ok(attempts, timeout, duration):
     """
     No error, no problem.
     """
 
-    @stamina.retry(on=Exception, attempts=attempts, timeout=timeout)
+    @stamina.retry(
+        on=Exception,
+        attempts=attempts,
+        timeout=timeout,
+        wait_initial=duration,
+        wait_max=duration,
+        wait_jitter=duration,
+    )
     def f():
         return 42
 
     assert 42 == f()
 
 
-def test_retries():
+@pytest.mark.parametrize(
+    "timeout",
+    [None, 1, dt.timedelta(days=1)],
+)
+@pytest.mark.parametrize("duration", [0, dt.timedelta(days=0)])
+def test_retries(duration, timeout):
     """
     Retries if the specific error is raised.
     """
     i = 0
 
-    @stamina.retry(on=ValueError, wait_max=0)
+    @stamina.retry(
+        on=ValueError,
+        timeout=timeout,
+        wait_max=duration,
+        wait_initial=duration,
+        wait_jitter=duration,
+    )
     def f():
         nonlocal i
-        if i == 0:
+        if i < 1:
             i += 1
             raise ValueError
 
         return 42
 
     assert 42 == f()
     assert 1 == i
@@ -53,32 +73,47 @@
     def f():
         raise TypeError("passed")
 
     with pytest.raises(TypeError, match="passed"):
         f()
 
 
-def test_retry_inactive(monkeypatch):
+def test_retry_inactive():
     """
     If inactive, don't retry.
     """
+    num_called = 0
 
     @stamina.retry(on=Exception)
     def f():
+        nonlocal num_called
+        num_called += 1
         raise Exception("passed")
 
     stamina.set_active(False)
 
-    retrying = Mock()
-    monkeypatch.setattr(stamina._sync._t, "Retrying", retrying)
-
     with pytest.raises(Exception, match="passed"):
         f()
 
-    retrying.assert_not_called()
+    assert 1 == num_called
+
+
+def test_retry_block():
+    """
+    Sync retry_context blocks are retried.
+    """
+    i = 0
+
+    for attempt in stamina.retry_context(on=ValueError, wait_max=0):
+        with attempt:
+            i += 1
+            if i < 2:
+                raise ValueError
+
+    assert 2 == i
 
 
 class TestMakeStop:
     def test_never(self):
         """
         If all conditions are None, return stop_never.
         """
```

### Comparing `stamina-22.2.0/LICENSE` & `stamina-23.1.0/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 MIT License
 
-Copyright (c) 2022 Hynek Schlawack
+Copyright (c) 2022 Hynek Schlawack and the stamina contributors
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `stamina-22.2.0/PKG-INFO` & `stamina-23.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,107 @@
 Metadata-Version: 2.1
 Name: stamina
-Version: 22.2.0
-Summary: Easy mode for Tenacity.
-Project-URL: Documentation, https://github.com/hynek/stamina#readme
+Version: 23.1.0
+Summary: Production-grade retries made easy.
+Project-URL: Documentation, https://stamina.hynek.me
 Project-URL: Source, https://github.com/hynek/stamina
 Project-URL: Changelog, https://github.com/hynek/stamina/blob/main/CHANGELOG.md
 Project-URL: Funding, https://github.com/sponsors/hynek
-Project-URL: Ko-fi, https://ko-fi.com/the_hynek
 Author-email: Hynek Schlawack <hs@ox.cx>
+License-Expression: MIT
 License-File: LICENSE
 Keywords: reliability,retries,retry,tenacity
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: tenacity
 Requires-Dist: typing-extensions; python_version < '3.10'
 Provides-Extra: dev
 Requires-Dist: nox; extra == 'dev'
+Requires-Dist: prometheus-client; extra == 'dev'
 Requires-Dist: stamina[tests,typing]; extra == 'dev'
+Requires-Dist: structlog; extra == 'dev'
+Requires-Dist: tomli; python_version < '3.11' and extra == 'dev'
+Provides-Extra: docs
+Requires-Dist: furo; extra == 'docs'
+Requires-Dist: myst-parser; extra == 'docs'
+Requires-Dist: prometheus-client; extra == 'docs'
+Requires-Dist: sphinx; extra == 'docs'
+Requires-Dist: sphinx-notfound-page; extra == 'docs'
+Requires-Dist: structlog; extra == 'docs'
 Provides-Extra: tests
 Requires-Dist: pytest; extra == 'tests'
 Requires-Dist: pytest-asyncio; extra == 'tests'
 Provides-Extra: typing
-Requires-Dist: mypy; extra == 'typing'
+Requires-Dist: mypy>=1.4; extra == 'typing'
 Description-Content-Type: text/markdown
 
-# stamina
-
-[![PyPI - Version](https://img.shields.io/pypi/v/stamina.svg)](https://pypi.org/project/stamina)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stamina.svg)](https://pypi.org/project/stamina)
-[![License: MIT](https://img.shields.io/badge/license-MIT-C06524)](https://github.com/hynek/stamina/blob/main/LICENSE)
-
+# *stamina*: Production-grade Retries Made Easy
 
 Transient failures are common in distributed systems.
-To deal with them, you need to **retry** failed operations.
-[*Tenacity*](https://tenacity.readthedocs.io/) is an *amazing* and beautifully *composable* toolkit for handling retries that I've been using it for years.
-In practice, I've found myself to use only very few knobs and wished it wouldn't erase the types of the callables that I decorate with `@tenacity.retry`.
+To make your systems resilient, you need to **retry** failed operations.
+But bad retries can make things *much worse*.
 
-*stamina* is an **opinionated** thin layer around *Tenacity* that I've been copy-pasting between my projects for a long time:
+*stamina* is an opinionated wrapper around the *great-but-unopinionated* [Tenacity](https://tenacity.readthedocs.io/) package.
+Its goal is to be as ergonomic as possible, while doing the right thing by default, while minimizing potential for misuse.
+It is the result of years of copy-pasting the same configuration over and over again:
 
 - Retry only on certain exceptions.
-- [Exponential backoff with _jitter_](https://aws.amazon.com/blogs/architecture/exponential-backoff-and-jitter/) between retries.
+- Exponential backoff with _jitter_ between retries.
 - Limit the number of retries **and** total time.
-- Preserve type hints of the decorated callable.
-- Count ([*Prometheus*](https://github.com/prometheus/client_python)) and log ([*structlog*](https://www.structlog.org/)) retries with basic metadata (if they're installed).
-- Easy deactivation for testing.
+- Automatic **async** support.
+- Preserve **type hints** of the decorated callable.
+- Count ([Prometheus](https://github.com/prometheus/client_python)) and log ([*structlog*](https://www.structlog.org/)) retries with basic metadata, if they're installed.
+- Easy _global_ deactivation for testing.
+
+For example:
+
+```python
+import httpx
+
+import stamina
+
+
+@stamina.retry(on=httpx.HTTPError, attempts=3)
+def do_it(code: int) -> httpx.Response:
+    resp = httpx.get(f"https://httpbin.org/status/{code}")
+    resp.raise_for_status()
+
+    return resp
+```
+
+**Async** callables work use the same API and it's possible to retry **arbitrary blocks**, too.
+Please refer to our [tutorial](https://stamina.hynek.me/en/latest/tutorial.html) for more examples.
+
 
 
 ## Release Information
 
 ### Added
 
-- Retries are now instrumented.
-  If [*prometheus-client*](https://github.com/prometheus/client_python) is installed, retries are counted using the *Prometheus* counter `stamina_retries_total`.
-  If [*structlog*](https://www.structlog.org/) is installed, they are logged using a *structlog* logger at warning level.
-  These two instrumentations are *independent* from each other.
+- Official Python 3.12 support.
+  [#9](https://github.com/hynek/stamina/pull/9)
+- Async support.
+  [#10](https://github.com/hynek/stamina/pull/10)
+- Retries of arbitrary blocks using (async) `for` loops and context managers.
+  [#12](https://github.com/hynek/stamina/pull/12)
+- Proper documentation.
+  [#16](https://github.com/hynek/stamina/pull/16)
+- A backwards-compatibility policy.
+
+
+### Changed
+
+- The *timeout*, *wait_initial*, *wait_max*, and *wait_jitter* arguments can now also be of type [`datetime.timedelta`](https://docs.python.org/3/library/datetime.html#datetime.timedelta).
+
+
+---
 
+[→ Full Changelog](https://github.com/hynek/stamina/blob/main/CHANGELOG.md)
 
-## License
 
-*stamina* is written by [Hynek Schlawack](https://hynek.me/) and distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

