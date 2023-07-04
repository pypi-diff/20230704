# Comparing `tmp/ez-a-sync-0.5.4.tar.gz` & `tmp/ez-a-sync-0.5.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-a-sync-0.5.4.tar", last modified: Mon Jul  3 20:45:31 2023, max compression
+gzip compressed data, was "ez-a-sync-0.5.5.dev1.tar", last modified: Tue Jul  4 05:43:19 2023, max compression
```

## Comparing `ez-a-sync-0.5.4.tar` & `ez-a-sync-0.5.5.dev1.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:45:31.015968 ez-a-sync-0.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:45:31.011968 ez-a-sync-0.5.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:45:31.011968 ez-a-sync-0.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-03 20:45:31.015968 ez-a-sync-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/TODO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:45:31.011968 ez-a-sync-0.5.4/a_sync/
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4513 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/_bound.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/_typing.py
--rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6097 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5019 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/modified.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:45:31.011968 ez-a-sync-0.5.4/a_sync/modifiers/
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/modifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:45:31.015968 ez-a-sync-0.5.4/a_sync/modifiers/cache/
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/modifiers/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/modifiers/cache/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/modifiers/limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/modifiers/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     2405 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/modifiers/semaphores.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:45:31.015968 ez-a-sync-0.5.4/a_sync/primitives/
--rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/primitives/_loggable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7338 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/primitives/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:45:31.015968 ez-a-sync-0.5.4/a_sync/primitives/locks/
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/primitives/locks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/primitives/locks/counter.py
--rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/primitives/locks/event.py
--rw-r--r--   0 runner    (1001) docker     (122)     4025 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/primitives/locks/semaphore.py
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/property.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/a_sync/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:45:31.015968 ez-a-sync-0.5.4/ez_a_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-03 20:45:30.000000 ez-a-sync-0.5.4/ez_a_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-07-03 20:45:30.000000 ez-a-sync-0.5.4/ez_a_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 20:45:30.000000 ez-a-sync-0.5.4/ez_a_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-03 20:45:30.000000 ez-a-sync-0.5.4/ez_a_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-03 20:45:30.000000 ez-a-sync-0.5.4/ez_a_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-03 20:45:31.015968 ez-a-sync-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:45:31.015968 ez-a-sync-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/tests/executor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/tests/test_limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-03 20:45:19.000000 ez-a-sync-0.5.4/tests/test_semaphore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 05:43:19.510616 ez-a-sync-0.5.5.dev1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 05:43:19.506615 ez-a-sync-0.5.5.dev1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 05:43:19.506615 ez-a-sync-0.5.5.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-04 05:43:19.510616 ez-a-sync-0.5.5.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/TODO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 05:43:19.510616 ez-a-sync-0.5.5.dev1/a_sync/
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4513 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/_bound.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6097 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5019 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/modified.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 05:43:19.510616 ez-a-sync-0.5.5.dev1/a_sync/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/modifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 05:43:19.510616 ez-a-sync-0.5.5.dev1/a_sync/modifiers/cache/
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/modifiers/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/modifiers/cache/memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/modifiers/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/modifiers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2405 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/modifiers/semaphores.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 05:43:19.510616 ez-a-sync-0.5.5.dev1/a_sync/primitives/
+-rw-r--r--   0 runner    (1001) docker     (122)      500 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/primitives/_loggable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7589 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/primitives/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 05:43:19.510616 ez-a-sync-0.5.5.dev1/a_sync/primitives/locks/
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/primitives/locks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/primitives/locks/counter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/primitives/locks/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4025 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/primitives/locks/semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/property.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/a_sync/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 05:43:19.510616 ez-a-sync-0.5.5.dev1/ez_a_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-04 05:43:19.000000 ez-a-sync-0.5.5.dev1/ez_a_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-07-04 05:43:19.000000 ez-a-sync-0.5.5.dev1/ez_a_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-04 05:43:19.000000 ez-a-sync-0.5.5.dev1/ez_a_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-04 05:43:19.000000 ez-a-sync-0.5.5.dev1/ez_a_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-04 05:43:19.000000 ez-a-sync-0.5.5.dev1/ez_a_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-04 05:43:19.510616 ez-a-sync-0.5.5.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 05:43:19.510616 ez-a-sync-0.5.5.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/tests/executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/tests/test_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-04 05:43:01.000000 ez-a-sync-0.5.5.dev1/tests/test_semaphore.py
```

### Comparing `ez-a-sync-0.5.4/.github/workflows/codeql.yaml` & `ez-a-sync-0.5.5.dev1/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/.github/workflows/mypy.yaml` & `ez-a-sync-0.5.5.dev1/.github/workflows/mypy.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/.github/workflows/pytest.yaml` & `ez-a-sync-0.5.5.dev1/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/.github/workflows/release.yaml` & `ez-a-sync-0.5.5.dev1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/LICENSE.txt` & `ez-a-sync-0.5.5.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/README.md` & `ez-a-sync-0.5.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/__init__.py` & `ez-a-sync-0.5.5.dev1/a_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/_bound.py` & `ez-a-sync-0.5.5.dev1/a_sync/_bound.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/_flags.py` & `ez-a-sync-0.5.5.dev1/a_sync/_flags.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/_helpers.py` & `ez-a-sync-0.5.5.dev1/a_sync/_helpers.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/_kwargs.py` & `ez-a-sync-0.5.5.dev1/a_sync/_kwargs.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/_meta.py` & `ez-a-sync-0.5.5.dev1/a_sync/_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/_typing.py` & `ez-a-sync-0.5.5.dev1/a_sync/_typing.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/abstract.py` & `ez-a-sync-0.5.5.dev1/a_sync/abstract.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/base.py` & `ez-a-sync-0.5.5.dev1/a_sync/base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/config.py` & `ez-a-sync-0.5.5.dev1/a_sync/config.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/decorator.py` & `ez-a-sync-0.5.5.dev1/a_sync/decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/exceptions.py` & `ez-a-sync-0.5.5.dev1/a_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/modified.py` & `ez-a-sync-0.5.5.dev1/a_sync/modified.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/modifiers/__init__.py` & `ez-a-sync-0.5.5.dev1/a_sync/modifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/modifiers/cache/__init__.py` & `ez-a-sync-0.5.5.dev1/a_sync/modifiers/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/modifiers/cache/memory.py` & `ez-a-sync-0.5.5.dev1/a_sync/modifiers/cache/memory.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/modifiers/limiter.py` & `ez-a-sync-0.5.5.dev1/a_sync/modifiers/limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/modifiers/manager.py` & `ez-a-sync-0.5.5.dev1/a_sync/modifiers/manager.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/modifiers/semaphores.py` & `ez-a-sync-0.5.5.dev1/a_sync/modifiers/semaphores.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/primitives/executor.py` & `ez-a-sync-0.5.5.dev1/a_sync/primitives/executor.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,17 +31,18 @@
         Doesn't `await this_executor.run(fn, *args)` look so much better?
         """
         self._check_kwargs(_kwargs_dont_work_but_i_need_this_here_to_make_type_hints_work)
         t = self._start_debug_daemon(fn, *args)
         retval = await self._aioloop_run_in_executor(self, fn, *args)
         t.cancel()
         return retval
-    def submit(self, fn: Callable[P, T], *args: P.args, **_kwargs_dont_work_but_i_need_this_here_to_make_type_hints_work: P.kwargs) -> "asyncio.Task[T]":
-        """Submits a job to the executor and returns an `asyncio.Task` that can be awaited for the result."""
-        return asyncio.ensure_future(self.run(fn, *args, **_kwargs_dont_work_but_i_need_this_here_to_make_type_hints_work))
+    # TODO: implement this later so submit returns asyncio.Future instead of cf.Future
+    #def submit(self, fn: Callable[P, T], *args: P.args, **_kwargs_dont_work_but_i_need_this_here_to_make_type_hints_work: P.kwargs) -> "asyncio.Task[T]":
+    #    """Submits a job to the executor and returns an `asyncio.Task` that can be awaited for the result."""
+    #    return asyncio.ensure_future(self.run(fn, *args, **_kwargs_dont_work_but_i_need_this_here_to_make_type_hints_work))
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} object at {hex(id(self))} [{len(self)}/{self._max_workers} {self._workers}]>"
     def __len__(self) -> int:
         return len(getattr(self, f"_{self._workers}"))
     @cached_property
     def _aioloop_run_in_executor(self) -> asyncio.BaseEventLoop:
         return asyncio.get_event_loop().run_in_executor
@@ -54,21 +55,27 @@
             await asyncio.sleep(15)
             logger.debug(f'{self} processing {fn}{args}')
     def _start_debug_daemon(self, fn, *args) -> "asyncio.Task[NoReturn]":
         return asyncio.create_task(self._debug_daemon(fn, *args))
     
 # Process
 
-class ProcessPoolExecutor(cf.ProcessPoolExecutor, _ASyncExecutorBase):
+class AsyncProcessPoolExecutor(cf.ProcessPoolExecutor, _ASyncExecutorBase):
     _workers = "processes"
 
 # Thread
 
-class ThreadPoolExecutor(cf.ThreadPoolExecutor, _ASyncExecutorBase):
+class AsyncThreadPoolExecutor(cf.ThreadPoolExecutor, _ASyncExecutorBase):
     _workers = "threads"
+    
+# For backward-compatibility
+ProcessPoolExecutor = AsyncProcessPoolExecutor
+ThreadPoolExecutor = AsyncThreadPoolExecutor
+
+# Pruning thread pool
 
 def _worker(executor_reference, work_queue, initializer, initargs, timeout):  # NOTE: NEW 'timeout'
     if initializer is not None:
         try:
             initializer(*initargs)
         except BaseException:
             _base.LOGGER.critical('Exception in initializer:', exc_info=True)
@@ -123,15 +130,15 @@
                 # Notice other workers
                 work_queue.put(None)
                 return
             del executor
     except BaseException:
         _base.LOGGER.critical('Exception in worker', exc_info=True)
 
-class PruningThreadPoolExecutor(cf.ThreadPoolExecutor):
+class PruningThreadPoolExecutor(AsyncThreadPoolExecutor):
     """
     This ThreadPoolExecutor implementation prunes inactive threads after 'timeout' seconds without a work item.
     Pruned threads will be automatically recreated as needed for future workloads. up to 'max_threads' can be active at any one time.
     """
     def __init__(self, max_workers=None, thread_name_prefix='',
                  initializer=None, initargs=(), timeout=TEN_MINUTES):
         self._timeout=timeout
```

### Comparing `ez-a-sync-0.5.4/a_sync/primitives/locks/counter.py` & `ez-a-sync-0.5.5.dev1/a_sync/primitives/locks/counter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/primitives/locks/event.py` & `ez-a-sync-0.5.5.dev1/a_sync/primitives/locks/event.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/primitives/locks/semaphore.py` & `ez-a-sync-0.5.5.dev1/a_sync/primitives/locks/semaphore.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/a_sync/property.py` & `ez-a-sync-0.5.5.dev1/a_sync/property.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/ez_a_sync.egg-info/SOURCES.txt` & `ez-a-sync-0.5.5.dev1/ez_a_sync.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -49,10 +49,11 @@
 tests/__init__.py
 tests/conftest.py
 tests/executor.py
 tests/fixtures.py
 tests/test_base.py
 tests/test_cache.py
 tests/test_decorator.py
+tests/test_executor.py
 tests/test_limiter.py
 tests/test_meta.py
 tests/test_semaphore.py
```

### Comparing `ez-a-sync-0.5.4/setup.py` & `ez-a-sync-0.5.5.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/tests/fixtures.py` & `ez-a-sync-0.5.5.dev1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/tests/test_base.py` & `ez-a-sync-0.5.5.dev1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/tests/test_cache.py` & `ez-a-sync-0.5.5.dev1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/tests/test_decorator.py` & `ez-a-sync-0.5.5.dev1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/tests/test_limiter.py` & `ez-a-sync-0.5.5.dev1/tests/test_limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/tests/test_meta.py` & `ez-a-sync-0.5.5.dev1/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.4/tests/test_semaphore.py` & `ez-a-sync-0.5.5.dev1/tests/test_semaphore.py`

 * *Files identical despite different names*

