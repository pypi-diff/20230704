# Comparing `tmp/naneos-devices-0.2.tar.gz` & `tmp/naneos-devices-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naneos-devices-0.2.tar", last modified: Tue Jul  4 15:43:25 2023, max compression
+gzip compressed data, was "naneos-devices-0.3.tar", last modified: Tue Jul  4 15:51:17 2023, max compression
```

## Comparing `naneos-devices-0.2.tar` & `naneos-devices-0.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:43:25.392215 naneos-devices-0.2/
--rw-r--r--   0 huegi      (501) staff       (20)      642 2023-07-04 14:17:35.000000 naneos-devices-0.2/.coveragerc
--rw-r--r--   0 huegi      (501) staff       (20)      620 2023-07-04 14:17:35.000000 naneos-devices-0.2/.gitignore
--rw-r--r--   0 huegi      (501) staff       (20)      513 2023-07-04 14:17:35.000000 naneos-devices-0.2/.readthedocs.yml
--rw-r--r--   0 huegi      (501) staff       (20)       49 2023-07-04 14:17:35.000000 naneos-devices-0.2/AUTHORS.md
--rw-r--r--   0 huegi      (501) staff       (20)      122 2023-07-04 14:17:35.000000 naneos-devices-0.2/CHANGELOG.md
--rw-r--r--   0 huegi      (501) staff       (20)    14207 2023-07-04 14:17:35.000000 naneos-devices-0.2/CONTRIBUTING.rst
--rw-r--r--   0 huegi      (501) staff       (20)     1093 2023-07-04 14:17:35.000000 naneos-devices-0.2/LICENSE.txt
--rw-r--r--   0 huegi      (501) staff       (20)      842 2023-07-04 15:43:25.392278 naneos-devices-0.2/PKG-INFO
--rw-r--r--   0 huegi      (501) staff       (20)      225 2023-07-04 15:40:46.000000 naneos-devices-0.2/Pipfile
--rw-r--r--   0 huegi      (501) staff       (20)    34193 2023-07-04 14:21:53.000000 naneos-devices-0.2/Pipfile.lock
--rw-r--r--   0 huegi      (501) staff       (20)      378 2023-07-04 14:17:35.000000 naneos-devices-0.2/README.md
-drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:43:25.388723 naneos-devices-0.2/docs/
--rw-r--r--   0 huegi      (501) staff       (20)     1183 2023-07-04 14:17:35.000000 naneos-devices-0.2/docs/Makefile
-drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:43:25.388861 naneos-devices-0.2/docs/_static/
--rw-r--r--   0 huegi      (501) staff       (20)       19 2023-07-04 14:17:35.000000 naneos-devices-0.2/docs/_static/.gitignore
--rw-r--r--   0 huegi      (501) staff       (20)       49 2023-07-04 14:17:35.000000 naneos-devices-0.2/docs/authors.md
--rw-r--r--   0 huegi      (501) staff       (20)      122 2023-07-04 14:17:35.000000 naneos-devices-0.2/docs/changelog.md
--rw-r--r--   0 huegi      (501) staff       (20)    10571 2023-07-04 14:17:35.000000 naneos-devices-0.2/docs/conf.py
--rw-r--r--   0 huegi      (501) staff       (20)       34 2023-07-04 14:17:35.000000 naneos-devices-0.2/docs/contributing.rst
--rw-r--r--   0 huegi      (501) staff       (20)     1073 2023-07-04 14:17:35.000000 naneos-devices-0.2/docs/index.md
--rw-r--r--   0 huegi      (501) staff       (20)       74 2023-07-04 14:17:35.000000 naneos-devices-0.2/docs/license.rst
--rw-r--r--   0 huegi      (501) staff       (20)      378 2023-07-04 14:17:35.000000 naneos-devices-0.2/docs/readme.md
--rw-r--r--   0 huegi      (501) staff       (20)      252 2023-07-04 14:17:35.000000 naneos-devices-0.2/docs/requirements.txt
--rw-r--r--   0 huegi      (501) staff       (20)      364 2023-07-04 14:17:35.000000 naneos-devices-0.2/pyproject.toml
--rw-r--r--   0 huegi      (501) staff       (20)     1236 2023-07-04 15:43:25.392633 naneos-devices-0.2/setup.cfg
--rw-r--r--   0 huegi      (501) staff       (20)      728 2023-07-04 14:17:35.000000 naneos-devices-0.2/setup.py
-drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:43:25.384207 naneos-devices-0.2/src/
-drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:43:25.384120 naneos-devices-0.2/src/naneos/
-drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:43:25.389748 naneos-devices-0.2/src/naneos/partector2/
--rw-r--r--   0 huegi      (501) staff       (20)      147 2023-07-04 14:17:35.000000 naneos-devices-0.2/src/naneos/partector2/__init__.py
--rw-r--r--   0 huegi      (501) staff       (20)      642 2023-07-04 15:24:18.000000 naneos-devices-0.2/src/naneos/partector2/_data_structure.py
--rw-r--r--   0 huegi      (501) staff       (20)     1419 2023-07-04 14:17:35.000000 naneos-devices-0.2/src/naneos/partector2/_lambda_upload.py
--rw-r--r--   0 huegi      (501) staff       (20)     6800 2023-07-04 15:24:59.000000 naneos-devices-0.2/src/naneos/partector2/partector2.py
--rw-r--r--   0 huegi      (501) staff       (20)     1044 2023-07-04 14:17:35.000000 naneos-devices-0.2/src/naneos/partector2/scan_for_p2.py
-drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:43:25.390180 naneos-devices-0.2/src/naneos/partector2_ble/
--rw-r--r--   0 huegi      (501) staff       (20)       74 2023-07-04 14:17:35.000000 naneos-devices-0.2/src/naneos/partector2_ble/__init__.py
--rw-r--r--   0 huegi      (501) staff       (20)     1471 2023-07-04 14:17:35.000000 naneos-devices-0.2/src/naneos/partector2_ble/_lambda_upload.py
--rw-r--r--   0 huegi      (501) staff       (20)     6473 2023-07-04 14:17:35.000000 naneos-devices-0.2/src/naneos/partector2_ble/partector2_ble.py
-drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:43:25.390449 naneos-devices-0.2/src/naneos/serial_utils/
--rw-r--r--   0 huegi      (501) staff       (20)       85 2023-07-04 14:17:35.000000 naneos-devices-0.2/src/naneos/serial_utils/__init__.py
--rw-r--r--   0 huegi      (501) staff       (20)     1019 2023-07-04 14:50:26.000000 naneos-devices-0.2/src/naneos/serial_utils/list_serial_ports.py
-drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:43:25.391416 naneos-devices-0.2/src/naneos_devices.egg-info/
--rw-r--r--   0 huegi      (501) staff       (20)      842 2023-07-04 15:43:25.000000 naneos-devices-0.2/src/naneos_devices.egg-info/PKG-INFO
--rw-r--r--   0 huegi      (501) staff       (20)     1084 2023-07-04 15:43:25.000000 naneos-devices-0.2/src/naneos_devices.egg-info/SOURCES.txt
--rw-r--r--   0 huegi      (501) staff       (20)        1 2023-07-04 15:43:25.000000 naneos-devices-0.2/src/naneos_devices.egg-info/dependency_links.txt
--rw-r--r--   0 huegi      (501) staff       (20)        1 2023-07-04 14:20:37.000000 naneos-devices-0.2/src/naneos_devices.egg-info/not-zip-safe
--rw-r--r--   0 huegi      (501) staff       (20)      128 2023-07-04 15:43:25.000000 naneos-devices-0.2/src/naneos_devices.egg-info/requires.txt
--rw-r--r--   0 huegi      (501) staff       (20)        7 2023-07-04 15:43:25.000000 naneos-devices-0.2/src/naneos_devices.egg-info/top_level.txt
--rw-r--r--   0 huegi      (501) staff       (20)      249 2023-07-04 15:06:44.000000 naneos-devices-0.2/test.py
--rw-r--r--   0 huegi      (501) staff       (20)      180 2023-07-04 15:29:28.000000 naneos-devices-0.2/test_ble.py
-drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:43:25.391995 naneos-devices-0.2/tests/
--rw-r--r--   0 huegi      (501) staff       (20)      288 2023-07-04 14:17:35.000000 naneos-devices-0.2/tests/conftest.py
--rw-r--r--   0 huegi      (501) staff       (20)      216 2023-07-04 14:32:52.000000 naneos-devices-0.2/tests/test_partector2_ble.py
--rw-r--r--   0 huegi      (501) staff       (20)     1839 2023-07-04 14:52:51.000000 naneos-devices-0.2/tests/test_partector2_serial.py
--rw-r--r--   0 huegi      (501) staff       (20)     2674 2023-07-04 14:17:35.000000 naneos-devices-0.2/tox.ini
+drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:51:17.748491 naneos-devices-0.3/
+-rw-r--r--   0 huegi      (501) staff       (20)      642 2023-07-04 14:17:35.000000 naneos-devices-0.3/.coveragerc
+-rw-r--r--   0 huegi      (501) staff       (20)      620 2023-07-04 14:17:35.000000 naneos-devices-0.3/.gitignore
+-rw-r--r--   0 huegi      (501) staff       (20)      513 2023-07-04 14:17:35.000000 naneos-devices-0.3/.readthedocs.yml
+-rw-r--r--   0 huegi      (501) staff       (20)       49 2023-07-04 14:17:35.000000 naneos-devices-0.3/AUTHORS.md
+-rw-r--r--   0 huegi      (501) staff       (20)      122 2023-07-04 14:17:35.000000 naneos-devices-0.3/CHANGELOG.md
+-rw-r--r--   0 huegi      (501) staff       (20)    14207 2023-07-04 14:17:35.000000 naneos-devices-0.3/CONTRIBUTING.rst
+-rw-r--r--   0 huegi      (501) staff       (20)     1093 2023-07-04 14:17:35.000000 naneos-devices-0.3/LICENSE.txt
+-rw-r--r--   0 huegi      (501) staff       (20)      870 2023-07-04 15:51:17.748560 naneos-devices-0.3/PKG-INFO
+-rw-r--r--   0 huegi      (501) staff       (20)      225 2023-07-04 15:51:03.000000 naneos-devices-0.3/Pipfile
+-rw-r--r--   0 huegi      (501) staff       (20)    34193 2023-07-04 14:21:53.000000 naneos-devices-0.3/Pipfile.lock
+-rw-r--r--   0 huegi      (501) staff       (20)      378 2023-07-04 14:17:35.000000 naneos-devices-0.3/README.md
+drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:51:17.745161 naneos-devices-0.3/docs/
+-rw-r--r--   0 huegi      (501) staff       (20)     1183 2023-07-04 14:17:35.000000 naneos-devices-0.3/docs/Makefile
+drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:51:17.745312 naneos-devices-0.3/docs/_static/
+-rw-r--r--   0 huegi      (501) staff       (20)       19 2023-07-04 14:17:35.000000 naneos-devices-0.3/docs/_static/.gitignore
+-rw-r--r--   0 huegi      (501) staff       (20)       49 2023-07-04 14:17:35.000000 naneos-devices-0.3/docs/authors.md
+-rw-r--r--   0 huegi      (501) staff       (20)      122 2023-07-04 14:17:35.000000 naneos-devices-0.3/docs/changelog.md
+-rw-r--r--   0 huegi      (501) staff       (20)    10571 2023-07-04 14:17:35.000000 naneos-devices-0.3/docs/conf.py
+-rw-r--r--   0 huegi      (501) staff       (20)       34 2023-07-04 14:17:35.000000 naneos-devices-0.3/docs/contributing.rst
+-rw-r--r--   0 huegi      (501) staff       (20)     1073 2023-07-04 14:17:35.000000 naneos-devices-0.3/docs/index.md
+-rw-r--r--   0 huegi      (501) staff       (20)       74 2023-07-04 14:17:35.000000 naneos-devices-0.3/docs/license.rst
+-rw-r--r--   0 huegi      (501) staff       (20)      378 2023-07-04 14:17:35.000000 naneos-devices-0.3/docs/readme.md
+-rw-r--r--   0 huegi      (501) staff       (20)      252 2023-07-04 14:17:35.000000 naneos-devices-0.3/docs/requirements.txt
+-rw-r--r--   0 huegi      (501) staff       (20)      364 2023-07-04 14:17:35.000000 naneos-devices-0.3/pyproject.toml
+-rw-r--r--   0 huegi      (501) staff       (20)     1264 2023-07-04 15:51:17.748906 naneos-devices-0.3/setup.cfg
+-rw-r--r--   0 huegi      (501) staff       (20)      728 2023-07-04 14:17:35.000000 naneos-devices-0.3/setup.py
+drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:51:17.740875 naneos-devices-0.3/src/
+drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:51:17.740814 naneos-devices-0.3/src/naneos/
+drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:51:17.746200 naneos-devices-0.3/src/naneos/partector2/
+-rw-r--r--   0 huegi      (501) staff       (20)      147 2023-07-04 14:17:35.000000 naneos-devices-0.3/src/naneos/partector2/__init__.py
+-rw-r--r--   0 huegi      (501) staff       (20)      642 2023-07-04 15:24:18.000000 naneos-devices-0.3/src/naneos/partector2/_data_structure.py
+-rw-r--r--   0 huegi      (501) staff       (20)     1419 2023-07-04 14:17:35.000000 naneos-devices-0.3/src/naneos/partector2/_lambda_upload.py
+-rw-r--r--   0 huegi      (501) staff       (20)     6800 2023-07-04 15:24:59.000000 naneos-devices-0.3/src/naneos/partector2/partector2.py
+-rw-r--r--   0 huegi      (501) staff       (20)     1044 2023-07-04 14:17:35.000000 naneos-devices-0.3/src/naneos/partector2/scan_for_p2.py
+drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:51:17.746630 naneos-devices-0.3/src/naneos/partector2_ble/
+-rw-r--r--   0 huegi      (501) staff       (20)       74 2023-07-04 14:17:35.000000 naneos-devices-0.3/src/naneos/partector2_ble/__init__.py
+-rw-r--r--   0 huegi      (501) staff       (20)     1471 2023-07-04 14:17:35.000000 naneos-devices-0.3/src/naneos/partector2_ble/_lambda_upload.py
+-rw-r--r--   0 huegi      (501) staff       (20)     6473 2023-07-04 14:17:35.000000 naneos-devices-0.3/src/naneos/partector2_ble/partector2_ble.py
+drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:51:17.746907 naneos-devices-0.3/src/naneos/serial_utils/
+-rw-r--r--   0 huegi      (501) staff       (20)       85 2023-07-04 14:17:35.000000 naneos-devices-0.3/src/naneos/serial_utils/__init__.py
+-rw-r--r--   0 huegi      (501) staff       (20)     1019 2023-07-04 14:50:26.000000 naneos-devices-0.3/src/naneos/serial_utils/list_serial_ports.py
+drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:51:17.747748 naneos-devices-0.3/src/naneos_devices.egg-info/
+-rw-r--r--   0 huegi      (501) staff       (20)      870 2023-07-04 15:51:17.000000 naneos-devices-0.3/src/naneos_devices.egg-info/PKG-INFO
+-rw-r--r--   0 huegi      (501) staff       (20)     1084 2023-07-04 15:51:17.000000 naneos-devices-0.3/src/naneos_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 huegi      (501) staff       (20)        1 2023-07-04 15:51:17.000000 naneos-devices-0.3/src/naneos_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 huegi      (501) staff       (20)        1 2023-07-04 14:20:37.000000 naneos-devices-0.3/src/naneos_devices.egg-info/not-zip-safe
+-rw-r--r--   0 huegi      (501) staff       (20)      128 2023-07-04 15:51:17.000000 naneos-devices-0.3/src/naneos_devices.egg-info/requires.txt
+-rw-r--r--   0 huegi      (501) staff       (20)        7 2023-07-04 15:51:17.000000 naneos-devices-0.3/src/naneos_devices.egg-info/top_level.txt
+-rw-r--r--   0 huegi      (501) staff       (20)      249 2023-07-04 15:06:44.000000 naneos-devices-0.3/test.py
+-rw-r--r--   0 huegi      (501) staff       (20)      180 2023-07-04 15:29:28.000000 naneos-devices-0.3/test_ble.py
+drwxr-xr-x   0 huegi      (501) staff       (20)        0 2023-07-04 15:51:17.748291 naneos-devices-0.3/tests/
+-rw-r--r--   0 huegi      (501) staff       (20)      288 2023-07-04 14:17:35.000000 naneos-devices-0.3/tests/conftest.py
+-rw-r--r--   0 huegi      (501) staff       (20)      216 2023-07-04 14:32:52.000000 naneos-devices-0.3/tests/test_partector2_ble.py
+-rw-r--r--   0 huegi      (501) staff       (20)     1839 2023-07-04 14:52:51.000000 naneos-devices-0.3/tests/test_partector2_serial.py
+-rw-r--r--   0 huegi      (501) staff       (20)     2674 2023-07-04 14:17:35.000000 naneos-devices-0.3/tox.ini
```

### Comparing `naneos-devices-0.2/.coveragerc` & `naneos-devices-0.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/.gitignore` & `naneos-devices-0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/.readthedocs.yml` & `naneos-devices-0.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/CONTRIBUTING.rst` & `naneos-devices-0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/LICENSE.txt` & `naneos-devices-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/Pipfile.lock` & `naneos-devices-0.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/docs/Makefile` & `naneos-devices-0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/docs/conf.py` & `naneos-devices-0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/docs/index.md` & `naneos-devices-0.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/setup.cfg` & `naneos-devices-0.3/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = naneos-devices
-description = Add a short description here!
+description = Python client for naneos particle solutions gmbh devices.
 author = huegi
 author_email = m.huegi@outlook.com
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://github.com/pyscaffold/pyscaffold/
```

### Comparing `naneos-devices-0.2/setup.py` & `naneos-devices-0.3/setup.py`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/src/naneos/partector2/_data_structure.py` & `naneos-devices-0.3/src/naneos/partector2/_data_structure.py`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/src/naneos/partector2/_lambda_upload.py` & `naneos-devices-0.3/src/naneos/partector2/_lambda_upload.py`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/src/naneos/partector2/partector2.py` & `naneos-devices-0.3/src/naneos/partector2/partector2.py`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/src/naneos/partector2/scan_for_p2.py` & `naneos-devices-0.3/src/naneos/partector2/scan_for_p2.py`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/src/naneos/partector2_ble/_lambda_upload.py` & `naneos-devices-0.3/src/naneos/partector2_ble/_lambda_upload.py`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/src/naneos/partector2_ble/partector2_ble.py` & `naneos-devices-0.3/src/naneos/partector2_ble/partector2_ble.py`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/src/naneos/serial_utils/list_serial_ports.py` & `naneos-devices-0.3/src/naneos/serial_utils/list_serial_ports.py`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/src/naneos_devices.egg-info/SOURCES.txt` & `naneos-devices-0.3/src/naneos_devices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/tests/test_partector2_serial.py` & `naneos-devices-0.3/tests/test_partector2_serial.py`

 * *Files identical despite different names*

### Comparing `naneos-devices-0.2/tox.ini` & `naneos-devices-0.3/tox.ini`

 * *Files identical despite different names*

