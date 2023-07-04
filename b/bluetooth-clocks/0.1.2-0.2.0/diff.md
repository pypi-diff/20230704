# Comparing `tmp/bluetooth-clocks-0.1.2.tar.gz` & `tmp/bluetooth-clocks-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluetooth-clocks-0.1.2.tar", last modified: Thu Feb  2 08:16:15 2023, max compression
+gzip compressed data, was "bluetooth-clocks-0.2.0.tar", last modified: Tue Jul  4 13:32:57 2023, max compression
```

## Comparing `bluetooth-clocks-0.1.2.tar` & `bluetooth-clocks-0.2.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:16:15.891975 bluetooth-clocks-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:16:15.887974 bluetooth-clocks-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:16:15.887974 bluetooth-clocks-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12192 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-02-02 08:16:15.895974 bluetooth-clocks-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:16:15.891975 bluetooth-clocks-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:16:15.891975 bluetooth-clocks-0.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)   497996 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/docs/_static/synchronized-clocks.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/docs/devices.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-02-02 08:16:15.895974 bluetooth-clocks-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:16:15.887974 bluetooth-clocks-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:16:15.891975 bluetooth-clocks-0.1.2/src/bluetooth_clocks/
--rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:16:15.891975 bluetooth-clocks-0.1.2/src/bluetooth_clocks/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks/devices/current_time_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks/devices/pvvx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks/devices/qingping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks/devices/thermopro.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks/devices/xiaomi.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks/scanners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:16:15.891975 bluetooth-clocks-0.1.2/src/bluetooth_clocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-02-02 08:16:15.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-02-02 08:16:15.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 08:16:15.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-02 08:16:15.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 08:16:15.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-02 08:16:15.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-02 08:16:15.000000 bluetooth-clocks-0.1.2/src/bluetooth_clocks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:16:15.891975 bluetooth-clocks-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/tests/test_bluetooth_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/tests/test_current_time_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/tests/test_pvvx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/tests/test_qingping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/tests/test_thermopro.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/tests/test_xiaomi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-02-02 08:14:43.000000 bluetooth-clocks-0.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:32:57.189039 bluetooth-clocks-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:32:57.181038 bluetooth-clocks-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:32:57.185039 bluetooth-clocks-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12192 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-04 13:32:57.189039 bluetooth-clocks-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:32:57.185039 bluetooth-clocks-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:32:57.185039 bluetooth-clocks-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)   497996 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/docs/_static/synchronized-clocks.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/docs/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-04 13:32:57.189039 bluetooth-clocks-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:32:57.181038 bluetooth-clocks-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:32:57.185039 bluetooth-clocks-0.2.0/src/bluetooth_clocks/
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:32:57.189039 bluetooth-clocks-0.2.0/src/bluetooth_clocks/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks/devices/current_time_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks/devices/pvvx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks/devices/qingping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks/devices/thermopro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks/devices/xiaomi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks/scanners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:32:57.189039 bluetooth-clocks-0.2.0/src/bluetooth_clocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-04 13:32:57.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-04 13:32:57.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:32:57.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 13:32:57.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:32:56.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-04 13:32:57.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 13:32:57.000000 bluetooth-clocks-0.2.0/src/bluetooth_clocks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:32:57.189039 bluetooth-clocks-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/tests/test_bluetooth_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/tests/test_current_time_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/tests/test_pvvx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/tests/test_qingping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/tests/test_thermopro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/tests/test_xiaomi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-04 13:31:51.000000 bluetooth-clocks-0.2.0/tox.ini
```

### Comparing `bluetooth-clocks-0.1.2/.coveragerc` & `bluetooth-clocks-0.2.0/.coveragerc`

 * *Files 13% similar despite different names*

```diff
@@ -22,7 +22,10 @@
     # Don't complain if tests don't hit defensive assertion code:
     raise AssertionError
     raise NotImplementedError
 
     # Don't complain if non-runnable code isn't run:
     if 0:
     if __name__ == .__main__.:
+
+    # Assume if TYPE_CHECKING is covered
+    if TYPE_CHECKING:
```

### Comparing `bluetooth-clocks-0.1.2/.github/workflows/ci.yml` & `bluetooth-clocks-0.2.0/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -60,16 +60,15 @@
 
   test:
     needs: prepare
     strategy:
       fail-fast: false
       matrix:
         python:
-        - "3.7"  # oldest Python supported by PSF
-        - "3.8"
+        - "3.8"  # oldest Python supported by PSF
         - "3.9"
         - "3.10"
         - "3.11"  # newest Python that is stable
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
```

### Comparing `bluetooth-clocks-0.1.2/.gitignore` & `bluetooth-clocks-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bluetooth-clocks-0.1.2/CHANGELOG.rst` & `bluetooth-clocks-0.2.0/CHANGELOG.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 =========
 Changelog
 =========
 
+Version 0.2.0: Get time from PVVX (2023-07-04)
+==============================================
+
+This release adds support for reading the time from devices with PVVX firmware.
+
+* Migrate code linting to Ruff, apply fixes by @koenvervloesem in https://github.com/koenvervloesem/bluetooth-clocks/pull/15
+* Add MJWSD05MMC and MHO-C122 to list of supported PVVX models by @koenvervloesem in https://github.com/koenvervloesem/bluetooth-clocks/pull/16
+* Assume if TYPE_CHECKING is covered by @koenvervloesem in https://github.com/koenvervloesem/bluetooth-clocks/pull/17
+* Deprecate Python 3.7 by @koenvervloesem in https://github.com/koenvervloesem/bluetooth-clocks/pull/18
+* Add read time command for PVVX firmware by @koenvervloesem in https://github.com/koenvervloesem/bluetooth-clocks/pull/19
+
 Version 0.1.2: Local time, please (2023-02-02)
 ==============================================
 
 This is a bugfix release. Previously the time on Qingping devices and devices running the PVVX ATC firmware was set to UTC instead of local time.
 
 * Autoupdate pre-commit by @koenvervloesem in https://github.com/koenvervloesem/bluetooth-clocks/pull/12
 * Fix local time on PVVX and Qingping devices by @koenvervloesem in https://github.com/koenvervloesem/bluetooth-clocks/pull/13
```

### Comparing `bluetooth-clocks-0.1.2/CONTRIBUTING.rst` & `bluetooth-clocks-0.2.0/CONTRIBUTING.rst`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
     tox -e docs
 
    Try running::
 
     tox -r -e docs
 
 #. Make sure to have a reliable |tox|_ installation that uses the correct
-   Python version (e.g., 3.7+). When in doubt you can run::
+   Python version (e.g., 3.8+). When in doubt you can run::
 
     tox --version
     # OR
     which tox
 
    If you have trouble and are seeing weird errors upon running |tox|_, you can
    also try to create a dedicated `virtual environment`_ with a |tox|_ binary
```

### Comparing `bluetooth-clocks-0.1.2/LICENSE.txt` & `bluetooth-clocks-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bluetooth-clocks-0.1.2/PKG-INFO` & `bluetooth-clocks-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetooth-clocks
-Version: 0.1.2
+Version: 0.2.0
 Summary: Set and get the time on various Bluetooth Low Energy clocks
 Home-page: https://github.com/koenvervloesem/bluetooth-clocks
 Author: Koen Vervloesem
 Author-email: koen@vervloesem.eu
 License: MIT
 Project-URL: Documentation, https://bluetooth-clocks.readthedocs.io/
 Project-URL: Source, https://github.com/koenvervloesem/bluetooth-clocks
@@ -19,23 +19,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 .. image:: https://github.com/koenvervloesem/bluetooth-clocks/workflows/tests/badge.svg
     :alt: Continuous Integration
     :target: https://github.com/koenvervloesem/bluetooth-clocks/actions
@@ -74,33 +73,32 @@
 .. inclusion-marker-after-intro
 
 Supported devices
 =================
 
 Bluetooth Clocks supports the following devices:
 
-+-------------------------+------------+-------------------+-----------+
-| Device                  | Set time   | Set 12/24h format | Read time |
-+=========================+============+===================+===========+
-| `Current Time Service`_ | Yes        | No                | Yes       |
-| (e.g. PineTime with     |            |                   |           |
-| InfiniTime firmware)    |            |                   |           |
-+-------------------------+------------+-------------------+-----------+
-| `PVVX firmware`_        | Yes        | No                | No        |
-| (LYWSD03MMC, MHO-C401,  |            |                   | (not yet) |
-| CGG1, CGDK2)            |            |                   |           |
-+-------------------------+------------+-------------------+-----------+
-| Qingping BT Clock Lite  | Yes        | No                | No        |
-+-------------------------+------------+-------------------+-----------+
-| ThermoPro TP358         | Yes        | Yes               | No        |
-+-------------------------+------------+-------------------+-----------+
-| ThermoPro TP393         | Yes        | Yes               | No        |
-+-------------------------+------------+-------------------+-----------+
-| Xiaomi LYWSD02          | Yes        | No                | Yes       |
-+-------------------------+------------+-------------------+-----------+
++--------------------------+------------+-------------------+-----------+
+| Device                   | Set time   | Set 12/24h format | Read time |
++==========================+============+===================+===========+
+| `Current Time Service`_  | Yes        | No                | Yes       |
+| (e.g. PineTime with      |            |                   |           |
+| InfiniTime firmware)     |            |                   |           |
++--------------------------+------------+-------------------+-----------+
+| `PVVX firmware`_         | Yes        | No                | Yes       |
+| (LYWSD03MMC, MHO-C401,   |            |                   |           |
+| CGG1, CGDK2, MJWSD05MMC, |            |                   |           |
+| MHO-C122)                |            |                   |           |
++--------------------------+------------+-------------------+-----------+
+| Qingping BT Clock Lite   | Yes        | No                | No        |
++--------------------------+------------+-------------------+-----------+
+| ThermoPro TP358/TP393    | Yes        | Yes               | No        |
++--------------------------+------------+-------------------+-----------+
+| Xiaomi LYWSD02           | Yes        | No                | Yes       |
++--------------------------+------------+-------------------+-----------+
 
 .. _Current Time Service: https://www.bluetooth.com/specifications/specs/current-time-service-1-1/
 .. _PVVX firmware: https://github.com/pvvx/ATC_MiThermometer
 
 .. inclusion-marker-before-installation
 
 Installation
```

### Comparing `bluetooth-clocks-0.1.2/README.rst` & `bluetooth-clocks-0.2.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -36,33 +36,32 @@
 .. inclusion-marker-after-intro
 
 Supported devices
 =================
 
 Bluetooth Clocks supports the following devices:
 
-+-------------------------+------------+-------------------+-----------+
-| Device                  | Set time   | Set 12/24h format | Read time |
-+=========================+============+===================+===========+
-| `Current Time Service`_ | Yes        | No                | Yes       |
-| (e.g. PineTime with     |            |                   |           |
-| InfiniTime firmware)    |            |                   |           |
-+-------------------------+------------+-------------------+-----------+
-| `PVVX firmware`_        | Yes        | No                | No        |
-| (LYWSD03MMC, MHO-C401,  |            |                   | (not yet) |
-| CGG1, CGDK2)            |            |                   |           |
-+-------------------------+------------+-------------------+-----------+
-| Qingping BT Clock Lite  | Yes        | No                | No        |
-+-------------------------+------------+-------------------+-----------+
-| ThermoPro TP358         | Yes        | Yes               | No        |
-+-------------------------+------------+-------------------+-----------+
-| ThermoPro TP393         | Yes        | Yes               | No        |
-+-------------------------+------------+-------------------+-----------+
-| Xiaomi LYWSD02          | Yes        | No                | Yes       |
-+-------------------------+------------+-------------------+-----------+
++--------------------------+------------+-------------------+-----------+
+| Device                   | Set time   | Set 12/24h format | Read time |
++==========================+============+===================+===========+
+| `Current Time Service`_  | Yes        | No                | Yes       |
+| (e.g. PineTime with      |            |                   |           |
+| InfiniTime firmware)     |            |                   |           |
++--------------------------+------------+-------------------+-----------+
+| `PVVX firmware`_         | Yes        | No                | Yes       |
+| (LYWSD03MMC, MHO-C401,   |            |                   |           |
+| CGG1, CGDK2, MJWSD05MMC, |            |                   |           |
+| MHO-C122)                |            |                   |           |
++--------------------------+------------+-------------------+-----------+
+| Qingping BT Clock Lite   | Yes        | No                | No        |
++--------------------------+------------+-------------------+-----------+
+| ThermoPro TP358/TP393    | Yes        | Yes               | No        |
++--------------------------+------------+-------------------+-----------+
+| Xiaomi LYWSD02           | Yes        | No                | Yes       |
++--------------------------+------------+-------------------+-----------+
 
 .. _Current Time Service: https://www.bluetooth.com/specifications/specs/current-time-service-1-1/
 .. _PVVX firmware: https://github.com/pvvx/ATC_MiThermometer
 
 .. inclusion-marker-before-installation
 
 Installation
```

### Comparing `bluetooth-clocks-0.1.2/docs/Makefile` & `bluetooth-clocks-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bluetooth-clocks-0.1.2/docs/_static/synchronized-clocks.jpg` & `bluetooth-clocks-0.2.0/docs/_static/synchronized-clocks.jpg`

 * *Files identical despite different names*

### Comparing `bluetooth-clocks-0.1.2/docs/conf.py` & `bluetooth-clocks-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bluetooth-clocks-0.1.2/docs/index.rst` & `bluetooth-clocks-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bluetooth-clocks-0.1.2/setup.cfg` & `bluetooth-clocks-0.2.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Utilities
@@ -38,18 +37,17 @@
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	bleak>=0.19.0
-	importlib-metadata; python_version<"3.8"
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
@@ -75,43 +73,14 @@
 	.tox
 testpaths = tests
 
 [devpi:upload]
 no_vcs = 1
 formats = bdist_wheel
 
-[flake8]
-max_line_length = 88
-docstring-convention = google
-rst-roles = 
-	class,
-	func,
-	ref,
-	meth,
-	mod,
-	obj,
-rst-directives = 
-	envvar,
-	exception,
-rst-substitutions = 
-	version,
-extend_ignore = E203, W503
-	RST307,
-	RST201,RST203,RST301,
-	ANN101,ANN102,
-	E501, W505,
-	PAR101,
-exclude = 
-	.tox
-	build
-	dist
-	.eggs
-	docs/conf.py
-pytest-parametrize-names-type = csv
-
 [pyscaffold]
 version = 4.3.1
 package = bluetooth_clocks
 extensions = 
 	github_actions
 	pre_commit
```

### Comparing `bluetooth-clocks-0.1.2/setup.py` & `bluetooth-clocks-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Learn more under: https://pyscaffold.org/
 """
 from setuptools import setup
 
 if __name__ == "__main__":
     try:
         setup(use_scm_version={"version_scheme": "no-guess-dev"})
-    except:  # noqa
+    except:
         print(
             "\n\nAn error occurred while building the project, "
             "please ensure you have the most updated version of setuptools, "
             "setuptools_scm and wheel with:\n"
-            "   pip install -U setuptools setuptools_scm wheel\n\n"
+            "   pip install -U setuptools setuptools_scm wheel\n\n",
         )
         raise
```

### Comparing `bluetooth-clocks-0.1.2/src/bluetooth_clocks/__init__.py` & `bluetooth-clocks-0.2.0/src/bluetooth_clocks/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,38 +2,37 @@
 
 This project offers a way to easily recognize Bluetooth Low Energy clocks from their
 advertisements and has a device-independent API to set and get the time on them.
 """
 from __future__ import annotations
 
 import logging
-import sys
 from abc import ABC, abstractmethod
 from importlib import import_module
+from importlib.metadata import PackageNotFoundError, version  # pragma: no cover
 from inspect import isclass
 from pathlib import Path
 from pkgutil import iter_modules
 from time import time
-from typing import ClassVar, Type  # noqa: F401
-from uuid import UUID
+from typing import TYPE_CHECKING, ClassVar
+
+if TYPE_CHECKING:
+    from uuid import UUID
 
 from bleak import BleakClient
-from bleak.backends.device import BLEDevice
-from bleak.backends.scanner import AdvertisementData
 
-from bluetooth_clocks.exceptions import TimeNotReadableError, UnsupportedDeviceError
+if TYPE_CHECKING:
+    from bleak.backends.device import BLEDevice
+    from bleak.backends.scanner import AdvertisementData
 
-if sys.version_info[:2] >= (3, 8):
-    from importlib.metadata import PackageNotFoundError, version  # pragma: no cover
-else:
-    from importlib_metadata import PackageNotFoundError, version  # pragma: no cover
+from bluetooth_clocks.exceptions import TimeNotReadableError, UnsupportedDeviceError
 
 try:
     # Change here if project is renamed and does not equal the package name
-    dist_name = "bluetooth-clocks"  # pylint: disable=invalid-name
+    dist_name = "bluetooth-clocks"
     __version__ = version(dist_name)
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
 finally:
     del version, PackageNotFoundError
 
 _logger = logging.getLogger(__name__)
@@ -79,41 +78,41 @@
 
     Attributes:
         address (str): The Bluetooth address of the device.
         name (str | None): The name of the device, or ``None`` if it doesn't
           have a name.
     """
 
-    DEVICE_TYPE: ClassVar[str]  # noqa: CCE001
+    DEVICE_TYPE: ClassVar[str]
     """The name of the device type."""
 
-    SERVICE_UUID: ClassVar[UUID]  # noqa: CCE001
+    SERVICE_UUID: ClassVar[UUID]
     """The UUID of the service used to read/write the time."""
 
-    CHAR_UUID: ClassVar[UUID]  # noqa: CCE001
+    CHAR_UUID: ClassVar[UUID]
     """The UUID of the characteristic used to read/write the time."""
 
-    TIME_GET_FORMAT: ClassVar[str | None]  # noqa: CCE001
+    TIME_GET_FORMAT: ClassVar[str | None]
     """The format string to convert bytes read from the device to a time.
 
     This is ``None`` if the device doesn't support reading the time.
     """
 
-    TIME_SET_FORMAT: ClassVar[str]  # noqa: CCE001
+    TIME_SET_FORMAT: ClassVar[str]
     """The format string to convert a time to bytes written to the device."""
 
-    WRITE_WITH_RESPONSE: ClassVar[bool]  # noqa: CCE001
+    WRITE_WITH_RESPONSE: ClassVar[bool]
     """``True`` if the bytes to set the time should use write with response."""
 
-    LOCAL_NAME: ClassVar[str | None]  # noqa: CCE001
+    LOCAL_NAME: ClassVar[str | None]
     """The local name used to recognize this type of device.
 
     This is ``None`` if the local name isn't used to recognize the device."""
 
-    LOCAL_NAME_STARTS_WITH: ClassVar[bool | None]  # noqa: CCE001
+    LOCAL_NAME_STARTS_WITH: ClassVar[bool | None]
     """Whether the local name should start with `LOCAL_NAME`.
 
     ``True`` if the start of `LOCAL_NAME` is used to recognize this type of device.
     ``False`` if the local name should exactly match `LOCAL_NAME`.
     This is ``None`` if the local name isn't used to recognize the device.
     """
 
@@ -124,15 +123,17 @@
             device (BLEDevice): The Bluetooth device.
         """
         self.address = device.address
         self.name = device.name
 
     @classmethod
     def create_from_advertisement(
-        cls, device: BLEDevice, advertisement_data: AdvertisementData
+        cls,
+        device: BLEDevice,
+        advertisement_data: AdvertisementData,
     ) -> BluetoothClock:
         """Create object of a :class:`BluetoothClock` subclass from advertisement data.
 
         This is a factory method that you use if you don't know the exact device type
         beforehand. This method automatically recognizes the device type and creates
         an object of the corresponding subclass.
 
@@ -171,15 +172,15 @@
             False
         """
         return bool(cls.TIME_GET_FORMAT)
 
     @classmethod
     def recognize(
         cls,
-        device: BLEDevice,  # pylint: disable=unused-argument
+        device: BLEDevice,
         advertisement_data: AdvertisementData,
     ) -> bool:
         """Recognize this device type from advertisement data.
 
         By default this checks whether the advertisement data has a local name
         that is equal to or starts with `LOCAL_NAME`, by calling
         :meth:`recognize_from_local_name`.
@@ -242,17 +243,15 @@
             # The device doesn't advertise a local name
             # or the device type can't be recognized by its local name.
             return False
         if cls.LOCAL_NAME_STARTS_WITH:
             return local_name.startswith(cls.LOCAL_NAME)
         return local_name == cls.LOCAL_NAME
 
-    def get_time_from_bytes(  # pylint: disable=unused-argument
-        self, time_bytes: bytes
-    ) -> float:
+    def get_time_from_bytes(self, time_bytes: bytes) -> float:
         """Convert bytes read from a device to a timestamp.
 
         Override this method in a subclass for a device that supports getting the time.
 
         Args:
             time_bytes (bytes): The raw bytes read from the device.
 
@@ -263,20 +262,20 @@
         Returns:
             float: The time encoded as a Unix timestamp.
 
         Example:
             >>> from bluetooth_clocks.devices.xiaomi import LYWSD02
             >>> from bleak.backends.device import BLEDevice
             >>> from datetime import datetime
-            >>> clock = LYWSD02(BLEDevice("E7:2E:00:B1:38:96"))
+            >>> clock = LYWSD02(BLEDevice("E7:2E:00:B1:38:96", "", {}, -67))
             >>> timestamp = clock.get_time_from_bytes(
             ...             bytes([0xdd, 0xbc, 0xb9, 0x63, 0x00]))
             >>> print(datetime.utcfromtimestamp(timestamp).strftime("%Y-%m-%d %H:%M:%S"))
             2023-01-07 18:41:33
-        """
+        """  # noqa: E501
         raise TimeNotReadableError
 
     @abstractmethod
     def get_bytes_from_time(self, timestamp: float, ampm: bool = False) -> bytes:
         """Generate the bytes to set the time on this device.
 
         Override this method in a subclass to implement the device's time format.
@@ -290,15 +289,15 @@
         Returns:
             bytes: The bytes needed to set the time of the device to `timestamp`.
 
         Example:
             >>> from bluetooth_clocks.devices.thermopro import TP393
             >>> from bleak.backends.device import BLEDevice
             >>> from datetime import datetime
-            >>> clock = TP393(BLEDevice("10:76:36:14:2A:3D"))
+            >>> clock = TP393(BLEDevice("10:76:36:14:2A:3D", "TP393 (2A3D)", {}, -67))
             >>> timestamp = datetime.fromisoformat("2023-01-07 17:32:50").timestamp()
             >>> clock.get_bytes_from_time(timestamp, ampm=True).hex()
             'a517010711203206005a'
         """
 
     async def get_time(self) -> float:
         """Get the time of the Bluetooth clock.
@@ -317,15 +316,17 @@
         async with BleakClient(self.address) as client:
             service = client.services.get_service(self.SERVICE_UUID)
             characteristic = service.get_characteristic(self.CHAR_UUID)
             time_bytes = await client.read_gatt_char(characteristic)
             return self.get_time_from_bytes(time_bytes)
 
     async def set_time(
-        self, timestamp: float | None = None, ampm: bool = False
+        self,
+        timestamp: float | None = None,
+        ampm: bool = False,
     ) -> None:
         """Set the time of the Bluetooth clock.
 
         Args:
             timestamp (float | None = None): The timestamp to write to the clock. If
               this is ``None``, the current time is used.
             ampm (bool): ``True`` if the device should show the time with AM/PM,
@@ -343,15 +344,15 @@
                 self.get_bytes_from_time(timestamp, ampm),
                 response=self.WRITE_WITH_RESPONSE,
             )
 
 
 # Iterate through the modules in the module `device`.
 package_dir = Path(__file__).resolve().parent / "devices"
-for _, module_name, _ in iter_modules([str(package_dir)]):  # type: ignore
+for _, module_name, _ in iter_modules([str(package_dir)]):  # type: ignore[assignment]
     # Import the module and iterate through its attributes
     module = import_module(f"{__name__}.devices.{module_name}")
     for attribute_name in dir(module):
         attribute = getattr(module, attribute_name)
 
         if isclass(attribute) and hasattr(attribute, "DEVICE_TYPE"):
             _supported_devices.append(attribute)
```

### Comparing `bluetooth-clocks-0.1.2/src/bluetooth_clocks/__main__.py` & `bluetooth-clocks-0.2.0/src/bluetooth_clocks/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,28 +75,30 @@
     )
 
     subparsers = parser.add_subparsers(title="Subcommands")
     subparsers.required = True
 
     # Parser for the "discover" subcommand
     parser_discover = subparsers.add_parser(
-        "discover", help="discover supported Bluetooth clocks"
+        "discover",
+        help="discover supported Bluetooth clocks",
     )
     parser_discover.add_argument(
         "-s",
         "--scan-duration",
         type=float,
         default=5.0,
         help="scan duration (default: 5 seconds)",
     )
     parser_discover.set_defaults(func=discover)
 
     # Parser for the "get" subcommand
     parser_get = subparsers.add_parser(
-        "get", help="get the time from a Bluetooth clock"
+        "get",
+        help="get the time from a Bluetooth clock",
     )
     parser_get.add_argument(
         "-a",
         "--address",
         help="Bluetooth address (e.g. 12:34:56:78:9A:BC)",
         required=True,
     )
@@ -124,15 +126,15 @@
         default=5.0,
         help="scan duration (default: 5 seconds)",
     )
     parser_set.add_argument(
         "-t",
         "--time",
         type=str,
-        help="the time to set, in ISO 8601 format (e.g. 2023-01-10T16:20, default: current time)",
+        help="the time to set, in ISO 8601 format (e.g. 2023-01-10T16:20, default: current time)",  # noqa: E501
     )
     parser_set.add_argument(
         "-p",
         "--am-pm",
         help="use AM/PM format (default: 24-hour format)",
         action="store_true",
     )
@@ -146,15 +148,18 @@
     """Setup basic logging.
 
     Args:
       loglevel (int): minimum loglevel for emitting messages
     """
     logformat = "[%(asctime)s] %(levelname)s:%(name)s:%(message)s"
     logging.basicConfig(
-        level=loglevel, stream=sys.stdout, format=logformat, datefmt="%Y-%m-%d %H:%M:%S"
+        level=loglevel,
+        stream=sys.stdout,
+        format=logformat,
+        datefmt="%Y-%m-%d %H:%M:%S",
     )
 
 
 async def discover(args: Namespace) -> None:
     """Discover Bluetooth clocks."""
     found_clock = False
```

### Comparing `bluetooth-clocks-0.1.2/src/bluetooth_clocks/devices/current_time_service.py` & `bluetooth-clocks-0.2.0/src/bluetooth_clocks/devices/current_time_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 This includes the PineTime with InfiniTime firmware.
 """
 from __future__ import annotations
 
 import struct
 from datetime import datetime
+from typing import TYPE_CHECKING
 from uuid import UUID
 
-from bleak.backends.device import BLEDevice
-from bleak.backends.scanner import AdvertisementData
+if TYPE_CHECKING:
+    from bleak.backends.device import BLEDevice
+    from bleak.backends.scanner import AdvertisementData
 
 from bluetooth_clocks import MICROSECONDS, BluetoothClock
 from bluetooth_clocks.exceptions import InvalidTimeBytesError
 
 
 class CurrentTimeService(BluetoothClock):
     """Bluetooth clock support for devices implementing the Current Time Service.
@@ -38,15 +40,17 @@
     This starts with an unsigned short in little-endian format, followed by eight bytes.
     """
     WRITE_WITH_RESPONSE = True
     """Writing the time to the Current Time Service needs write with response."""
 
     @classmethod
     def recognize(
-        cls, device: BLEDevice, advertisement_data: AdvertisementData
+        cls,
+        device: BLEDevice,
+        advertisement_data: AdvertisementData,
     ) -> bool:
         """Recognize the Current Time Service from advertisement data.
 
         This checks whether the Current Time Service's service UUID is in the list
         of advertised service UUIDs.
 
         Args:
@@ -91,15 +95,19 @@
                 second=second,
                 microsecond=int(fractions256 / 256 * MICROSECONDS),
             )
         except struct.error as exception:
             raise InvalidTimeBytesError(time_bytes) from exception
         return date_time.timestamp()
 
-    def get_bytes_from_time(self, timestamp: float, ampm: bool = False) -> bytes:
+    def get_bytes_from_time(
+        self,
+        timestamp: float,
+        ampm: bool = False,
+    ) -> bytes:
         """Generate the bytes to set the time on the Current Time Service.
 
         Args:
             timestamp (float): The time encoded as a Unix timestamp.
             ampm (bool): ``True`` if the device should show the time with AM/PM,
                 ``False`` if it should use 24-hour format. The Current Time Service
                 ignores this argument, as it doesn't support this option.
@@ -130,15 +138,17 @@
     """The local name used to recognize this type of device."""
 
     LOCAL_NAME_STARTS_WITH = False
     """The local name should exactly match `LOCAL_NAME`."""
 
     @classmethod
     def recognize(
-        cls, device: BLEDevice, advertisement_data: AdvertisementData
+        cls,
+        device: BLEDevice,
+        advertisement_data: AdvertisementData,
     ) -> bool:
         """Recognize the PineTime with InfiniTime firmware from advertisement data.
 
         This checks whether the advertisement data has a local name that is equal
         to or starts with `LOCAL_NAME`.
 
         Args:
```

### Comparing `bluetooth-clocks-0.1.2/src/bluetooth_clocks/devices/pvvx.py` & `bluetooth-clocks-0.2.0/tests/test_bluetooth_clock.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,80 @@
-"""Bluetooth clock support for devices running the PVVX firmware."""
-from __future__ import annotations
-
-import struct
-from time import localtime
-from uuid import UUID
-
+"""Test the BluetoothClock abstract class."""
+import pytest
 from bleak.backends.device import BLEDevice
 from bleak.backends.scanner import AdvertisementData
 
-from bluetooth_clocks import BluetoothClock
-
-
-class PVVX(BluetoothClock):
-    """Bluetooth clock support for devices running the PVVX firmware."""
-
-    DEVICE_TYPE = "PVVX"
-    SERVICE_UUID = UUID("00001f10-0000-1000-8000-00805f9b34fb")
-    CHAR_UUID = UUID("00001f1f-0000-1000-8000-00805f9b34fb")
-
-    TIME_GET_FORMAT = None
-    """The PVVX firmware doesn't support reading the time."""
-
-    TIME_SET_FORMAT = "<BL"
-    """The format string to convert a time to bytes written to the PVVX device."""
-
-    WRITE_WITH_RESPONSE = False
-    """Writing the time to the PVVX device needs write without response."""
-
-    SERVICE_DATA_UUID = UUID("0000181a-0000-1000-8000-00805f9b34fb")
-    """UUID of the service data the PVVX device is advertising."""
-
-    @classmethod
-    def recognize(
-        cls, device: BLEDevice, advertisement_data: AdvertisementData
-    ) -> bool:
-        """Recognize the PVVX device from advertisement data.
-
-        This checks whether the advertisement has service data with service UUID
-        0x181a (PVVX custom format).
-
-        Args:
-            device (~bleak.backends.device.BLEDevice): The Bluetooth device.
-            advertisement_data (AdvertisementData): The advertisement data.
-
-        Returns:
-            bool: ``True`` if the device is recognized as a PVVX device,
-            ``False`` otherwise.
-        """
-        return str(cls.SERVICE_DATA_UUID) in advertisement_data.service_data
-
-    def get_bytes_from_time(self, timestamp: float, ampm: bool = False) -> bytes:
-        """Generate the bytes to set the time on the PVVX device.
-
-        Args:
-            timestamp (float): The time encoded as a Unix timestamp.
-            ampm (bool): ``True`` if the device should show the time with AM/PM,
-                ``False`` if it should use 24-hour format. The PVVX device
-                ignores this argument, as it doesn't support this option.
-
-        Returns:
-            bytes: The bytes needed to set the time of the device to `timestamp`.
-        """
-        # Convert timestamp to little-endian unsigned long integer
-        # And add header byte
-        return struct.pack(
-            self.TIME_SET_FORMAT,
-            0x23,
-            int(timestamp + localtime(timestamp).tm_gmtoff),
+from bluetooth_clocks import BluetoothClock, supported_devices
+from bluetooth_clocks.devices.xiaomi import LYWSD02
+from bluetooth_clocks.exceptions import UnsupportedDeviceError
+
+__author__ = "Koen Vervloesem"
+__copyright__ = "Koen Vervloesem"
+__license__ = "MIT"
+
+
+def test_supported_devices() -> None:
+    """Test whether the list of supported devices isn't empty."""
+    assert supported_devices()
+
+
+def test_create_from_advertisement() -> None:
+    """Test whether an object of the right subclass is created from an advertisement."""
+    assert isinstance(
+        BluetoothClock.create_from_advertisement(
+            BLEDevice("E7:2E:00:B1:38:96", "LYWSD02", {}, -67),
+            AdvertisementData(
+                local_name="LYWSD02",
+                manufacturer_data={},
+                platform_data=(),
+                rssi=-67,
+                service_data={
+                    "0000fe95-0000-1000-8000-00805f9b34fb": bytes(
+                        [
+                            0x70,
+                            0x20,
+                            0x5B,
+                            0x04,
+                            0x27,
+                            0x96,
+                            0x38,
+                            0xB1,
+                            0x00,
+                            0x2E,
+                            0xE7,
+                            0x09,
+                            0x04,
+                            0x10,
+                            0x02,
+                            0xD5,
+                            0x00,
+                        ],
+                    ),
+                },
+                service_uuids=[
+                    "0000181a-0000-1000-8000-00805f9b34fb",
+                    "0000fef5-0000-1000-8000-00805f9b34fb",
+                ],
+                tx_power=0,
+            ),
+        ),
+        LYWSD02,
+    )
+
+
+def test_create_from_advertisement_unknown() -> None:
+    """Test whether no subclass is created from an unknown advertisement."""
+    with pytest.raises(UnsupportedDeviceError):
+        BluetoothClock.create_from_advertisement(
+            BLEDevice("45:B4:07:8A:66:6A", "", {}, -67),
+            AdvertisementData(
+                local_name=None,
+                manufacturer_data={
+                    0x004C: bytes([0x10, 0x05, 0x47, 0x1C, 0x7F, 0xF1, 0x93]),
+                },
+                platform_data=(),
+                rssi=-67,
+                service_data={},
+                service_uuids=[],
+                tx_power=0,
+            ),
         )
```

### Comparing `bluetooth-clocks-0.1.2/src/bluetooth_clocks/devices/qingping.py` & `bluetooth-clocks-0.2.0/src/bluetooth_clocks/devices/qingping.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,22 +36,26 @@
 
     LOCAL_NAME = "Qingping BT Clock Lite"
     """The local name used to recognize this type of device."""
 
     LOCAL_NAME_STARTS_WITH = False
     """The local name should exactly match `LOCAL_NAME`."""
 
-    def get_bytes_from_time(self, timestamp: float, ampm: bool = False) -> bytes:
+    def get_bytes_from_time(
+        self,
+        timestamp: float,
+        ampm: bool = False,
+    ) -> bytes:
         """Generate the bytes to set the time on the Qingping BT Clock Lite.
 
         Args:
             timestamp (float): The time encoded as a Unix timestamp.
             ampm (bool): ``True`` if the device should show the time with AM/PM,
                 ``False`` if it should use 24-hour format. The Qingping BT Clock
-                Lite ignores this argument, as it doesn’t support this option.
+                Lite ignores this argument, as it doesn`t support this option.
 
         Returns:
             bytes: The bytes needed to set the time of the device to `timestamp`.
         """
         return pack(
             self.TIME_SET_FORMAT,
             0x05,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bluetooth-clocks-0.1.2/src/bluetooth_clocks/devices/thermopro.py` & `bluetooth-clocks-0.2.0/src/bluetooth_clocks/devices/thermopro.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     SERVICE_UUID = UUID("00010203-0405-0607-0809-0a0b0c0d1910")
     """The UUID of the service used to write the time."""
 
     CHAR_UUID = UUID("00010203-0405-0607-0809-0a0b0c0d2b11")
     """The UUID of the characteristic used to write the time."""
 
     TIME_GET_FORMAT = None
-    """ThermoPro devices don’t support reading the time."""
+    """ThermoPro devices don`t support reading the time."""
 
     TIME_SET_FORMAT = "BBBBBBBBBB"
     """The format string to convert a time to bytes written to the device.
 
     These are ten bytes.
     """
 
@@ -57,26 +57,26 @@
             date_time.second,
             date_time.weekday() + 1,  # Monday-Sunday -> 0-6
             int(not ampm),
             0x5A,
         )
 
 
-class TP358(TPXXX):  # pylint: disable=too-few-public-methods
+class TP358(TPXXX):
     """Bluetooth clock support for the ThermoPro TP358."""
 
     DEVICE_TYPE = "ThermoPro TP358"
     LOCAL_NAME = "TP358"
     """The local name used to recognize this type of device."""
 
     LOCAL_NAME_STARTS_WITH = True
     """The local name should start with `LOCAL_NAME`."""
 
 
-class TP393(TPXXX):  # pylint: disable=too-few-public-methods
+class TP393(TPXXX):
     """Bluetooth clock support for the ThermoPro TP393."""
 
     DEVICE_TYPE = "ThermoPro TP393"
     LOCAL_NAME = "TP393"
     """The local name used to recognize this type of device."""
 
     LOCAL_NAME_STARTS_WITH = True
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bluetooth-clocks-0.1.2/src/bluetooth_clocks/devices/xiaomi.py` & `bluetooth-clocks-0.2.0/src/bluetooth_clocks/devices/xiaomi.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,19 @@
         """
         try:
             time_time, _ = struct.unpack(self.TIME_GET_FORMAT, time_bytes)
         except struct.error as exception:
             raise InvalidTimeBytesError(time_bytes) from exception
         return float(time_time)
 
-    def get_bytes_from_time(self, timestamp: float, ampm: bool = False) -> bytes:
+    def get_bytes_from_time(
+        self,
+        timestamp: float,
+        ampm: bool = False,
+    ) -> bytes:
         """Generate the bytes to set the time on the Xiaomi LYWSD02.
 
         Args:
             timestamp (float): The time encoded as a Unix timestamp.
             ampm (bool): ``True`` if the device should show the time with AM/PM,
                 ``False`` if it should use 24-hour format. The Xiaomi LYWSD02
                 ignores this argument, as it doesn't support this option.
```

### Comparing `bluetooth-clocks-0.1.2/src/bluetooth_clocks/exceptions.py` & `bluetooth-clocks-0.2.0/src/bluetooth_clocks/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 
 
 class InvalidTimeBytesError(BluetoothClocksError):
     """Exception raised when bytes read from a device don't have the right format."""
 
 
 class TimeNotReadableError(BluetoothClocksError):
-    """Exception raised when trying to read the time on a device that doesn't support this."""
+    """Exception raised when reading the time on a device that doesn't support this."""
 
 
 class UnsupportedDeviceError(BluetoothClocksError):
     """Exception raised when a device is not supported."""
```

### Comparing `bluetooth-clocks-0.1.2/src/bluetooth_clocks/scanners.py` & `bluetooth-clocks-0.2.0/src/bluetooth_clocks/scanners.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Module with functions to scan for Bluetooth clocks."""
 from __future__ import annotations
 
 import asyncio
 import logging
-from typing import Callable
+from typing import TYPE_CHECKING, Callable
 
 from bleak import BleakScanner
-from bleak.backends.device import BLEDevice
-from bleak.backends.scanner import AdvertisementData
+
+if TYPE_CHECKING:
+    from bleak.backends.device import BLEDevice
+    from bleak.backends.scanner import AdvertisementData
 
 from bluetooth_clocks import BluetoothClock, supported_devices
 from bluetooth_clocks.exceptions import UnsupportedDeviceError
 
 _logger = logging.getLogger(__name__)
 
 
@@ -20,47 +22,53 @@
 
     Args:
         address (str): The Bluetooth address of the device.
         scan_duration (float): The scan duration for finding the device. Defaults to
           5 seconds.
 
     Raises:
-        UnsupportedDeviceError: If the device with address `address` isn’t
+        UnsupportedDeviceError: If the device with address `address` isn`t
           supported.
 
     Returns:
         BluetoothClock | None: A :class:`BluetoothClock` object for the device, or
         ``None`` if the device isn't found.
     """
     found_clock = None
 
     def device_found(device: BLEDevice, advertisement_data: AdvertisementData) -> None:
         """Try to recognize device as a Bluetooth clock."""
         nonlocal found_clock
         if device.address == address:
-            _logger.info(f"Device with address {address} found")
+            _logger.info(
+                "Device with address {address} found",
+                extra={"address": address},
+            )
             found_clock = BluetoothClock.create_from_advertisement(
-                device, advertisement_data
+                device,
+                advertisement_data,
             )
             _logger.info(
-                f"Device with address {address} recognized as {found_clock.DEVICE_TYPE}"
+                "Device with address {address} recognized as {device_type}",
+                extra={"address": address, "device_type": found_clock.DEVICE_TYPE},
             )
 
     scanner = BleakScanner(detection_callback=device_found)
 
     _logger.info("Scanning for device...")
     await scanner.start()
     await asyncio.sleep(scan_duration)
     await scanner.stop()
 
-    return found_clock  # noqa: R504
+    return found_clock
 
 
 async def discover_clocks(
-    callback: Callable[[BluetoothClock], None], scan_duration: float = 5.0
+    callback: Callable[[BluetoothClock], None],
+    scan_duration: float = 5.0,
 ) -> None:
     """Discover Bluetooth clocks.
 
     Args:
         callback (Callable[[BluetoothClock], None]): Function to call when a clock
           has been discovered. This function gets passed the discovered
           :class:`BluetoothClock` object as its argument.
@@ -72,28 +80,42 @@
     def device_found(device: BLEDevice, advertisement_data: AdvertisementData) -> None:
         """Call callback if we recognize a found device as a clock."""
         nonlocal found_addresses
         address = device.address
         if address not in found_addresses:
             try:
                 clock = BluetoothClock.create_from_advertisement(
-                    device, advertisement_data
+                    device,
+                    advertisement_data,
                 )
                 name = advertisement_data.local_name
                 clock_type = clock.DEVICE_TYPE
-                _logger.info(f"Found a {clock_type}: address {address}, name {name}")
+                _logger.info(
+                    "Found a {clock_type}: address {address}, name {device_name}",
+                    extra={
+                        "clock_type": clock_type,
+                        "address": address,
+                        "device_name": name,
+                    },
+                )
                 callback(clock)
             except UnsupportedDeviceError:
                 # Just ignore devices we don't recognize as a clock.
                 pass
             finally:
                 # Don't try to recognize the device with the same address again.
                 found_addresses.append(address)
 
-    _logger.info(f"Supported devices: {', '.join(supported_devices())}")
+    _logger.info(
+        "Supported devices: {devices}",
+        extra={"devices": ", ".join(supported_devices())},
+    )
     scanner = BleakScanner(detection_callback=device_found)
 
-    _logger.info(f"Scanning for supported clocks for {scan_duration} seconds...")
+    _logger.info(
+        "Scanning for supported clocks for {scan_duration} seconds...",
+        extra={"scan_duration": scan_duration},
+    )
 
     await scanner.start()
     await asyncio.sleep(scan_duration)
     await scanner.stop()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bluetooth-clocks-0.1.2/src/bluetooth_clocks.egg-info/PKG-INFO` & `bluetooth-clocks-0.2.0/src/bluetooth_clocks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetooth-clocks
-Version: 0.1.2
+Version: 0.2.0
 Summary: Set and get the time on various Bluetooth Low Energy clocks
 Home-page: https://github.com/koenvervloesem/bluetooth-clocks
 Author: Koen Vervloesem
 Author-email: koen@vervloesem.eu
 License: MIT
 Project-URL: Documentation, https://bluetooth-clocks.readthedocs.io/
 Project-URL: Source, https://github.com/koenvervloesem/bluetooth-clocks
@@ -19,23 +19,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 .. image:: https://github.com/koenvervloesem/bluetooth-clocks/workflows/tests/badge.svg
     :alt: Continuous Integration
     :target: https://github.com/koenvervloesem/bluetooth-clocks/actions
@@ -74,33 +73,32 @@
 .. inclusion-marker-after-intro
 
 Supported devices
 =================
 
 Bluetooth Clocks supports the following devices:
 
-+-------------------------+------------+-------------------+-----------+
-| Device                  | Set time   | Set 12/24h format | Read time |
-+=========================+============+===================+===========+
-| `Current Time Service`_ | Yes        | No                | Yes       |
-| (e.g. PineTime with     |            |                   |           |
-| InfiniTime firmware)    |            |                   |           |
-+-------------------------+------------+-------------------+-----------+
-| `PVVX firmware`_        | Yes        | No                | No        |
-| (LYWSD03MMC, MHO-C401,  |            |                   | (not yet) |
-| CGG1, CGDK2)            |            |                   |           |
-+-------------------------+------------+-------------------+-----------+
-| Qingping BT Clock Lite  | Yes        | No                | No        |
-+-------------------------+------------+-------------------+-----------+
-| ThermoPro TP358         | Yes        | Yes               | No        |
-+-------------------------+------------+-------------------+-----------+
-| ThermoPro TP393         | Yes        | Yes               | No        |
-+-------------------------+------------+-------------------+-----------+
-| Xiaomi LYWSD02          | Yes        | No                | Yes       |
-+-------------------------+------------+-------------------+-----------+
++--------------------------+------------+-------------------+-----------+
+| Device                   | Set time   | Set 12/24h format | Read time |
++==========================+============+===================+===========+
+| `Current Time Service`_  | Yes        | No                | Yes       |
+| (e.g. PineTime with      |            |                   |           |
+| InfiniTime firmware)     |            |                   |           |
++--------------------------+------------+-------------------+-----------+
+| `PVVX firmware`_         | Yes        | No                | Yes       |
+| (LYWSD03MMC, MHO-C401,   |            |                   |           |
+| CGG1, CGDK2, MJWSD05MMC, |            |                   |           |
+| MHO-C122)                |            |                   |           |
++--------------------------+------------+-------------------+-----------+
+| Qingping BT Clock Lite   | Yes        | No                | No        |
++--------------------------+------------+-------------------+-----------+
+| ThermoPro TP358/TP393    | Yes        | Yes               | No        |
++--------------------------+------------+-------------------+-----------+
+| Xiaomi LYWSD02           | Yes        | No                | Yes       |
++--------------------------+------------+-------------------+-----------+
 
 .. _Current Time Service: https://www.bluetooth.com/specifications/specs/current-time-service-1-1/
 .. _PVVX firmware: https://github.com/pvvx/ATC_MiThermometer
 
 .. inclusion-marker-before-installation
 
 Installation
```

### Comparing `bluetooth-clocks-0.1.2/src/bluetooth_clocks.egg-info/SOURCES.txt` & `bluetooth-clocks-0.2.0/src/bluetooth_clocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluetooth-clocks-0.1.2/tests/test_current_time_service.py` & `bluetooth-clocks-0.2.0/tests/test_current_time_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,24 +21,24 @@
     "model",
     [
         CurrentTimeService,
         InfiniTime,
     ],
 )
 def test_in_supported_devices(model: type[BluetoothClock]) -> None:
-    """Test whether the Current Time Service model is in the list of supported devices."""
+    """Test whether Current Time Service model is in the list of supported devices."""
     assert model.DEVICE_TYPE in supported_devices()
 
 
 @pytest.mark.parametrize(
-    "model, device, advertisement_data",
+    ("model", "device", "advertisement_data"),
     [
         (
             CurrentTimeService,
-            BLEDevice("EB:76:55:B9:56:18", "F15"),
+            BLEDevice("EB:76:55:B9:56:18", "F15", {}, -67),
             AdvertisementData(
                 local_name="F15",
                 manufacturer_data={},
                 platform_data=(),
                 rssi=-67,
                 service_data={},
                 service_uuids=[
@@ -49,15 +49,15 @@
                     "0000feea-0000-1000-8000-00805f9b34fb",
                 ],
                 tx_power=0,
             ),
         ),
         (
             InfiniTime,
-            BLEDevice("F3:BE:3E:97:17:A4", "InfiniTime"),
+            BLEDevice("F3:BE:3E:97:17:A4", "InfiniTime", {}, -67),
             AdvertisementData(
                 local_name="InfiniTime",
                 manufacturer_data={},
                 platform_data=(),
                 rssi=-67,
                 service_data={},
                 service_uuids=["00001530-1212-efde-1523-785feabcd123"],
@@ -67,15 +67,15 @@
     ],
 )
 def test_recognize(
     model: type[BluetoothClock],
     device: BLEDevice,
     advertisement_data: AdvertisementData,
 ) -> None:
-    """Test whether the Current Time Service model is recognized from an advertisement."""
+    """Test whether Current Time Service model is recognized from an advertisement."""
     assert model.recognize(device=device, advertisement_data=advertisement_data)
 
 
 @pytest.mark.parametrize(
     "model",
     [
         CurrentTimeService,
@@ -84,77 +84,85 @@
 )
 def test_readable(model: type[BluetoothClock]) -> None:
     """Test whether the time is readable on the device."""
     assert model.is_readable()
 
 
 @pytest.mark.parametrize(
-    "model, device, time_bytes, time",
+    ("model", "device", "time_bytes", "time"),
     [
         (
             CurrentTimeService,
-            BLEDevice("EB:76:55:B9:56:18"),
+            BLEDevice("EB:76:55:B9:56:18", "", {}, -67),
             bytes([0xE7, 0x07, 0x01, 0x07, 0x12, 0x29, 0x21, 0x06, 0x00]),
             "2023-01-07 18:41:33",
         ),
         (
             InfiniTime,
-            BLEDevice("F3:BE:3E:97:17:A4"),
+            BLEDevice("F3:BE:3E:97:17:A4", "", {}, -67),
             bytes([0xE7, 0x07, 0x01, 0x07, 0x12, 0x29, 0x21, 0x06, 0x00]),
             "2023-01-07 18:41:33",
         ),
     ],
 )
 def test_get_time_from_bytes(
-    model: type[BluetoothClock], device: BLEDevice, time_bytes: bytes, time: str
+    model: type[BluetoothClock],
+    device: BLEDevice,
+    time_bytes: bytes,
+    time: str,
 ) -> None:
     """Test the conversion from bytes to a timestamp."""
     timestamp = datetime.fromisoformat(time).timestamp()
     assert model(device).get_time_from_bytes(time_bytes) == timestamp
 
 
 @pytest.mark.parametrize(
-    "model, device, time_bytes",
+    ("model", "device", "time_bytes"),
     [
         (
             CurrentTimeService,
-            BLEDevice("EB:76:55:B9:56:18"),
+            BLEDevice("EB:76:55:B9:56:18", "", {}, -67),
             bytes([0x2A]),
         ),
         (
             InfiniTime,
-            BLEDevice("F3:BE:3E:97:17:A4"),
+            BLEDevice("F3:BE:3E:97:17:A4", "", {}, -67),
             bytes([0x00, 0x01, 0x02, 0x03, 0x04, 0x05, 0x06, 0x07, 0x08, 0x09]),
         ),
     ],
 )
 def test_get_time_from_bytes_invalid(
-    model: type[BluetoothClock], device: BLEDevice, time_bytes: bytes
+    model: type[BluetoothClock],
+    device: BLEDevice,
+    time_bytes: bytes,
 ) -> None:
     """Test whether trying to convert invalid bytes raises an exception."""
     with pytest.raises(InvalidTimeBytesError):
         model(device).get_time_from_bytes(time_bytes)
 
 
 @pytest.mark.parametrize(
-    "model, device, time, time_bytes",
+    ("model", "device", "time", "time_bytes"),
     [
         (
             CurrentTimeService,
-            BLEDevice("EB:76:55:B9:56:18"),
+            BLEDevice("EB:76:55:B9:56:18", "", {}, -67),
             "2023-01-07 18:41:33",
             bytes([0xE7, 0x07, 0x01, 0x07, 0x12, 0x29, 0x21, 0x06, 0x00, 0x00]),
         ),
         (
             InfiniTime,
-            BLEDevice("F3:BE:3E:97:17:A4"),
+            BLEDevice("F3:BE:3E:97:17:A4", "", {}, -67),
             "2023-01-07 18:41:33",
             bytes([0xE7, 0x07, 0x01, 0x07, 0x12, 0x29, 0x21, 0x06, 0x00, 0x00]),
         ),
     ],
 )
 def test_get_bytes_from_time(
-    model: type[BluetoothClock], device: BLEDevice, time: str, time_bytes: bytes
+    model: type[BluetoothClock],
+    device: BLEDevice,
+    time: str,
+    time_bytes: bytes,
 ) -> None:
     """Test the command to set the time."""
     timestamp = datetime.fromisoformat(time).timestamp()
     assert model(device).get_bytes_from_time(timestamp) == bytes(time_bytes)
```

### Comparing `bluetooth-clocks-0.1.2/tests/test_pvvx.py` & `bluetooth-clocks-0.2.0/tests/test_pvvx.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import pytest
 import time_machine
 from bleak.backends.device import BLEDevice
 from bleak.backends.scanner import AdvertisementData
 
 from bluetooth_clocks import supported_devices
 from bluetooth_clocks.devices.pvvx import PVVX
-from bluetooth_clocks.exceptions import TimeNotReadableError
 
 if sys.version_info >= (3, 9):
     from zoneinfo import ZoneInfo
 else:
     from backports.zoneinfo import ZoneInfo
 
 __author__ = "Koen Vervloesem"
@@ -28,15 +27,15 @@
     """Test whether PVVX is in the list of supported devices."""
     assert PVVX.DEVICE_TYPE in supported_devices()
 
 
 def test_recognize() -> None:
     """Test whether PVVX is recognized from an advertisement."""
     assert PVVX.recognize(
-        BLEDevice("A4:C1:38:D9:01:10", "LYWSD03MMC"),
+        BLEDevice("A4:C1:38:D9:01:10", "LYWSD03MMC", {}, -67),
         AdvertisementData(
             local_name="LYWSD03MMC",
             manufacturer_data={},
             platform_data=(),
             rssi=-67,
             service_data={
                 "0000181a-0000-1000-8000-00805f9b34fb": bytes(
@@ -52,36 +51,40 @@
                         0xDD,
                         0x18,
                         0x14,
                         0x0C,
                         0x64,
                         0xDC,
                         0x05,
-                    ]
-                )
+                    ],
+                ),
             },
             service_uuids=[],
             tx_power=0,
         ),
     )
 
 
 def test_readable() -> None:
     """Test whether the time is readable on the device."""
-    assert not PVVX.is_readable()
+    assert PVVX.is_readable()
 
 
+@pytest.mark.skipif(sys.platform.startswith("win"), reason="timezone problem")
+@time_machine.travel(datetime(2023, 7, 4, 17, 4, 5, tzinfo=CET_TZ), tick=False)
 def test_get_time_from_bytes() -> None:
     """Test the conversion from bytes to a timestamp."""
-    with pytest.raises(TimeNotReadableError):
-        PVVX(BLEDevice("A4:C1:38:D9:01:10")).get_time_from_bytes(
-            bytes([0x23, 0xDD, 0xBC, 0xB9, 0x63])
+    assert (
+        PVVX(BLEDevice("A4:C1:38:D9:01:10", "", {}, -67)).get_time_from_bytes(
+            bytes([0x23, 0xE5, 0x34, 0xA4, 0x64, 0x33, 0x3B, 0xA3, 0x64]),
         )
+        == time()
+    )
 
 
 @pytest.mark.skipif(sys.platform.startswith("win"), reason="timezone problem")
 @time_machine.travel(datetime(2023, 1, 7, 18, 41, tzinfo=CET_TZ), tick=False)
 def test_get_bytes_from_time() -> None:
     """Test the command to set the time."""
-    assert PVVX(BLEDevice("A4:C1:38:D9:01:10")).get_bytes_from_time(time()) == bytes(
-        [0x23, 0xBC, 0xBC, 0xB9, 0x63]
-    )
+    assert PVVX(BLEDevice("A4:C1:38:D9:01:10", "", {}, -67)).get_bytes_from_time(
+        time(),
+    ) == bytes([0x23, 0xBC, 0xBC, 0xB9, 0x63])
```

### Comparing `bluetooth-clocks-0.1.2/tests/test_qingping.py` & `bluetooth-clocks-0.2.0/tests/test_qingping.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """Test whether the Qingping BT Clock Lite is in the list of supported devices."""
     assert CGC1.DEVICE_TYPE in supported_devices()
 
 
 def test_recognize() -> None:
     """Test whether the Qingping BT Clock Lite is recognized from an advertisement."""
     assert CGC1.recognize(
-        BLEDevice("58:2D:34:54:2D:2C", "Qingping BT Clock Lite"),
+        BLEDevice("58:2D:34:54:2D:2C", "Qingping BT Clock Lite", {}, -67),
         AdvertisementData(
             local_name="Qingping BT Clock Lite",
             manufacturer_data={},
             platform_data=(),
             rssi=-67,
             service_data={
                 "0000fdcd-0000-1000-8000-00805f9b34fb": bytes(
@@ -54,16 +54,16 @@
                         0xD2,
                         0x00,
                         0x80,
                         0x02,
                         0x02,
                         0x01,
                         0x64,
-                    ]
-                )
+                    ],
+                ),
             },
             service_uuids=[],
             tx_power=0,
         ),
     )
 
 
@@ -71,19 +71,19 @@
     """Test whether the time is not readable on the device."""
     assert not CGC1.is_readable()
 
 
 def test_get_time_from_bytes() -> None:
     """Test that this class doesn't support conversion from bytes to a timestamp."""
     with pytest.raises(TimeNotReadableError):
-        CGC1(BLEDevice("58:2D:34:54:2D:2C")).get_time_from_bytes(
-            bytes([0x05, 0x09, 0x00, 0xF6, 0xAE, 0x63])
+        CGC1(BLEDevice("58:2D:34:54:2D:2C", "", {}, -67)).get_time_from_bytes(
+            bytes([0x05, 0x09, 0x00, 0xF6, 0xAE, 0x63]),
         )
 
 
 @pytest.mark.skipif(sys.platform.startswith("win"), reason="timezone problem")
 @time_machine.travel(datetime(2022, 12, 30, 16, 30, tzinfo=CET_TZ), tick=False)
 def test_get_bytes_from_time() -> None:
     """Test the command to set the time."""
-    assert CGC1(BLEDevice("58:2D:34:54:2D:2C")).get_bytes_from_time(time()) == bytes(
-        [0x05, 0x09, 0x08, 0x12, 0xAF, 0x63]
-    )
+    assert CGC1(BLEDevice("58:2D:34:54:2D:2C", "", {}, -67)).get_bytes_from_time(
+        time(),
+    ) == bytes([0x05, 0x09, 0x08, 0x12, 0xAF, 0x63])
```

### Comparing `bluetooth-clocks-0.1.2/tests/test_thermopro.py` & `bluetooth-clocks-0.2.0/tests/test_thermopro.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,32 +26,32 @@
 )
 def test_in_supported_devices(model: type[BluetoothClock]) -> None:
     """Test whether the ThermoPro device is in the list of supported devices."""
     assert model.DEVICE_TYPE in supported_devices()
 
 
 @pytest.mark.parametrize(
-    "model, device, advertisement_data",
+    ("model", "device", "advertisement_data"),
     [
         (
             TP358,
-            BLEDevice("BC:C7:DA:6A:52:C6", "TP358 (52C6)"),
+            BLEDevice("BC:C7:DA:6A:52:C6", "TP358 (52C6)", {}, -67),
             AdvertisementData(
                 local_name="TP358 (52C6)",
                 manufacturer_data={0xD2C2: bytes([0x00, 0x3C, 0x02, 0x2C])},
                 platform_data=(),
                 rssi=-67,
                 service_data={},
                 service_uuids=[],
                 tx_power=0,
             ),
         ),
         (
             TP393,
-            BLEDevice("10:76:36:14:2A:3D", "TP393 (2A3D)"),
+            BLEDevice("10:76:36:14:2A:3D", "TP393 (2A3D)", {}, -67),
             AdvertisementData(
                 local_name="TP393 (2A3D)",
                 manufacturer_data={0xD0C2: bytes([0x00, 0x3F, 0x02, 0x2C])},
                 platform_data=(),
                 rssi=-67,
                 service_data={},
                 service_uuids=[],
@@ -78,49 +78,51 @@
 )
 def test_not_readable(model: type[BluetoothClock]) -> None:
     """Test whether the time is not readable on the device."""
     assert not model.is_readable()
 
 
 @pytest.mark.parametrize(
-    "model, device, time_bytes",
+    ("model", "device", "time_bytes"),
     [
         (
             TP358,
-            BLEDevice("BC:C7:DA:6A:52:C6"),
+            BLEDevice("BC:C7:DA:6A:52:C6", "", {}, -67),
             bytes([0xA5, 0x16, 0x0C, 0x1D, 0x12, 0x09, 0x01, 0x04, 0x01, 0x5A]),
         ),
         (
             TP393,
-            BLEDevice("10:76:36:14:2A:3D"),
+            BLEDevice("10:76:36:14:2A:3D", "", {}, -67),
             bytes([0xA5, 0x17, 0x01, 0x07, 0x11, 0x20, 0x32, 0x06, 0x00, 0x5A]),
         ),
     ],
 )
 def test_get_time_from_bytes(
-    model: type[BluetoothClock], device: BLEDevice, time_bytes: bytes
+    model: type[BluetoothClock],
+    device: BLEDevice,
+    time_bytes: bytes,
 ) -> None:
     """Test that this class doesn't support conversion from bytes to a timestamp."""
     with pytest.raises(TimeNotReadableError):
         model(device).get_time_from_bytes(time_bytes)
 
 
 @pytest.mark.parametrize(
-    "model, device, time, ampm, time_bytes",
+    ("model", "device", "time", "ampm", "time_bytes"),
     [
         (
             TP358,
-            BLEDevice("BC:C7:DA:6A:52:C6"),
+            BLEDevice("BC:C7:DA:6A:52:C6", "", {}, -67),
             "2022-12-29 18:09:01",
             False,
             bytes([0xA5, 0x16, 0x0C, 0x1D, 0x12, 0x09, 0x01, 0x04, 0x01, 0x5A]),
         ),
         (
             TP393,
-            BLEDevice("10:76:36:14:2A:3D"),
+            BLEDevice("10:76:36:14:2A:3D", "", {}, -67),
             "2023-01-07 17:32:50",
             True,
             bytes([0xA5, 0x17, 0x01, 0x07, 0x11, 0x20, 0x32, 0x06, 0x00, 0x5A]),
         ),
     ],
 )
 def test_get_bytes_from_time(
```

### Comparing `bluetooth-clocks-0.1.2/tests/test_xiaomi.py` & `bluetooth-clocks-0.2.0/tests/test_xiaomi.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """Test whether the Xiaomi LYWSD02 is in the list of supported devices."""
     assert LYWSD02.DEVICE_TYPE in supported_devices()
 
 
 def test_recognize() -> None:
     """Test whether the Xiaomi LYWSD02 is recognized from an advertisement."""
     assert LYWSD02.recognize(
-        BLEDevice("E7:2E:00:B1:38:96", "LYWSD02"),
+        BLEDevice("E7:2E:00:B1:38:96", "LYWSD02", {}, -67),
         AdvertisementData(
             local_name="LYWSD02",
             manufacturer_data={},
             platform_data=(),
             rssi=-67,
             service_data={
                 "0000fe95-0000-1000-8000-00805f9b34fb": bytes(
@@ -54,16 +54,16 @@
                         0xE7,
                         0x09,
                         0x04,
                         0x10,
                         0x02,
                         0xD5,
                         0x00,
-                    ]
-                )
+                    ],
+                ),
             },
             service_uuids=[
                 "0000181a-0000-1000-8000-00805f9b34fb",
                 "0000fef5-0000-1000-8000-00805f9b34fb",
             ],
             tx_power=0,
         ),
@@ -75,27 +75,29 @@
     assert LYWSD02.is_readable()
 
 
 def test_get_time_from_bytes() -> None:
     """Test the conversion from bytes to a timestamp."""
     timestamp = datetime.fromisoformat("2023-01-07 18:41:33+00:00").timestamp()
     assert (
-        LYWSD02(BLEDevice("E7:2E:00:B1:38:96")).get_time_from_bytes(
-            bytes([0xDD, 0xBC, 0xB9, 0x63, 0x00])
+        LYWSD02(BLEDevice("E7:2E:00:B1:38:96", "", {}, -67)).get_time_from_bytes(
+            bytes([0xDD, 0xBC, 0xB9, 0x63, 0x00]),
         )
         == timestamp
     )
 
 
 def test_get_time_from_bytes_invalid() -> None:
     """Test whether trying to convert invalid bytes raises an exception."""
     with pytest.raises(InvalidTimeBytesError):
-        LYWSD02(BLEDevice("E7:2E:00:B1:38:96")).get_time_from_bytes(bytes([0x2A]))
+        LYWSD02(BLEDevice("E7:2E:00:B1:38:96", "", {}, -67)).get_time_from_bytes(
+            bytes([0x2A]),
+        )
 
 
 @pytest.mark.skipif(sys.platform.startswith("win"), reason="timezone problem")
 @time_machine.travel(datetime(2023, 1, 7, 18, 41, tzinfo=CET_TZ), tick=False)
 def test_get_bytes_from_time() -> None:
     """Test the command to set the time."""
-    assert LYWSD02(BLEDevice("E7:2E:00:B1:38:96")).get_bytes_from_time(time()) == bytes(
-        [0xAC, 0xAE, 0xB9, 0x63, 0x01]
-    )
+    assert LYWSD02(BLEDevice("E7:2E:00:B1:38:96", "", {}, -67)).get_bytes_from_time(
+        time(),
+    ) == bytes([0xAC, 0xAE, 0xB9, 0x63, 0x01])
```

### Comparing `bluetooth-clocks-0.1.2/tox.ini` & `bluetooth-clocks-0.2.0/tox.ini`

 * *Files identical despite different names*

