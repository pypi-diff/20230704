# Comparing `tmp/exec-helpers-7.3.6.tar.gz` & `tmp/exec-helpers-7.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exec-helpers-7.3.6.tar", last modified: Fri Dec 16 09:37:05 2022, max compression
+gzip compressed data, was "exec-helpers-7.4.0.tar", last modified: Tue Jul  4 10:54:27 2023, max compression
```

## Comparing `exec-helpers-7.3.6.tar` & `exec-helpers-7.4.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 09:37:05.613874 exec-helpers-7.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/CI_REQUIREMENTS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11366 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      394 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17538 2022-12-16 09:37:05.613874 exec-helpers-7.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16066 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/build_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      577 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/classifiers.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 09:37:05.609873 exec-helpers-7.3.6/exec_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/_log_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    73592 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/_ssh_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17129 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/_ssh_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/_subprocess_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-16 09:37:05.000000 exec-helpers-7.3.6/exec_helpers/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    31197 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 09:37:05.609873 exec-helpers-7.3.6/exec_helpers/async_api/
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/async_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/async_api/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29978 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/async_api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/async_api/exec_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    33946 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/async_api/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    11795 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24522 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/exec_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/proc_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)    15105 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/ssh_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    34738 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/exec_helpers/subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 09:37:05.609873 exec-helpers-7.3.6/exec_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17538 2022-12-16 09:37:05.000000 exec-helpers-7.3.6/exec_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2022-12-16 09:37:05.000000 exec-helpers-7.3.6/exec_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 09:37:05.000000 exec-helpers-7.3.6/exec_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2022-12-16 09:37:05.000000 exec-helpers-7.3.6/exec_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-16 09:37:05.000000 exec-helpers-7.3.6/exec_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/flake8_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/mypy_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/pytest_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-16 09:37:05.613874 exec-helpers-7.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      836 2022-12-16 09:36:45.000000 exec-helpers-7.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:54:27.028649 exec-helpers-7.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/CI_REQUIREMENTS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11366 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17666 2023-07-04 10:54:27.028649 exec-helpers-7.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16066 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/build_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/classifiers.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:54:27.024649 exec-helpers-7.4.0/exec_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/_log_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74568 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/_ssh_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17129 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/_ssh_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/_subprocess_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-04 10:54:26.000000 exec-helpers-7.4.0/exec_helpers/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31559 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:54:27.024649 exec-helpers-7.4.0/exec_helpers/async_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/async_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/async_api/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    30041 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/async_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/async_api/exec_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33387 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/async_api/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/exec_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/proc_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/ssh_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/exec_helpers/subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:54:27.024649 exec-helpers-7.4.0/exec_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17666 2023-07-04 10:54:26.000000 exec-helpers-7.4.0/exec_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-04 10:54:27.000000 exec-helpers-7.4.0/exec_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:54:26.000000 exec-helpers-7.4.0/exec_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:54:26.000000 exec-helpers-7.4.0/exec_helpers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-04 10:54:26.000000 exec-helpers-7.4.0/exec_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 10:54:26.000000 exec-helpers-7.4.0/exec_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/flake8_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/mypy_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/pytest_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 10:54:27.028649 exec-helpers-7.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-04 10:54:08.000000 exec-helpers-7.4.0/setup.py
```

### Comparing `exec-helpers-7.3.6/.pre-commit-config.yaml` & `exec-helpers-7.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `exec-helpers-7.3.6/.readthedocs.yaml` & `exec-helpers-7.4.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `exec-helpers-7.3.6/LICENSE` & `exec-helpers-7.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exec-helpers-7.3.6/PKG-INFO` & `exec-helpers-7.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: exec-helpers
-Version: 7.3.6
+Version: 7.4.0
 Summary: Execution helpers for simplified usage of subprocess and ssh.
+Home-page: https://github.com/python-useful-helpers/exec-helpers
 Author-email: Alexey Stepanov <penguinolog@gmail.com>
-Maintainer-email: Alexey Stepanov <penguinolog@gmail.com>, Antonio Esposito <esposito.cloud@gmail.com>, Dennis Dmitriev <dis-xcom@gmail.com>
-License: Apache License, Version 2.0
-Project-URL: Bug Tracker, https://github.com/python-useful-helpers/exec-helpers/issues
+Maintainer-email: Aleksei Stepanov <penguinolog@gmail.com>, Antonio Esposito <esposito.cloud@gmail.com>, Dennis Dmitriev <dis-xcom@gmail.com>
+License: Apache-2.0
 Project-URL: Documentation, https://exec-helpers.readthedocs.io/
+Project-URL: Repository, https://github.com/python-useful-helpers/exec-helpers
+Project-URL: Bug Tracker, https://github.com/python-useful-helpers/exec-helpers/issues
 Keywords: subprocess,ssh
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `exec-helpers-7.3.6/README.rst` & `exec-helpers-7.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `exec-helpers-7.3.6/classifiers.txt` & `exec-helpers-7.4.0/classifiers.txt`

 * *Files identical despite different names*

### Comparing `exec-helpers-7.3.6/exec_helpers/__init__.py` & `exec-helpers-7.4.0/exec_helpers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2022 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 
 #         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -17,17 +17,17 @@
 from __future__ import annotations
 
 # Standard Library
 import importlib
 import typing
 import warnings
 
-try:
+try:  # noqa: SIM105
     # Local Implementation
-    from ._version import version as __version__
+    from ._version import version as __version__  # noqa: F401
 except ImportError:
     pass
 
 if typing.TYPE_CHECKING:
     # Standard Library
     from collections.abc import Sequence
 
@@ -96,30 +96,34 @@
 def __getattr__(name: str) -> typing.Any:
     """Get attributes lazy.
 
     :return: attribute by name
     :raises AttributeError: attribute is not defined for lazy load
     """
     if name in _deprecated:
-        warnings.warn(f"{name} is deprecated in favor of {_deprecated[name]}", DeprecationWarning)
+        warnings.warn(
+            f"{name} is deprecated in favor of {_deprecated[name]}",
+            DeprecationWarning,
+            stacklevel=2,
+        )
     if name in __lazy_load_modules:
         mod = importlib.import_module(f"{__package__}.{name}")
         __locals[name] = mod
         return mod
     if name in __lazy_load_parent_modules:
         mod = importlib.import_module(f"{__package__}.{__lazy_load_parent_modules[name]}")
         obj = getattr(mod, name)
         __locals[name] = obj
         return obj
     raise AttributeError(f"{name} not found in {__package__}")
 
 
-__author__ = "Alexey Stepanov"
+__author__ = "Aleksei Stepanov"
 __author_email__ = "penguinolog@gmail.com"
 __maintainers__ = {
-    "Alexey Stepanov": "penguinolog@gmail.com",
+    "Aleksei Stepanov": "penguinolog@gmail.com",
     "Antonio Esposito": "esposito.cloud@gmail.com",
     "Dennis Dmitriev": "dis-xcom@gmail.com",
 }
 __url__ = "https://github.com/python-useful-helpers/exec-helpers"
 __description__ = "Execution helpers for simplified usage of subprocess and ssh."
 __license__ = "Apache License, Version 2.0"
```

### Comparing `exec-helpers-7.3.6/exec_helpers/__init__.pyi` & `exec-helpers-7.4.0/exec_helpers/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2021 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 
 #         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -35,17 +35,17 @@
 from .exceptions import ParallelCallProcessError
 from .exec_result import ExecResult
 from .proc_enums import ExitCodes
 from .ssh import SSHClient
 from .ssh_auth import SSHAuth
 from .subprocess import Subprocess  # nosec  # Expected
 
-try:
+try:  # noqa: SIM105
     # Local Implementation
-    from ._version import version as __version__
+    from ._version import version as __version__  # noqa: F401
 except ImportError:
     pass
 
 # noinspection PyUnresolvedReferences
 __all__ = (
     # pylint: disable=undefined-all-variable
     # lazy load
```

### Comparing `exec-helpers-7.3.6/exec_helpers/_helpers.py` & `exec-helpers-7.4.0/exec_helpers/_helpers.py`

 * *Files identical despite different names*

### Comparing `exec-helpers-7.3.6/exec_helpers/_log_templates.py` & `exec-helpers-7.4.0/exec_helpers/_log_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2022 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Copyright 2017 Mirantis, Inc.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
```

### Comparing `exec-helpers-7.3.6/exec_helpers/_ssh_base.py` & `exec-helpers-7.4.0/exec_helpers/_ssh_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2022 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Copyright 2013 - 2016 Mirantis, Inc.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 
@@ -52,14 +52,17 @@
 if typing.TYPE_CHECKING:
     # Standard Library
     import socket
     from collections.abc import Iterable
     from collections.abc import Sequence
     from types import TracebackType
 
+    # External Dependencies
+    from typing_extensions import Self
+
     # Package Implementation
     from exec_helpers.api import CalledProcessErrorSubClassT
     from exec_helpers.api import CommandT
     from exec_helpers.api import ErrorInfoT
     from exec_helpers.api import ExpectedExitCodesT
     from exec_helpers.api import LogMaskReT
     from exec_helpers.api import OptionalStdinT
@@ -69,15 +72,15 @@
 __all__ = ("SSHClientBase", "SshExecuteAsyncResult", "SupportPathT")
 
 KeepAlivePeriodT = typing.Union[int, bool]
 SupportPathT = typing.Union[str, pathlib.PurePath]
 _RT = typing.TypeVar("_RT")
 
 
-class RetryOnExceptions(tenacity.retry_if_exception):  # type: ignore[name-defined,misc]
+class RetryOnExceptions(tenacity.retry_if_exception):
     """Advanced retry on exceptions.
 
     :param retry_on: Exceptions to retry on
     :type retry_on: type[BaseException] | tuple[type[BaseException], ...]
     :param reraise: Exceptions, which should be reraised, even if subclasses retry_on
     :type reraise: type[BaseException] | tuple[type[BaseException], ...]
     """
@@ -109,15 +112,19 @@
     @property
     def stdin(self) -> paramiko.ChannelFile:  # type: ignore[name-defined]  # paramiko bug: not in __all__
         """Override original NamedTuple with proper typing.
 
         :return: STDIN interface
         :rtype: paramiko.ChannelFile
         """
-        warnings.warn("stdin access deprecated: FIFO is often closed on execution and direct access is not expected.")
+        warnings.warn(
+            "stdin access deprecated: FIFO is often closed on execution and direct access is not expected.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         return super().stdin
 
     @property
     def stderr(self) -> paramiko.ChannelFile | None:  # type: ignore[name-defined]
         """Override original NamedTuple with proper typing.
 
         :return: STDERR interface
@@ -316,15 +323,14 @@
                     self.__auth.enter_password(_stdin)  # type: ignore[arg-type]
                     _stdin.flush()
             else:
                 chan.exec_command(self.command)  # nosec  # Sanitize on caller side
 
             if self.stdin is not None:
                 if not _stdin.channel.closed:
-
                     _stdin.write(self.stdin)
                     _stdin.flush()
                 else:
                     self.logger.warning("STDIN Send failed: closed channel")
 
         if self.open_stdout:
             res_stdout: paramiko.channel.ChannelFile | None = stdout
@@ -395,35 +401,39 @@
 
     :param ssh: connection instance
     :type ssh: SSHClientBase
     :param enforce: keepalive period for context manager
     :type enforce: int
     """
 
-    __slots__ = ("__ssh", "__keepalive_period", "__enforce")
+    __slots__ = ("__ssh", "__keepalive_mode", "__keepalive_period", "__enforce")
 
     def __init__(self, ssh: SSHClientBase, enforce: int) -> None:
         """Context manager for keepalive management."""
         self.__ssh: SSHClientBase = ssh
+        self.__keepalive_mode: bool = ssh.keepalive_mode
         self.__keepalive_period: int = ssh.keepalive_period
         self.__enforce: int = enforce
 
     def __enter__(self) -> None:
         self.__ssh.__enter__()
+        self.__keepalive_mode = self.__ssh.keepalive_mode
         self.__keepalive_period = self.__ssh.keepalive_period
+        self.__ssh.keepalive_mode = bool(self.__enforce)
         self.__ssh.keepalive_period = self.__enforce
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         # Exit before releasing!
         self.__ssh.__exit__(exc_type, exc_val, exc_tb)
+        self.__ssh.keepalive_mode = self.__keepalive_mode
         self.__ssh.keepalive_period = self.__keepalive_period
 
 
 class SSHClientBase(api.ExecHelper):
     """SSH Client helper.
 
     :param host: remote hostname
@@ -463,23 +473,25 @@
     .. versionchanged:: 6.0.0 added optional ssh_auth_map for ssh proxy cases with authentication on each step
     .. versionchanged:: 6.0.0 added optional sock for manual proxy chain handling
     .. versionchanged:: 6.0.0 keepalive exposed to constructor
     .. versionchanged:: 6.0.0 keepalive became int, now used in ssh transport as period of keepalive requests
     .. versionchanged:: 6.0.0 private_keys is deprecated
     .. versionchanged:: 7.0.0 private_keys is removed
     .. versionchanged:: 7.0.0 keepalive_mode is removed
+    .. versionchanged:: 7.4.0 return of keepalive_mode to prevent mix with keepalive period. Default is `False`
     """
 
     __slots__ = (
         "__hostname",
         "__port",
         "__auth_mapping",
         "__ssh",
         "__sftp",
         "__sudo_mode",
+        "__keepalive_mode",
         "__keepalive_period",
         "__verbose",
         "__ssh_config",
         "__sock",
         "__conn_chain",
     )
 
@@ -526,14 +538,15 @@
         self.__auth_mapping = ssh_auth.SSHAuthMapping(ssh_auth_map)
         # We are already resolved hostname
         if self.hostname not in self.__auth_mapping and host in self.__auth_mapping:
             self.__auth_mapping[self.hostname] = self.__auth_mapping[host]
 
         self.__sudo_mode = False
         self.__keepalive_period: int = int(keepalive)
+        self.__keepalive_mode = False
         self.__verbose: bool = verbose
         self.__sock = sock
 
         self.__ssh: paramiko.SSHClient
         self.__sftp: paramiko.SFTPClient | None = None
 
         # Rebuild SSHAuth object if required.
@@ -819,36 +832,27 @@
         """
         try:
             self.__ssh.close()
         except BaseException as e:  # pragma: no cover  # NOSONAR
             self.logger.debug(f"Exception in {self!s} destructor call: {e}")
         self.__sftp = None
 
-    def __enter__(self) -> SSHClientBase:
-        """Get context manager.
-
-        :return: exec helper instance with entered context manager
-        :rtype: SSHClientBase
-        """
-        # noinspection PyTypeChecker
-        return super().__enter__()
-
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         """Exit context manager.
 
         .. versionchanged:: 1.0.0 disconnect enforced on close
         .. versionchanged:: 1.1.0 release lock on exit
         .. versionchanged:: 1.2.1 disconnect enforced on close only not in keepalive mode
         """
-        if not self.__keepalive_period:
+        if self._context_count == 1 and not self.__keepalive_mode:
             self.close()
         super().__exit__(exc_type, exc_val, exc_tb)
 
     @property
     def sudo_mode(self) -> bool:
         """Persistent sudo mode for connection object.
 
@@ -882,14 +886,41 @@
         :type period: int | bool
         If 0 - close connection on exit from context manager.
         """
         self.__keepalive_period = int(period)
         transport: paramiko.Transport = self._ssh_transport
         transport.set_keepalive(int(period))
 
+    @property
+    def keepalive_mode(self) -> bool:
+        """Keepalive mode.
+
+        :rtype: bool
+        Do not close connection on __exit__ if set.
+        """
+        return self.__keepalive_mode
+
+    @keepalive_mode.setter
+    def keepalive_mode(self, mode: bool) -> None:
+        """Keepalive mode.
+
+        :param mode: new mode
+        :type mode: bool
+        Do not close connection on __exit__ if set.
+        """
+        self.__keepalive_mode = mode
+
+    @keepalive_mode.deleter
+    def keepalive_mode(self) -> None:
+        """Keepalive mode.
+
+        Do not close connection on __exit__ if set.
+        """
+        self.keepalive_mode = False
+
     def reconnect(self) -> None:
         """Reconnect SSH session."""
         with self.lock:
             self.close()
             self.__connect()
 
     def sudo(self, enforce: bool | None = None) -> _SudoContext:
@@ -985,15 +1016,15 @@
         .. versionchanged:: 1.2.0 open_stdout and open_stderr flags
         .. versionchanged:: 1.2.0 stdin data
         .. versionchanged:: 1.2.0 get_pty moved to `**kwargs`
         .. versionchanged:: 2.1.0 Use typed NamedTuple as result
         .. versionchanged:: 3.2.0 Expose pty options as optional keyword-only arguments
         .. versionchanged:: 4.1.0 support chroot
         """
-        warnings.warn("_execute_async is deprecated and will be removed soon", DeprecationWarning)
+        warnings.warn("_execute_async is deprecated and will be removed soon", DeprecationWarning, stacklevel=2)
         chan: paramiko.Channel = self._ssh_transport.open_session()
         if timeout is not None:
             chan.settimeout(timeout)
 
         if get_pty:
             # Open PTY
             chan.get_pty(term="vt100", width=width, height=height, width_pixels=0, height_pixels=0)
@@ -1540,15 +1571,15 @@
         password: str | None = None,
         *,
         auth: ssh_auth.SSHAuth | None = None,
         verbose: bool = True,
         ssh_config: (str | paramiko.SSHConfig | SSHConfigsDictT | _ssh_helpers.HostsSSHConfigs | None) = None,
         ssh_auth_map: dict[str, ssh_auth.SSHAuth] | ssh_auth.SSHAuthMapping | None = None,
         keepalive: KeepAlivePeriodT = 1,
-    ) -> SSHClientBase:
+    ) -> Self:
         """Start new SSH connection using current as proxy.
 
         :param host: remote hostname
         :type host: str
         :param port: remote ssh port
         :type port: int | None
         :param username: remote username.
@@ -1581,15 +1612,15 @@
             parsed_ssh_config: _ssh_helpers.HostsSSHConfigs = ssh_config
         else:
             parsed_ssh_config = _ssh_helpers.parse_ssh_config(ssh_config, host)
 
         hostname = parsed_ssh_config[host].hostname
 
         sock: paramiko.Channel = self._get_proxy_channel(port=port, ssh_config=parsed_ssh_config[hostname])
-        cls: type[SSHClientBase] = self.__class__
+        cls: type[Self] = self.__class__
         return cls(
             host=host,
             port=port,
             username=username,
             password=password,
             auth=auth,
             verbose=verbose,
@@ -1659,15 +1690,15 @@
         .. versionchanged:: 1.2.0 log_mask_re regex rule for masking cmd
         .. versionchanged:: 3.2.0 Expose pty options as optional keyword-only arguments
         .. versionchanged:: 4.0.0 Expose stdin and log_mask_re as optional keyword-only arguments
         .. versionchanged:: 6.0.0 Move channel open to separate method and make proper ssh-proxy usage
         .. versionchanged:: 6.0.0 only hostname and command are positional argument, target_port changed to port.
         .. versionchanged:: 7.0.0 target_port argument removed
         """
-        conn: SSHClientBase
+        conn: Self
         if auth is None:
             auth = self.auth
 
         with self.proxy_to(
             host=hostname,
             port=port,
             auth=auth,
@@ -1810,15 +1841,15 @@
 
         for remote, future in futures.items():
             try:
                 result = future.result(timeout=0.1)
                 results[(remote.hostname, remote.port)] = result
                 if result.exit_code not in prep_expected:
                     errors[(remote.hostname, remote.port)] = result
-            except Exception as e:
+            except Exception as e:  # noqa: PERF203
                 raised_exceptions[(remote.hostname, remote.port)] = e
 
         if raised_exceptions:  # always raise
             raise exceptions.ParallelCallExceptionsError(
                 command=cmd,
                 exceptions=raised_exceptions,
                 errors=errors,
```

### Comparing `exec-helpers-7.3.6/exec_helpers/_ssh_helpers.py` & `exec-helpers-7.4.0/exec_helpers/_ssh_helpers.py`

 * *Files identical despite different names*

### Comparing `exec-helpers-7.3.6/exec_helpers/_subprocess_helpers.py` & `exec-helpers-7.4.0/exec_helpers/_subprocess_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2022 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 
 #         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `exec-helpers-7.3.6/exec_helpers/api.py` & `exec-helpers-7.4.0/exec_helpers/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2022 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 
 #         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -40,14 +40,17 @@
 from . import _helpers
 
 if typing.TYPE_CHECKING:
     # Standard Library
     from collections.abc import Sequence
     from types import TracebackType
 
+    # External Dependencies
+    from typing_extensions import Self
+
 __all__ = (
     "ExecHelper",
     "ExecuteAsyncResult",
     "CalledProcessErrorSubClassT",
     "OptionalStdinT",
     "OptionalTimeoutT",
     "CommandT",
@@ -224,22 +227,29 @@
     :type log_mask_re: str | re.Pattern[str] | None
 
     .. versionchanged:: 1.2.0 log_mask_re regex rule for masking cmd
     .. versionchanged:: 1.3.5 make API public to use as interface
     .. versionchanged:: 4.1.0 support chroot
     """
 
-    __slots__ = ("__lock", "__logger", "log_mask_re", "__chroot_path")
+    __slots__ = (
+        "__lock",
+        "__logger",
+        "log_mask_re",
+        "__chroot_path",
+        "__context_count",
+    )
 
     def __init__(self, log_mask_re: LogMaskReT = None, *, logger: logging.Logger) -> None:
         """Global ExecHelper API."""
         self.__lock = threading.RLock()
         self.__logger: logging.Logger = logger
         self.log_mask_re: LogMaskReT = log_mask_re
         self.__chroot_path: str | None = None
+        self.__context_count = 0
 
     @property
     def logger(self) -> logging.Logger:
         """Instance logger access.
 
         :return: logger instance
         :rtype: logging.Logger
@@ -296,32 +306,39 @@
         :rtype: typing.ContextManager
 
         .. Note:: Enter and exit main context manager is produced as well.
         .. versionadded:: 4.1.0
         """
         return _ChRootContext(conn=self, path=path)
 
-    def __enter__(self) -> ExecHelper:
+    @property
+    def _context_count(self) -> int:
+        """Instance context enter count."""
+        return self.__context_count
+
+    def __enter__(self) -> Self:
         """Get context manager.
 
         :return: exec helper instance with entered context manager
         :rtype: ExecHelper
 
         .. versionchanged:: 1.1.0 lock on enter
         """
         self.lock.acquire()
+        self.__context_count += 1
         return self
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         """Context manager usage."""
+        self.__context_count -= 1
         self.lock.release()
 
     def _mask_command(self, cmd: str, log_mask_re: LogMaskReT = None) -> str:
         """Log command with masking and return parsed cmd.
 
         :param cmd: command
         :type cmd: str
```

### Comparing `exec-helpers-7.3.6/exec_helpers/async_api/__init__.py` & `exec-helpers-7.4.0/exec_helpers/async_api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2022 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 
 #         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -56,15 +56,19 @@
 def __getattr__(name: str) -> typing.Any:
     """Get attributes lazy.
 
     :return: attribute by name
     :raises AttributeError: attribute is not defined for lazy load
     """
     if name in _deprecated:
-        warnings.warn(f"{name} is deprecated in favor of {_deprecated[name]}", DeprecationWarning)
+        warnings.warn(
+            f"{name} is deprecated in favor of {_deprecated[name]}",
+            DeprecationWarning,
+            stacklevel=2,
+        )
     if name in __lazy_load_modules:
         mod = importlib.import_module(f"{__package__}.{name}")
         __locals[name] = mod
         return mod
     if name in __lazy_load_parent_modules:
         mod = importlib.import_module(f"{__package__}.{__lazy_load_parent_modules[name]}")
         obj = getattr(mod, name)
```

### Comparing `exec-helpers-7.3.6/exec_helpers/async_api/__init__.pyi` & `exec-helpers-7.4.0/exec_helpers/async_api/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2021 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 
 #         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -13,34 +13,36 @@
 #    under the License.
 
 """Execution helpers for simplified usage of subprocess. Async version.
 
 .. versionadded:: 3.0.0
 """
 
+from __future__ import annotations
+
+# Standard Library
+import typing
+
+# Local Implementation
+from .api import ExecHelper
+from .exec_result import ExecResult
+from .subprocess import Subprocess  # nosec  # Expected
+
 # noinspection PyUnresolvedReferences
 __all__ = (
     # pylint: disable=undefined-all-variable
     # lazy load
     # API
     "ExecHelper",
     "ExecResult",
     # Expensive
     "Subprocess",
 )
 
-# Standard Library
-import typing
-
-# Local Implementation
-from .api import ExecHelper
-from .exec_result import ExecResult
-from .subprocess import Subprocess  # nosec  # Expected
-
-_deprecated: typing.Dict[str, str] = ...
+_deprecated: dict[str, str] = ...
 
 def __getattr__(name: str) -> typing.Any:
     """Get attributes lazy.
 
     :return: attribute by name
     :raises AttributeError: attribute is not defined for lazy load
     """
```

### Comparing `exec-helpers-7.3.6/exec_helpers/async_api/api.py` & `exec-helpers-7.4.0/exec_helpers/async_api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2022 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 
 #         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -45,14 +45,17 @@
 from .. import _helpers
 
 if typing.TYPE_CHECKING:
     # Standard Library
     import types
     from collections.abc import Sequence
 
+    # External Dependencies
+    from typing_extensions import Self
+
     # Package Implementation
     from exec_helpers.proc_enums import ExitCodeT
 
 __all__ = (
     "ExecHelper",
     "CalledProcessErrorSubClassT",
     "OptionalStdinT",
@@ -269,15 +272,15 @@
         :rtype: typing.ContextManager
 
         .. Note:: Enter and exit main context manager is produced as well.
         .. versionadded:: 4.1.0
         """
         return _ChRootContext(conn=self, path=path)
 
-    async def __aenter__(self) -> ExecHelper:
+    async def __aenter__(self) -> Self:
         """Async context manager.
 
         :return: exec helper instance with async entered context manager
         :rtype: ExecHelper
         """
         if self.__alock is None:
             self.__alock = asyncio.Lock()
```

### Comparing `exec-helpers-7.3.6/exec_helpers/async_api/exec_result.py` & `exec-helpers-7.4.0/exec_helpers/async_api/exec_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2022 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 
 #         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `exec-helpers-7.3.6/exec_helpers/async_api/subprocess.py` & `exec-helpers-7.4.0/exec_helpers/async_api/subprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2022 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 
 #         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -17,14 +17,15 @@
 .. versionadded:: 3.0.0
 """
 
 from __future__ import annotations
 
 # Standard Library
 import asyncio
+import contextlib
 import copy
 import datetime
 import errno
 import logging
 import os
 import typing
 import warnings
@@ -80,15 +81,19 @@
     @property
     def stdin(self) -> asyncio.StreamWriter | None:  # type: ignore[override]
         """Override original NamedTuple with proper typing.
 
         :return: STDIN interface
         :rtype: asyncio.StreamWriter | None
         """
-        warnings.warn("stdin access deprecated: FIFO is often closed on execution and direct access is not expected.")
+        warnings.warn(
+            "stdin access deprecated: FIFO is often closed on execution and direct access is not expected.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         return super().stdin  # type: ignore[return-value]
 
     @property
     def stderr(self) -> AsyncIterable[bytes] | None:  # type: ignore[override]
         """Override original NamedTuple with proper typing.
 
         :return: STDERR interface
@@ -230,18 +235,16 @@
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: types.TracebackType | None,
     ) -> None:
         process = self.__process
         if process is not None:  # pylint: disable=consider-using-assignment-expr
             _subprocess_helpers.kill_proc_tree(process.pid)
-            try:
+            with contextlib.suppress(ProcessLookupError):
                 process.kill()
-            except ProcessLookupError:
-                pass  # process already closed
             self.__process = None
 
 
 class Subprocess(api.ExecHelper):
     """Subprocess helper with timeouts and lock-free FIFO.
 
     :param log_mask_re: regex lookup rule to mask command for logger.
@@ -263,32 +266,14 @@
         log_mask_re: LogMaskReT = None,
         *,
         logger: logging.Logger = logging.getLogger(__name__),  # noqa: B008
     ) -> None:
         """Subprocess helper with timeouts and lock-free FIFO."""
         super().__init__(logger=logger, log_mask_re=log_mask_re)
 
-    async def __aenter__(self) -> Subprocess:
-        """Async context manager.
-
-        :return: exec helper instance with async entered context manager
-        :rtype: Subprocess
-        """
-        # noinspection PyTypeChecker
-        return await super().__aenter__()
-
-    def __enter__(self) -> Subprocess:  # pylint: disable=useless-super-delegation
-        """Get context manager.
-
-        :return: exec helper instance with entered context manager
-        :rtype: Subprocess
-        """
-        # noinspection PyTypeChecker
-        return super().__enter__()  # type: ignore[no-any-return]  # pylint: disable=no-member
-
     async def _exec_command(  # type: ignore[override]
         self,
         command: str,
         async_result: SubprocessExecuteAsyncResult,
         timeout: OptionalTimeoutT,
         *,
         verbose: bool = False,
@@ -409,15 +394,15 @@
                         ('stderr', asyncio.StreamReader | None),
                         ('stdout', asyncio.StreamReader | None),
                         ("started", datetime.datetime),
                     ]
                 )
         :raises OSError: impossible to process STDIN
         """
-        warnings.warn("_execute_async is deprecated and will be removed soon", DeprecationWarning)
+        warnings.warn("_execute_async is deprecated and will be removed soon", DeprecationWarning, stacklevel=2)
         started = datetime.datetime.utcnow()
 
         if env_patch is not None:
             # make mutable copy
             env = dict(copy.deepcopy(os.environ) if env is None else copy.deepcopy(env))  # type: ignore[arg-type]
             env.update(env_patch)  # type: ignore[arg-type]
```

### Comparing `exec-helpers-7.3.6/exec_helpers/constants.py` & `exec-helpers-7.4.0/exec_helpers/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2022 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 
 #         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `exec-helpers-7.3.6/exec_helpers/exceptions.py` & `exec-helpers-7.4.0/exec_helpers/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2022 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 
 #         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -27,15 +27,15 @@
 
 if typing.TYPE_CHECKING:
     # Standard Library
     from collections.abc import Iterable
     from collections.abc import Sequence
 
     # Package Implementation
-    from exec_helpers import exec_result  # noqa: F401  # pylint: disable=cyclic-import
+    from exec_helpers import exec_result  # pylint: disable=cyclic-import
     from exec_helpers.proc_enums import ExitCodeT
 
 __all__ = (
     "ExecHelperError",
     "ExecHelperNoKillError",
     "ExecHelperTimeoutError",
     "ExecCalledProcessError",
@@ -319,18 +319,18 @@
             expected=expected,
             _message=message,
         )
         self.cmd: str = command
         self.exceptions: dict[tuple[str, int], Exception] = exceptions
 
 
-ParallelCallExceptions = ParallelCallExceptionsError  # noqa: N818
+ParallelCallExceptions = ParallelCallExceptionsError
 
 
-class StopExecution(Exception):  # noqa: N818
+class StopExecution(Exception):
     """Stop execution without waiting for exit code."""
 
     def __init__(
         self,
         trigger_line: bytes,
         result: exec_result.ExecResult,
         message: str = "StopExecution raised",
@@ -363,15 +363,15 @@
 
         :return: execution result object
         :rtype: exec_result.ExecResult
         """
         return self.__result
 
 
-class StopExecutionGraceful(StopExecution):  # noqa: N818
+class StopExecutionGraceful(StopExecution):
     """Stop execution without raising exception."""
 
     def __init__(
         self,
         trigger_line: bytes,
         result: exec_result.ExecResult,
     ) -> None:
```

### Comparing `exec-helpers-7.3.6/exec_helpers/exec_result.py` & `exec-helpers-7.4.0/exec_helpers/exec_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2022 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Copyright 2016 Mirantis, Inc.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 
@@ -203,29 +203,29 @@
         """
         return f"{self.__class__.__name__}(data={self._data!r})"
 
 
 class ExecResult:
     """Execution result."""
 
-    __slots__ = [
+    __slots__ = (
         "__cmd",
         "__stdin",
         "_stdout",
         "_stderr",
         "__exit_code",
         "__timestamp",
         "_stdout_str",
         "_stderr_str",
         "_stdout_brief",
         "_stderr_brief",
         "__stdout_lock",
         "__stderr_lock",
         "__started",
-    ]
+    )
 
     def __init__(
         self,
         cmd: str,
         stdin: OptionalStdinT = None,
         stdout: Iterable[bytes] | None = None,
         stderr: Iterable[bytes] | None = None,
```

### Comparing `exec-helpers-7.3.6/exec_helpers/proc_enums.py` & `exec-helpers-7.4.0/exec_helpers/proc_enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2022 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Copyright 2016 Mirantis, Inc.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 
@@ -182,25 +182,25 @@
         :return: string with value in decimal, hex and text information
         :rtype: str
         """
         return f"{self.name}<{self.value:d}(0x{self.value:02X})>"
 
 
 ExitCodeT = typing.Union[int, ExitCodes]
-EXPECTED: ExitCodeT = 0 if "win32" == sys.platform else ExitCodes.EX_OK
-INVALID: ExitCodeT = 0xDEADBEEF if "win32" == sys.platform else ExitCodes.EX_INVALID
+EXPECTED: ExitCodeT = 0 if sys.platform == "win32" else ExitCodes.EX_OK
+INVALID: ExitCodeT = 0xDEADBEEF if sys.platform == "win32" else ExitCodes.EX_INVALID
 
 
 def exit_code_to_enum(code: ExitCodeT) -> ExitCodeT:  # pragma: no cover
     """Convert exit code to enum if possible.
 
     :param code: code to convert from
     :return: enum code if suitable else original code
     """
-    if "win32" == sys.platform:
+    if sys.platform == "win32":
         return int(code)
     if isinstance(code, int) and code in ExitCodes.__members__.values():
         return ExitCodes(code)
     return code
 
 
 def exit_codes_to_enums(codes: Iterable[ExitCodeT] | None = None) -> Sequence[ExitCodeT]:
```

### Comparing `exec-helpers-7.3.6/exec_helpers/ssh.py` & `exec-helpers-7.4.0/exec_helpers/ssh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2022 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Copyright 2013 - 2016 Mirantis, Inc.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 
@@ -35,22 +35,14 @@
 
 
 class SSHClient(_ssh_base.SSHClientBase):
     """SSH Client helper."""
 
     __slots__ = ()
 
-    def __enter__(self) -> SSHClient:
-        """Get context manager.
-
-        :return: SSHClient instance with entered context
-        :rtype: SSHClient
-        """
-        return super().__enter__()
-
     @staticmethod
     def _path_esc(path: str) -> str:
         """Escape space character in the path.
 
         :param path: path to be escaped
         :type path: str
         :return: path with escaped spaces
```

### Comparing `exec-helpers-7.3.6/exec_helpers/ssh_auth.py` & `exec-helpers-7.4.0/exec_helpers/ssh_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2022 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Copyright 2013 - 2016 Mirantis, Inc.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 
@@ -201,15 +201,15 @@
                     key_filename=self.__key_filename,  # type: ignore[arg-type]  # types verified by not signature
                     **kwargs,
                 )
                 if index != self.__key_index:
                     self.__key_index = index
                     LOGGER.debug(f"Main key has been updated, public key is: \n{self.public_key}")
                 return
-            except paramiko.PasswordRequiredException:
+            except paramiko.PasswordRequiredException:  # noqa: PERF203
                 if self.__password is None:
                     LOGGER.exception("No password has been set!")
                     raise
                 LOGGER.critical("Unexpected PasswordRequiredException, when password is set!")
                 raise
             except (paramiko.AuthenticationException, paramiko.BadHostKeyException):
                 continue
```

### Comparing `exec-helpers-7.3.6/exec_helpers/subprocess.py` & `exec-helpers-7.4.0/exec_helpers/subprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2018 - 2022 Alexey Stepanov aka penguinolog.
+#    Copyright 2018 - 2023 Aleksei Stepanov aka penguinolog.
 
 #    Copyright 2016 Mirantis, Inc.
 
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 
@@ -65,30 +65,34 @@
 # noinspection PyTypeHints
 class SubprocessExecuteAsyncResult(api.ExecuteAsyncResult):
     """Override original NamedTuple with proper typing."""
 
     __slots__ = ()
 
     @property
-    def interface(self) -> subprocess.Popen[bytes]:  # noqa: E1136
+    def interface(self) -> subprocess.Popen[bytes]:
         """Override original NamedTuple with proper typing.
 
         :return: control interface
         :rtype: subprocess.Popen[bytes]
         """
         return super().interface  # type: ignore[no-any-return]
 
     @property
     def stdin(self) -> typing.IO[bytes] | None:
         """Override original NamedTuple with proper typing.
 
         :return: STDIN interface
         :rtype: typing.IO[bytes] | None
         """
-        warnings.warn("stdin access deprecated: FIFO is often closed on execution and direct access is not expected.")
+        warnings.warn(
+            "stdin access deprecated: FIFO is often closed on execution and direct access is not expected.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         return super().stdin
 
     @property
     def stderr(self) -> typing.IO[bytes] | None:
         """Override original NamedTuple with proper typing.
 
         :return: STDERR interface
@@ -266,23 +270,14 @@
         """Subprocess helper with timeouts and lock-free FIFO."""
         mod_name = "exec_helpers" if self.__module__.startswith("exec_helpers") else self.__module__
         super().__init__(
             logger=logging.getLogger(f"{mod_name}.{self.__class__.__name__}"),
             log_mask_re=log_mask_re,
         )
 
-    def __enter__(self) -> Subprocess:
-        """Get context manager.
-
-        :return: exec helper instance with entered context manager
-        :rtype: Subprocess
-        """
-        # noinspection PyTypeChecker
-        return super().__enter__()
-
     def _exec_command(  # type: ignore[override]
         self,
         command: str,
         async_result: SubprocessExecuteAsyncResult,
         timeout: OptionalTimeoutT,
         *,
         verbose: bool = False,
@@ -426,15 +421,15 @@
         :raises OSError: impossible to process STDIN
 
         .. versionadded:: 1.2.0
         .. versionchanged:: 2.1.0 Use typed NamedTuple as result
         .. versionchanged:: 3.2.0 Expose cwd and env as optional keyword-only arguments
         .. versionchanged:: 4.1.0 support chroot
         """
-        warnings.warn("_execute_async is deprecated and will be removed soon", DeprecationWarning)
+        warnings.warn("_execute_async is deprecated and will be removed soon", DeprecationWarning, stacklevel=2)
         started = datetime.datetime.utcnow()
 
         if env_patch is not None:
             # make mutable copy
             env = dict(copy.deepcopy(os.environ) if env is None else copy.deepcopy(env))  # type: ignore[arg-type]
             env.update(env_patch)  # type: ignore[arg-type]
```

### Comparing `exec-helpers-7.3.6/exec_helpers.egg-info/PKG-INFO` & `exec-helpers-7.4.0/exec_helpers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: exec-helpers
-Version: 7.3.6
+Version: 7.4.0
 Summary: Execution helpers for simplified usage of subprocess and ssh.
+Home-page: https://github.com/python-useful-helpers/exec-helpers
 Author-email: Alexey Stepanov <penguinolog@gmail.com>
-Maintainer-email: Alexey Stepanov <penguinolog@gmail.com>, Antonio Esposito <esposito.cloud@gmail.com>, Dennis Dmitriev <dis-xcom@gmail.com>
-License: Apache License, Version 2.0
-Project-URL: Bug Tracker, https://github.com/python-useful-helpers/exec-helpers/issues
+Maintainer-email: Aleksei Stepanov <penguinolog@gmail.com>, Antonio Esposito <esposito.cloud@gmail.com>, Dennis Dmitriev <dis-xcom@gmail.com>
+License: Apache-2.0
 Project-URL: Documentation, https://exec-helpers.readthedocs.io/
+Project-URL: Repository, https://github.com/python-useful-helpers/exec-helpers
+Project-URL: Bug Tracker, https://github.com/python-useful-helpers/exec-helpers/issues
 Keywords: subprocess,ssh
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `exec-helpers-7.3.6/exec_helpers.egg-info/SOURCES.txt` & `exec-helpers-7.4.0/exec_helpers.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 exec_helpers/py.typed
 exec_helpers/ssh.py
 exec_helpers/ssh_auth.py
 exec_helpers/subprocess.py
 exec_helpers.egg-info/PKG-INFO
 exec_helpers.egg-info/SOURCES.txt
 exec_helpers.egg-info/dependency_links.txt
+exec_helpers.egg-info/not-zip-safe
 exec_helpers.egg-info/requires.txt
 exec_helpers.egg-info/top_level.txt
 exec_helpers/async_api/__init__.py
 exec_helpers/async_api/__init__.pyi
 exec_helpers/async_api/api.py
 exec_helpers/async_api/exec_result.py
 exec_helpers/async_api/subprocess.py
```

