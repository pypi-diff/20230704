# Comparing `tmp/scottbrian_utils-2.3.0.tar.gz` & `tmp/scottbrian_utils-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scottbrian_utils-2.3.0.tar", last modified: Mon Feb  6 21:48:35 2023, max compression
+gzip compressed data, was "scottbrian_utils-2.4.0.tar", last modified: Mon Jul  3 13:41:26 2023, max compression
```

## Comparing `scottbrian_utils-2.3.0.tar` & `scottbrian_utils-2.4.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.480194 scottbrian_utils-2.3.0/
--rw-rw-rw-   0        0        0     2053 2022-01-25 18:21:47.000000 scottbrian_utils-2.3.0/.gitignore
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.411178 scottbrian_utils-2.3.0/.idea/
--rw-rw-rw-   0        0        0      184 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/.idea/.gitignore
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.412179 scottbrian_utils-2.3.0/.idea/codeStyles/
--rw-rw-rw-   0        0        0      153 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/.idea/codeStyles/codeStyleConfig.xml
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.413179 scottbrian_utils-2.3.0/.idea/dictionaries/
--rw-rw-rw-   0        0        0       86 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/.idea/dictionaries/Tiger.xml
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.414179 scottbrian_utils-2.3.0/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0      234 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      208 2023-01-22 01:56:06.000000 scottbrian_utils-2.3.0/.idea/misc.xml
--rw-rw-rw-   0        0        0      291 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/.idea/modules.xml
--rw-rw-rw-   0        0        0      191 2022-01-25 18:21:47.000000 scottbrian_utils-2.3.0/.idea/other.xml
--rw-rw-rw-   0        0        0     1206 2023-01-22 01:56:06.000000 scottbrian_utils-2.3.0/.idea/scottbrian_utils.iml
--rw-rw-rw-   0        0        0      185 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/.idea/vcs.xml
--rw-rw-rw-   0        0        0      636 2022-01-25 18:57:49.000000 scottbrian_utils-2.3.0/.readthedocs.yml
--rw-rw-rw-   0        0        0     1092 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/LICENSE
--rw-rw-rw-   0        0        0      443 2022-01-25 18:21:47.000000 scottbrian_utils-2.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5522 2023-02-06 21:48:35.481194 scottbrian_utils-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4491 2023-02-05 01:40:13.000000 scottbrian_utils-2.3.0/README.rst
--rw-rw-rw-   0        0        0     5418 2023-01-23 01:13:01.000000 scottbrian_utils-2.3.0/conftest.py
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.415180 scottbrian_utils-2.3.0/docs/
--rw-rw-rw-   0        0        0       50 2022-01-25 18:21:47.000000 scottbrian_utils-2.3.0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.430184 scottbrian_utils-2.3.0/docs/source/
--rw-rw-rw-   0        0        0        0 2022-01-14 00:08:20.000000 scottbrian_utils-2.3.0/docs/source/_static
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.432183 scottbrian_utils-2.3.0/docs/source/adjust_sphinx/
--rw-rw-rw-   0        0        0        0 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/docs/source/adjust_sphinx/__init__.py
--rw-rw-rw-   0        0        0     2425 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/docs/source/adjust_sphinx/adjust_sphinx.py
--rw-rw-rw-   0        0        0     2377 2022-01-27 18:12:37.000000 scottbrian_utils-2.3.0/docs/source/conf.py
--rw-rw-rw-   0        0        0       38 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/docs/source/diag_msg_link.rst
--rw-rw-rw-   0        0        0       42 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/docs/source/file_catalog_link.rst
--rw-rw-rw-   0        0        0       40 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/docs/source/flower_box_link.rst
--rw-rw-rw-   0        0        0      711 2022-02-23 01:02:07.000000 scottbrian_utils-2.3.0/docs/source/index.rst
--rw-rw-rw-   0        0        0       42 2022-01-25 18:21:47.000000 scottbrian_utils-2.3.0/docs/source/log_verifier_link.rst
--rw-rw-rw-   0        0        0       34 2022-01-25 18:21:47.000000 scottbrian_utils-2.3.0/docs/source/msgs_link.rst
--rw-rw-rw-   0        0        0       36 2022-02-23 01:02:07.000000 scottbrian_utils-2.3.0/docs/source/pauser_link.rst
--rw-rw-rw-   0        0        0      306 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/docs/source/setup.py
--rw-rw-rw-   0        0        0       40 2022-01-25 18:21:47.000000 scottbrian_utils-2.3.0/docs/source/stop_watch_link.rst
--rw-rw-rw-   0        0        0       38 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/docs/source/time_hdr_link.rst
--rw-rw-rw-   0        0        0       35 2022-01-25 18:21:47.000000 scottbrian_utils-2.3.0/docs/source/timer_link.rst
--rw-rw-rw-   0        0        0      230 2022-01-25 18:21:47.000000 scottbrian_utils-2.3.0/mypy.ini
--rw-rw-rw-   0        0        0      354 2023-01-25 21:00:51.000000 scottbrian_utils-2.3.0/pyproject.toml
--rw-rw-rw-   0        0        0      694 2023-01-19 21:14:45.000000 scottbrian_utils-2.3.0/pytest.ini
--rw-rw-rw-   0        0        0     1262 2023-02-06 21:48:35.482195 scottbrian_utils-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2122 2022-01-25 18:21:47.000000 scottbrian_utils-2.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.433184 scottbrian_utils-2.3.0/src/
--rw-rw-rw-   0        0        0     5191 2022-01-25 18:21:47.000000 scottbrian_utils-2.3.0/src/conftest.py
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.448187 scottbrian_utils-2.3.0/src/scottbrian_utils/
--rw-rw-rw-   0        0        0      139 2023-02-06 21:30:31.000000 scottbrian_utils-2.3.0/src/scottbrian_utils/__init__.py
--rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/src/scottbrian_utils/__init__.pyi
--rw-rw-rw-   0        0        0    13219 2023-01-27 22:54:42.000000 scottbrian_utils-2.3.0/src/scottbrian_utils/diag_msg.py
--rw-rw-rw-   0        0        0    15032 2023-01-19 19:51:29.000000 scottbrian_utils-2.3.0/src/scottbrian_utils/file_catalog.py
--rw-rw-rw-   0        0        0     1833 2022-01-25 18:21:47.000000 scottbrian_utils-2.3.0/src/scottbrian_utils/flower_box.py
--rw-rw-rw-   0        0        0    20300 2023-01-19 19:51:29.000000 scottbrian_utils-2.3.0/src/scottbrian_utils/log_verifier.py
--rw-rw-rw-   0        0        0     7606 2022-01-25 18:21:47.000000 scottbrian_utils-2.3.0/src/scottbrian_utils/msgs.py
--rw-rw-rw-   0        0        0    20558 2023-01-22 01:44:10.000000 scottbrian_utils-2.3.0/src/scottbrian_utils/pauser.py
--rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/src/scottbrian_utils/py.typed
--rw-rw-rw-   0        0        0     6792 2023-01-26 16:36:30.000000 scottbrian_utils-2.3.0/src/scottbrian_utils/stop_watch.py
--rw-rw-rw-   0        0        0    17926 2022-01-25 18:21:47.000000 scottbrian_utils-2.3.0/src/scottbrian_utils/time_hdr.py
--rw-rw-rw-   0        0        0    24422 2023-01-24 00:38:23.000000 scottbrian_utils-2.3.0/src/scottbrian_utils/timer.py
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.455188 scottbrian_utils-2.3.0/src/scottbrian_utils.egg-info/
--rw-rw-rw-   0        0        0     5522 2023-02-06 21:48:35.000000 scottbrian_utils-2.3.0/src/scottbrian_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2412 2023-02-06 21:48:35.000000 scottbrian_utils-2.3.0/src/scottbrian_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-06 21:48:35.000000 scottbrian_utils-2.3.0/src/scottbrian_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-12-29 18:29:15.000000 scottbrian_utils-2.3.0/src/scottbrian_utils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       24 2023-02-06 21:48:35.000000 scottbrian_utils-2.3.0/src/scottbrian_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-02-06 21:48:35.000000 scottbrian_utils-2.3.0/src/scottbrian_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.387992 scottbrian_utils-2.3.0/tests/
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.470192 scottbrian_utils-2.3.0/tests/test_scottbrian_utils/
--rw-rw-rw-   0        0        0       38 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/tests/test_scottbrian_utils/__init__.py
--rw-rw-rw-   0        0        0     8370 2022-01-25 18:21:47.000000 scottbrian_utils-2.3.0/tests/test_scottbrian_utils/adjust_diag_msg_tcode.py
--rw-rw-rw-   0        0        0     5501 2023-01-19 21:14:45.000000 scottbrian_utils-2.3.0/tests/test_scottbrian_utils/conftest.py
--rw-rw-rw-   0        0        0   550514 2023-01-28 00:55:13.000000 scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_diag_msg.py
--rw-rw-rw-   0        0        0    17571 2022-10-01 23:07:43.000000 scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_file_catalog.py
--rw-rw-rw-   0        0        0     7736 2022-01-25 18:21:47.000000 scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_flower_box.py
--rw-rw-rw-   0        0        0    44735 2023-01-27 17:24:14.000000 scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_log_verifier.py
--rw-rw-rw-   0        0        0    16717 2023-02-06 21:29:52.000000 scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_msgs.py
--rw-rw-rw-   0        0        0    37782 2023-01-23 01:13:01.000000 scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_pauser.py
--rw-rw-rw-   0        0        0    17674 2023-01-24 22:19:36.000000 scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_stop_watch.py
--rw-rw-rw-   0        0        0    76612 2023-01-26 17:08:38.000000 scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_time_hdr.py
--rw-rw-rw-   0        0        0    41088 2023-01-23 16:13:49.000000 scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_timer.py
--rw-rw-rw-   0        0        0     5785 2023-01-19 18:22:10.000000 scottbrian_utils-2.3.0/tox.ini
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.389172 scottbrian_utils-2.3.0/type_stubs/
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.471192 scottbrian_utils-2.3.0/type_stubs/mypywrapt/
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.474193 scottbrian_utils-2.3.0/type_stubs/mypywrapt/adjust_src/
--rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/type_stubs/mypywrapt/adjust_src/__init__.pyi
--rw-rw-rw-   0        0        0     1292 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/type_stubs/mypywrapt/adjust_src/adjust_src.py
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.390173 scottbrian_utils-2.3.0/type_stubs/mypywrapt/build/
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.390173 scottbrian_utils-2.3.0/type_stubs/mypywrapt/build/lib/
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.475193 scottbrian_utils-2.3.0/type_stubs/mypywrapt/build/lib/adjust_src/
--rw-rw-rw-   0        0        0     1292 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/type_stubs/mypywrapt/build/lib/adjust_src/adjust_src.py
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.477193 scottbrian_utils-2.3.0/type_stubs/mypywrapt/build/lib/wrapt-stubs/
--rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/type_stubs/mypywrapt/build/lib/wrapt-stubs/__init__.pyi
--rw-rw-rw-   0        0        0      329 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/type_stubs/mypywrapt/build/lib/wrapt-stubs/decorators.pyi
--rw-rw-rw-   0        0        0      388 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/type_stubs/mypywrapt/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-06 21:48:35.479194 scottbrian_utils-2.3.0/type_stubs/mypywrapt/wrapt-stubs/
--rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/type_stubs/mypywrapt/wrapt-stubs/__init__.pyi
--rw-rw-rw-   0        0        0      329 2021-12-29 18:20:23.000000 scottbrian_utils-2.3.0/type_stubs/mypywrapt/wrapt-stubs/decorators.pyi
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:26.095555 scottbrian_utils-2.4.0/
+-rw-rw-rw-   0        0        0     2053 2022-01-25 18:21:47.000000 scottbrian_utils-2.4.0/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:26.015537 scottbrian_utils-2.4.0/.idea/
+-rw-rw-rw-   0        0        0      184 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/.idea/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:26.017537 scottbrian_utils-2.4.0/.idea/codeStyles/
+-rw-rw-rw-   0        0        0      153 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/.idea/codeStyles/codeStyleConfig.xml
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:26.018538 scottbrian_utils-2.4.0/.idea/dictionaries/
+-rw-rw-rw-   0        0        0       86 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/.idea/dictionaries/Tiger.xml
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:26.019538 scottbrian_utils-2.4.0/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0      234 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      208 2023-01-22 01:56:06.000000 scottbrian_utils-2.4.0/.idea/misc.xml
+-rw-rw-rw-   0        0        0      291 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/.idea/modules.xml
+-rw-rw-rw-   0        0        0      191 2022-01-25 18:21:47.000000 scottbrian_utils-2.4.0/.idea/other.xml
+-rw-rw-rw-   0        0        0     1206 2023-01-22 01:56:06.000000 scottbrian_utils-2.4.0/.idea/scottbrian_utils.iml
+-rw-rw-rw-   0        0        0      185 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/.idea/vcs.xml
+-rw-rw-rw-   0        0        0      636 2022-01-25 18:57:49.000000 scottbrian_utils-2.4.0/.readthedocs.yml
+-rw-rw-rw-   0        0        0     1092 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/LICENSE
+-rw-rw-rw-   0        0        0      443 2022-01-25 18:21:47.000000 scottbrian_utils-2.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5655 2023-07-03 13:41:26.095555 scottbrian_utils-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4624 2023-07-01 00:51:21.000000 scottbrian_utils-2.4.0/README.rst
+-rw-rw-rw-   0        0        0     5418 2023-01-23 01:13:01.000000 scottbrian_utils-2.4.0/conftest.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:26.020538 scottbrian_utils-2.4.0/docs/
+-rw-rw-rw-   0        0        0       50 2022-01-25 18:21:47.000000 scottbrian_utils-2.4.0/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:26.037542 scottbrian_utils-2.4.0/docs/source/
+-rw-rw-rw-   0        0        0        0 2022-01-14 00:08:20.000000 scottbrian_utils-2.4.0/docs/source/_static
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:26.039543 scottbrian_utils-2.4.0/docs/source/adjust_sphinx/
+-rw-rw-rw-   0        0        0        0 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/docs/source/adjust_sphinx/__init__.py
+-rw-rw-rw-   0        0        0     2425 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/docs/source/adjust_sphinx/adjust_sphinx.py
+-rw-rw-rw-   0        0        0     2377 2023-07-01 00:51:20.000000 scottbrian_utils-2.4.0/docs/source/conf.py
+-rw-rw-rw-   0        0        0       38 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/docs/source/diag_msg_link.rst
+-rw-rw-rw-   0        0        0       42 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/docs/source/file_catalog_link.rst
+-rw-rw-rw-   0        0        0       40 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/docs/source/flower_box_link.rst
+-rw-rw-rw-   0        0        0      711 2022-02-23 01:02:07.000000 scottbrian_utils-2.4.0/docs/source/index.rst
+-rw-rw-rw-   0        0        0       42 2022-01-25 18:21:47.000000 scottbrian_utils-2.4.0/docs/source/log_verifier_link.rst
+-rw-rw-rw-   0        0        0       34 2022-01-25 18:21:47.000000 scottbrian_utils-2.4.0/docs/source/msgs_link.rst
+-rw-rw-rw-   0        0        0       36 2022-02-23 01:02:07.000000 scottbrian_utils-2.4.0/docs/source/pauser_link.rst
+-rw-rw-rw-   0        0        0      306 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/docs/source/setup.py
+-rw-rw-rw-   0        0        0       40 2022-01-25 18:21:47.000000 scottbrian_utils-2.4.0/docs/source/stop_watch_link.rst
+-rw-rw-rw-   0        0        0       38 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/docs/source/time_hdr_link.rst
+-rw-rw-rw-   0        0        0       35 2022-01-25 18:21:47.000000 scottbrian_utils-2.4.0/docs/source/timer_link.rst
+-rw-rw-rw-   0        0        0      230 2022-01-25 18:21:47.000000 scottbrian_utils-2.4.0/mypy.ini
+-rw-rw-rw-   0        0        0      354 2023-01-25 21:00:51.000000 scottbrian_utils-2.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      694 2023-01-19 21:14:45.000000 scottbrian_utils-2.4.0/pytest.ini
+-rw-rw-rw-   0        0        0     1262 2023-07-03 13:41:26.096555 scottbrian_utils-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2122 2022-01-25 18:21:47.000000 scottbrian_utils-2.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:26.040543 scottbrian_utils-2.4.0/src/
+-rw-rw-rw-   0        0        0     5191 2022-01-25 18:21:47.000000 scottbrian_utils-2.4.0/src/conftest.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:26.057546 scottbrian_utils-2.4.0/src/scottbrian_utils/
+-rw-rw-rw-   0        0        0      139 2023-07-01 00:51:20.000000 scottbrian_utils-2.4.0/src/scottbrian_utils/__init__.py
+-rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/src/scottbrian_utils/__init__.pyi
+-rw-rw-rw-   0        0        0    13219 2023-01-27 22:54:42.000000 scottbrian_utils-2.4.0/src/scottbrian_utils/diag_msg.py
+-rw-rw-rw-   0        0        0    15032 2023-01-19 19:51:29.000000 scottbrian_utils-2.4.0/src/scottbrian_utils/file_catalog.py
+-rw-rw-rw-   0        0        0     1833 2022-01-25 18:21:47.000000 scottbrian_utils-2.4.0/src/scottbrian_utils/flower_box.py
+-rw-rw-rw-   0        0        0    22684 2023-07-01 14:30:48.000000 scottbrian_utils-2.4.0/src/scottbrian_utils/log_verifier.py
+-rw-rw-rw-   0        0        0     7606 2022-01-25 18:21:47.000000 scottbrian_utils-2.4.0/src/scottbrian_utils/msgs.py
+-rw-rw-rw-   0        0        0    20558 2023-01-22 01:44:10.000000 scottbrian_utils-2.4.0/src/scottbrian_utils/pauser.py
+-rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/src/scottbrian_utils/py.typed
+-rw-rw-rw-   0        0        0     6792 2023-01-26 16:36:30.000000 scottbrian_utils-2.4.0/src/scottbrian_utils/stop_watch.py
+-rw-rw-rw-   0        0        0    17926 2022-01-25 18:21:47.000000 scottbrian_utils-2.4.0/src/scottbrian_utils/time_hdr.py
+-rw-rw-rw-   0        0        0    24423 2023-04-11 22:05:38.000000 scottbrian_utils-2.4.0/src/scottbrian_utils/timer.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:26.065548 scottbrian_utils-2.4.0/src/scottbrian_utils.egg-info/
+-rw-rw-rw-   0        0        0     5655 2023-07-03 13:41:25.000000 scottbrian_utils-2.4.0/src/scottbrian_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2412 2023-07-03 13:41:25.000000 scottbrian_utils-2.4.0/src/scottbrian_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 13:41:25.000000 scottbrian_utils-2.4.0/src/scottbrian_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-12-29 18:29:15.000000 scottbrian_utils-2.4.0/src/scottbrian_utils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       24 2023-07-03 13:41:25.000000 scottbrian_utils-2.4.0/src/scottbrian_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-03 13:41:25.000000 scottbrian_utils-2.4.0/src/scottbrian_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:25.990531 scottbrian_utils-2.4.0/tests/
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:26.083552 scottbrian_utils-2.4.0/tests/test_scottbrian_utils/
+-rw-rw-rw-   0        0        0       38 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/tests/test_scottbrian_utils/__init__.py
+-rw-rw-rw-   0        0        0     8370 2022-01-25 18:21:47.000000 scottbrian_utils-2.4.0/tests/test_scottbrian_utils/adjust_diag_msg_tcode.py
+-rw-rw-rw-   0        0        0     5469 2023-07-01 17:34:46.000000 scottbrian_utils-2.4.0/tests/test_scottbrian_utils/conftest.py
+-rw-rw-rw-   0        0        0   556494 2023-07-02 20:16:36.000000 scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_diag_msg.py
+-rw-rw-rw-   0        0        0    17555 2023-07-01 17:34:46.000000 scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_file_catalog.py
+-rw-rw-rw-   0        0        0     7704 2023-07-01 17:34:46.000000 scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_flower_box.py
+-rw-rw-rw-   0        0        0    58680 2023-07-01 17:34:46.000000 scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_log_verifier.py
+-rw-rw-rw-   0        0        0    16651 2023-07-01 17:34:46.000000 scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_msgs.py
+-rw-rw-rw-   0        0        0    37686 2023-07-01 17:34:46.000000 scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_pauser.py
+-rw-rw-rw-   0        0        0    17642 2023-07-01 17:34:46.000000 scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_stop_watch.py
+-rw-rw-rw-   0        0        0    76404 2023-07-01 17:39:55.000000 scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_time_hdr.py
+-rw-rw-rw-   0        0        0    41008 2023-07-01 17:34:46.000000 scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_timer.py
+-rw-rw-rw-   0        0        0     5964 2023-07-01 22:24:56.000000 scottbrian_utils-2.4.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:25.991531 scottbrian_utils-2.4.0/type_stubs/
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:26.085553 scottbrian_utils-2.4.0/type_stubs/mypywrapt/
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:26.087553 scottbrian_utils-2.4.0/type_stubs/mypywrapt/adjust_src/
+-rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/type_stubs/mypywrapt/adjust_src/__init__.pyi
+-rw-rw-rw-   0        0        0     1292 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/type_stubs/mypywrapt/adjust_src/adjust_src.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:25.992532 scottbrian_utils-2.4.0/type_stubs/mypywrapt/build/
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:25.993532 scottbrian_utils-2.4.0/type_stubs/mypywrapt/build/lib/
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:26.089554 scottbrian_utils-2.4.0/type_stubs/mypywrapt/build/lib/adjust_src/
+-rw-rw-rw-   0        0        0     1292 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/type_stubs/mypywrapt/build/lib/adjust_src/adjust_src.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:26.091554 scottbrian_utils-2.4.0/type_stubs/mypywrapt/build/lib/wrapt-stubs/
+-rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/type_stubs/mypywrapt/build/lib/wrapt-stubs/__init__.pyi
+-rw-rw-rw-   0        0        0      329 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/type_stubs/mypywrapt/build/lib/wrapt-stubs/decorators.pyi
+-rw-rw-rw-   0        0        0      388 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/type_stubs/mypywrapt/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:41:26.094555 scottbrian_utils-2.4.0/type_stubs/mypywrapt/wrapt-stubs/
+-rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/type_stubs/mypywrapt/wrapt-stubs/__init__.pyi
+-rw-rw-rw-   0        0        0      329 2021-12-29 18:20:23.000000 scottbrian_utils-2.4.0/type_stubs/mypywrapt/wrapt-stubs/decorators.pyi
```

### Comparing `scottbrian_utils-2.3.0/.gitignore` & `scottbrian_utils-2.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/.idea/scottbrian_utils.iml` & `scottbrian_utils-2.4.0/.idea/scottbrian_utils.iml`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/.readthedocs.yml` & `scottbrian_utils-2.4.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/LICENSE` & `scottbrian_utils-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/PKG-INFO` & `scottbrian_utils-2.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scottbrian_utils
-Version: 2.3.0
+Version: 2.4.0
 Summary: Miscellaneous utilities
 Home-page: https://github.com/ScottBrian/scottbrian_utils.git
 Author: Scott Tuttle
 Author-email: sbtuttle@outlook.com
 License: MIT
 Project-URL: Documentation, https://scottbrian-utils.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ScottBrian/scottbrian_utils.git
@@ -152,14 +152,18 @@
     * added repr for LogVer
 
 * 2.3.0
     * added is_specified method in Timer
     * added timeout_value in Timer
     * support for python 3.11
 
+* 2.4.0
+    * added fullmatch parm to add_msg in log_ver.py
+    * added print_matched parm to print_match_results in log_ver.py
+
 Meta
 ====
 
 Scott Tuttle
 
 Distributed under the MIT license. See ``LICENSE`` for more information.
```

### Comparing `scottbrian_utils-2.3.0/README.rst` & `scottbrian_utils-2.4.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -127,14 +127,18 @@
     * added repr for LogVer
 
 * 2.3.0
     * added is_specified method in Timer
     * added timeout_value in Timer
     * support for python 3.11
 
+* 2.4.0
+    * added fullmatch parm to add_msg in log_ver.py
+    * added print_matched parm to print_match_results in log_ver.py
+
 Meta
 ====
 
 Scott Tuttle
 
 Distributed under the MIT license. See ``LICENSE`` for more information.
```

### Comparing `scottbrian_utils-2.3.0/conftest.py` & `scottbrian_utils-2.4.0/conftest.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/docs/source/adjust_sphinx/adjust_sphinx.py` & `scottbrian_utils-2.4.0/docs/source/adjust_sphinx/adjust_sphinx.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/docs/source/conf.py` & `scottbrian_utils-2.4.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'scottbrian_utils'
 copyright = '2020, 2022, Scott Tuttle'
 author = 'Scott Tuttle'
 
 # The full version, including alpha/beta/rc tags
-release = '2.0.0'
+release = '2.4.0'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `scottbrian_utils-2.3.0/docs/source/index.rst` & `scottbrian_utils-2.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/pytest.ini` & `scottbrian_utils-2.4.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/setup.cfg` & `scottbrian_utils-2.4.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 00000030: 203d 204d 6973 6365 6c6c 616e 656f 7573   = Miscellaneous
 00000040: 2075 7469 6c69 7469 6573 0d0a 6c6f 6e67   utilities..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 7273 740d  ile: README.rst.
 00000070: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
 00000080: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
 00000090: 2074 6578 742f 782d 7273 740d 0a76 6572   text/x-rst..ver
-000000a0: 7369 6f6e 203d 2032 2e33 2e30 0d0a 7572  sion = 2.3.0..ur
+000000a0: 7369 6f6e 203d 2032 2e34 2e30 0d0a 7572  sion = 2.4.0..ur
 000000b0: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 000000c0: 7562 2e63 6f6d 2f53 636f 7474 4272 6961  ub.com/ScottBria
 000000d0: 6e2f 7363 6f74 7462 7269 616e 5f75 7469  n/scottbrian_uti
 000000e0: 6c73 2e67 6974 0d0a 6175 7468 6f72 203d  ls.git..author =
 000000f0: 2053 636f 7474 2054 7574 746c 650d 0a61   Scott Tuttle..a
 00000100: 7574 686f 725f 656d 6169 6c20 3d20 7362  uthor_email = sb
 00000110: 7475 7474 6c65 406f 7574 6c6f 6f6b 2e63  tuttle@outlook.c
```

### Comparing `scottbrian_utils-2.3.0/setup.py` & `scottbrian_utils-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/src/conftest.py` & `scottbrian_utils-2.4.0/src/conftest.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/src/scottbrian_utils/diag_msg.py` & `scottbrian_utils-2.4.0/src/scottbrian_utils/diag_msg.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/src/scottbrian_utils/file_catalog.py` & `scottbrian_utils-2.4.0/src/scottbrian_utils/file_catalog.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/src/scottbrian_utils/flower_box.py` & `scottbrian_utils-2.4.0/src/scottbrian_utils/flower_box.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/src/scottbrian_utils/log_verifier.py` & `scottbrian_utils-2.4.0/src/scottbrian_utils/log_verifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 :Example1: pytest test case logs a message and verifies
 
 .. code-block:: python
 
     from scottbrian_utils.log_verifier import LogVer
     import logging
-    def test_example1(caplog: pytest.CaptureFixture[str]) -> None:
+    def test_example1(caplog: pytest.LogCaptureFixture) -> None:
         logger = logging.getLogger('example_1')
         log_ver = LogVer('example_1')
         log_msg = 'hello'
         log_ver.add_msg(log_msg=log_msg)
         logger.debug(log_msg)
         match_results = log_ver.get_match_results(caplog=caplog)
         log_ver.print_match_results(match_results)
@@ -52,15 +52,15 @@
 
 :Example2: pytest test case expects two log records, only one was issued
 
 .. code-block:: python
 
     from scottbrian_utils.log_verifier import LogVer
     import logging
-    def test_example2(caplog: pytest.CaptureFixture[str]) -> None:
+    def test_example2(caplog: pytest.LogCaptureFixture) -> None:
         logger = logging.getLogger('example_2')
         log_ver = LogVer('example_2')
         log_msg1 = 'hello'
         log_ver.add_msg(log_msg=log_msg1)
         log_msg2 = 'goodbye'
         log_ver.add_msg(log_msg=log_msg2)
         logger.debug(log_msg1)
@@ -96,15 +96,15 @@
 
 :Example3: pytest test case expects one log record, two were issued
 
 .. code-block:: python
 
     from scottbrian_utils.log_verifier import LogVer
     import logging
-    def test_example3(caplog: pytest.CaptureFixture[str]) -> None:
+    def test_example3(caplog: pytest.LogCaptureFixture) -> None:
         logger = logging.getLogger('example_3')
         log_ver = LogVer('example_3')
         log_msg1 = 'hello'
         log_ver.add_msg(log_msg=log_msg1)
         log_msg2 = 'goodbye'
         logger.debug(log_msg1)
         logger.debug(log_msg2)
@@ -141,15 +141,15 @@
 :Example4: pytest test case expect two log records, two were issued,
            one different
 
 .. code-block:: python
 
     from scottbrian_utils.log_verifier import LogVer
     import logging
-    def test_example4(caplog: pytest.CaptureFixture[str]) -> None:
+    def test_example4(caplog: pytest.LogCaptureFixture) -> None:
         logger = logging.getLogger('example_4')
         log_ver = LogVer('example_4')
         log_msg1 = 'hello'
         log_ver.add_msg(log_msg=log_msg1)
         log_msg2a = 'goodbye'
         log_ver.add_msg(log_msg=log_msg2a)
         log_msg2b = 'see you soon'
@@ -275,14 +275,15 @@
         >>> logger = logging.getLogger('example_logger')
         >>> log_ver = LogVer('example_logger')
 
         """
         self.specified_args = locals()  # used for __repr__, see below
         self.call_seqs: dict[str, str] = {}
         self.expected_messages: list[tuple[str, int, Any]] = []
+        self.expected_messages_fullmatch: list[tuple[str, int, Any]] = []
         self.log_name = log_name
 
     ####################################################################
     # __repr__
     ####################################################################
     def __repr__(self) -> str:
         """Return a representation of the class.
@@ -346,27 +347,30 @@
 
     ####################################################################
     # add_msg
     ####################################################################
     def add_msg(self,
                 log_msg: str,
                 log_level: int = logging.DEBUG,
-                log_name: Optional[str] = None) -> None:
+                log_name: Optional[str] = None,
+                fullmatch: bool = False) -> None:
         """Add a message to the expected log messages.
 
         Args:
             log_msg: expected message to add
             log_level: expected logging level
             log_name: expected logger name
+            fullmatch: if True, use regex fullmatch instead of
+                match in method get_match_results
 
         Example: add two messages, each at a different level
 
         .. code-block:: python
 
-            def test_example(caplog: pytest.CaptureFixture[str]
+            def test_example(caplog: pytest.LogCaptureFixture
                             ) -> None:
                 logger = logging.getLogger('add_msg')
                 log_ver = LogVer('add_msg')
                 log_msg1 = 'hello'
                 log_msg2 = 'goodbye'
                 log_ver.add_msg(log_msg=log_msg1)
                 log_ver.add_msg(log_msg=log_msg2,
@@ -406,88 +410,133 @@
             ('add_msg', 40, 'goodbye')
 
         """
         if log_name:
             log_name_to_use = log_name
         else:
             log_name_to_use = self.log_name
-        self.expected_messages.append((log_name_to_use,
-                                       log_level,
-                                       re.compile(log_msg)
-                                       ))
+
+        if fullmatch:
+            self.expected_messages_fullmatch.append((log_name_to_use,
+                                                     log_level,
+                                                     re.compile(log_msg)
+                                                     ))
+        else:
+            self.expected_messages.append((log_name_to_use,
+                                           log_level,
+                                           re.compile(log_msg)
+                                           ))
 
     ####################################################################
     # get_match_results
     ####################################################################
     def get_match_results(self,
-                          caplog: pytest.CaptureFixture[str]
+                          caplog: pytest.LogCaptureFixture
                           ) -> MatchResults:
         """Match the expected to actual log records.
 
         Args:
             caplog: pytest fixture that captures log messages
 
         Returns:
             Number of expected records, number of actual records,
               number of matching records, list of unmatched expected
               records, list of unmatched actual records, and list
               or matching records
 
         """
-        unmatched_exp_records: list[tuple[str, int, Any]] = []
-        unmatched_actual_records: list[tuple[str, int, Any]] = []
-        matched_records: list[tuple[str, int, Any]] = []
+        # make a work copy of fullmatch expected records
+        unmatched_exp_records_fullmatch: list[tuple[str, int, Any]] = (
+            self.expected_messages_fullmatch.copy()
+        )
 
         # make a work copy of expected records
-        for record in self.expected_messages:
-            unmatched_exp_records.append(record)
+        unmatched_exp_records: list[tuple[str, int, Any]] = (
+            self.expected_messages.copy()
+        )
 
         # make a work copy of actual records
-        for record in caplog.record_tuples:
-            unmatched_actual_records.append(record)
+        unmatched_actual_records: list[tuple[str, int, Any]] = (
+            caplog.record_tuples.copy()
+        )
+
+        matched_records: list[tuple[str, int, Any]] = []
 
+        ################################################################
         # find matches, update working copies to reflect results
-        for actual_record in caplog.record_tuples:
-            for idx, exp_record in enumerate(unmatched_exp_records):
-                # check that the logger name, level, and message match
-                if (exp_record[0] == actual_record[0]
-                        and exp_record[1] == actual_record[1]
-                        and exp_record[2].match(actual_record[2])):
-                    unmatched_exp_records.pop(idx)
-                    unmatched_actual_records.remove(actual_record)
-                    matched_records.append((actual_record[0],
-                                            actual_record[1],
-                                            actual_record[2]))
-                    break
+        ################################################################
+        if unmatched_exp_records_fullmatch:  # if fullmatch records
+            for actual_record in caplog.record_tuples:
+                # look for fullmatch
+                for idx, exp_record in enumerate(
+                        unmatched_exp_records_fullmatch):
+                    # check that the logger name, level, and message
+                    # match
+                    if (exp_record[0] == actual_record[0]
+                            and exp_record[1] == actual_record[1]
+                            and exp_record[2].fullmatch(actual_record[2])):
+                        unmatched_exp_records_fullmatch.pop(idx)
+                        unmatched_actual_records.remove(actual_record)
+                        matched_records.append((actual_record[0],
+                                                actual_record[1],
+                                                actual_record[2]))
+                        break
+
+        if unmatched_exp_records:  # if partial match records
+            for actual_record in unmatched_actual_records.copy():
+                # look for partial match in unmatched_exp_records
+                for idx, exp_record in enumerate(unmatched_exp_records):
+                    # check that the logger name, level, and message
+                    # match
+                    if (exp_record[0] == actual_record[0]
+                            and exp_record[1] == actual_record[1]
+                            and exp_record[2].match(actual_record[2])):
+                        unmatched_exp_records.pop(idx)
+                        unmatched_actual_records.remove(actual_record)
+                        matched_records.append((actual_record[0],
+                                                actual_record[1],
+                                                actual_record[2]))
+                        break
 
         # convert unmatched expected records to string form
         unmatched_exp_records_2 = []
+        for item in unmatched_exp_records_fullmatch:
+            unmatched_exp_records_2.append((item[0],
+                                            item[1],
+                                            item[2].pattern))
+
         for item in unmatched_exp_records:
             unmatched_exp_records_2.append((item[0],
                                             item[1],
                                             item[2].pattern))
 
-        return MatchResults(num_exp_records=len(self.expected_messages),
-                            num_exp_unmatched=len(unmatched_exp_records_2),
-                            num_actual_records=len(caplog.records),
-                            num_actual_unmatched=len(unmatched_actual_records),
-                            num_records_matched=len(matched_records),
-                            unmatched_exp_records=unmatched_exp_records_2,
-                            unmatched_actual_records=unmatched_actual_records,
-                            matched_records=matched_records)
+        return MatchResults(
+            num_exp_records=(
+                len(self.expected_messages)
+                + len(self.expected_messages_fullmatch)),
+            num_exp_unmatched=len(unmatched_exp_records_2),
+            num_actual_records=len(caplog.records),
+            num_actual_unmatched=len(unmatched_actual_records),
+            num_records_matched=len(matched_records),
+            unmatched_exp_records=unmatched_exp_records_2,
+            unmatched_actual_records=unmatched_actual_records,
+            matched_records=matched_records)
 
     ####################################################################
     # print_match_results
     ####################################################################
     @staticmethod
-    def print_match_results(match_results: MatchResults) -> None:
+    def print_match_results(match_results: MatchResults,
+                            print_matched: bool = True) -> None:
         """Print the match results.
 
         Args:
             match_results: contains the results to be printed
+            print_matched: if True, print the matched records, otherwise
+                skip printing the matched records
 
         """
         max_num = max(match_results.num_exp_records,
                       match_results.num_exp_unmatched,
                       match_results.num_actual_records,
                       match_results.num_actual_unmatched,
                       match_results.num_records_matched)
@@ -510,17 +559,18 @@
         for log_msg in match_results.unmatched_exp_records:
             print(log_msg)
 
         print_flower_box_msg(['unmatched actual records', legend_msg])
         for log_msg in match_results.unmatched_actual_records:
             print(log_msg)
 
-        print_flower_box_msg(['matched records', legend_msg])
-        for log_msg in match_results.matched_records:
-            print(log_msg)
+        if print_matched:
+            print_flower_box_msg(['matched records', legend_msg])
+            for log_msg in match_results.matched_records:
+                print(log_msg)
 
     ####################################################################
     # verify log messages
     ####################################################################
     @staticmethod
     def verify_log_results(match_results: MatchResults) -> None:
         """Verify that each log message issued is as expected.
```

### Comparing `scottbrian_utils-2.3.0/src/scottbrian_utils/msgs.py` & `scottbrian_utils-2.4.0/src/scottbrian_utils/msgs.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/src/scottbrian_utils/pauser.py` & `scottbrian_utils-2.4.0/src/scottbrian_utils/pauser.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/src/scottbrian_utils/stop_watch.py` & `scottbrian_utils-2.4.0/src/scottbrian_utils/stop_watch.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/src/scottbrian_utils/time_hdr.py` & `scottbrian_utils-2.4.0/src/scottbrian_utils/time_hdr.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/src/scottbrian_utils/timer.py` & `scottbrian_utils-2.4.0/src/scottbrian_utils/timer.py`

 * *Files 0% similar despite different names*

```diff
@@ -466,15 +466,15 @@
         """
         if self._timeout:
             return True  # timeout with positive value was specified
         else:
             return False
 
     ####################################################################
-    # is_specified
+    # timeout_value
     ####################################################################
     def timeout_value(self) -> Optional[IntFloat]:
         """Return the timeout value that was specified.
 
         Returns:
             The timeout value that was specified, either via the timeout
                 value or the default timeout value, or None.
```

### Comparing `scottbrian_utils-2.3.0/src/scottbrian_utils.egg-info/PKG-INFO` & `scottbrian_utils-2.4.0/src/scottbrian_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scottbrian-utils
-Version: 2.3.0
+Version: 2.4.0
 Summary: Miscellaneous utilities
 Home-page: https://github.com/ScottBrian/scottbrian_utils.git
 Author: Scott Tuttle
 Author-email: sbtuttle@outlook.com
 License: MIT
 Project-URL: Documentation, https://scottbrian-utils.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ScottBrian/scottbrian_utils.git
@@ -152,14 +152,18 @@
     * added repr for LogVer
 
 * 2.3.0
     * added is_specified method in Timer
     * added timeout_value in Timer
     * support for python 3.11
 
+* 2.4.0
+    * added fullmatch parm to add_msg in log_ver.py
+    * added print_matched parm to print_match_results in log_ver.py
+
 Meta
 ====
 
 Scott Tuttle
 
 Distributed under the MIT license. See ``LICENSE`` for more information.
```

### Comparing `scottbrian_utils-2.3.0/src/scottbrian_utils.egg-info/SOURCES.txt` & `scottbrian_utils-2.4.0/src/scottbrian_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/tests/test_scottbrian_utils/adjust_diag_msg_tcode.py` & `scottbrian_utils-2.4.0/tests/test_scottbrian_utils/adjust_diag_msg_tcode.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/tests/test_scottbrian_utils/conftest.py` & `scottbrian_utils-2.4.0/tests/test_scottbrian_utils/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         """
         if self.exc_err_msg1:
             exc_msg = self.exc_err_msg1
             self.exc_err_msg1 = ''
             raise Exception(f'{exc_msg}')
 
 
-@pytest.fixture(autouse=True)  # type: ignore
+@pytest.fixture(autouse=True)
 def thread_exc(monkeypatch: Any) -> Generator[ExcHook, None, None]:
     """Instantiate and return a ThreadExc for testing.
 
     Args:
         monkeypatch: pytest fixture used to modify code for testing
 
     Yields:
@@ -142,15 +142,15 @@
                       '%a %b %d %Y %H:%M:%S',
                       '%a %b %d %H:%M:%S.%f',
                       '%A %b %d %H:%M:%S.%f',
                       '%A %B %d %H:%M:%S.%f'
                       ]
 
 
-@pytest.fixture(params=dt_format_arg_list)  # type: ignore
+@pytest.fixture(params=dt_format_arg_list)
 def dt_format_arg(request: Any) -> str:
     """Using different time formats.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
```

### Comparing `scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_diag_msg.py` & `scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_diag_msg.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 ########################################################################
 # depth_arg fixture
 ########################################################################
 depth_arg_list = [None, 0, 1, 2, 3]
 
 
-@pytest.fixture(params=depth_arg_list)  # type: ignore
+@pytest.fixture(params=depth_arg_list)
 def depth_arg(request: Any) -> int:
     """Using different depth args.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -72,15 +72,15 @@
 
 ########################################################################
 # file_arg fixture
 ########################################################################
 file_arg_list = [None, 'sys.stdout', 'sys.stderr']
 
 
-@pytest.fixture(params=file_arg_list)  # type: ignore
+@pytest.fixture(params=file_arg_list)
 def file_arg(request: Any) -> str:
     """Using different file arg.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -91,15 +91,15 @@
 
 ########################################################################
 # latest_arg fixture
 ########################################################################
 latest_arg_list = [None, 0, 1, 2, 3]
 
 
-@pytest.fixture(params=latest_arg_list)  # type: ignore
+@pytest.fixture(params=latest_arg_list)
 def latest_arg(request: Any) -> Union[int, None]:
     """Using different depth args.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -117,15 +117,15 @@
                 ['three + four'],
                 ['two', 'items'],
                 ['three', 'items', 'for you'],
                 ['this', 'has', 'number', 4],
                 ['here', 'some', 'math', 4 + 1]]
 
 
-@pytest.fixture(params=msg_arg_list)  # type: ignore
+@pytest.fixture(params=msg_arg_list)
 def msg_arg(request: Any) -> List[str]:
     """Using different message arg.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -4302,138 +4302,269 @@
         exp_stack.pop()
 
     ####################################################################
     # Class 0 Method 9
     ####################################################################
     @classmethod
     def test_get_caller_info_c0bt(cls,
-                                  exp_stack: Optional[Deque[CallerInfo]],
                                   capsys: pytest.CaptureFixture[str]
                                   ) -> None:
         """Get caller info overloaded class method 0.
 
         Args:
+            capsys: Pytest fixture that captures output
+
+        """
+        exp_stack: Deque[CallerInfo] = deque()
+        exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
+                                     cls_name='TestClassGetCallerInfo0',
+                                     func_name='test_get_caller_info_c0bt',
+                                     line_num=2567)
+        exp_stack.append(exp_caller_info)
+        update_stack(exp_stack=exp_stack, line_num=4327, add=0)
+        for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
+            try:
+                frame = _getframe(i)
+                caller_info = get_caller_info(frame)
+            finally:
+                del frame
+            assert caller_info == expected_caller_info
+
+        # test call sequence
+        update_stack(exp_stack=exp_stack, line_num=4334, add=0)
+        call_seq = get_formatted_call_sequence(depth=len(exp_stack))
+
+        assert call_seq == get_exp_seq(exp_stack=exp_stack)
+
+        # test diag_msg
+        update_stack(exp_stack=exp_stack, line_num=4341, add=0)
+        before_time = datetime.now()
+        diag_msg('message 1', 1, depth=len(exp_stack))
+        after_time = datetime.now()
+
+        diag_msg_args = TestDiagMsg.get_diag_msg_args(depth_arg=len(exp_stack),
+                                                      msg_arg=['message 1', 1])
+        verify_diag_msg(exp_stack=exp_stack,
+                        before_time=before_time,
+                        after_time=after_time,
+                        capsys=capsys,
+                        diag_msg_args=diag_msg_args)
+
+        # call module level function
+        update_stack(exp_stack=exp_stack, line_num=4354, add=0)
+        func_get_caller_info_1(exp_stack=exp_stack, capsys=capsys)
+
+        # call method
+        cls_get_caller_info1 = ClassGetCallerInfo1()
+        update_stack(exp_stack=exp_stack, line_num=4359, add=1)
+        cls_get_caller_info1.get_caller_info_m1(exp_stack=exp_stack,
+                                                capsys=capsys)
+
+        # call static method
+        update_stack(exp_stack=exp_stack, line_num=4364, add=1)
+        cls_get_caller_info1.get_caller_info_s1(exp_stack=exp_stack,
+                                                capsys=capsys)
+
+        # call class method
+        update_stack(exp_stack=exp_stack, line_num=4369, add=1)
+        ClassGetCallerInfo1.get_caller_info_c1(exp_stack=exp_stack,
+                                               capsys=capsys)
+
+        # call overloaded base class method
+        update_stack(exp_stack=exp_stack, line_num=4374, add=1)
+        cls_get_caller_info1.get_caller_info_m1bo(exp_stack=exp_stack,
+                                                  capsys=capsys)
+
+        # call overloaded base class static method
+        update_stack(exp_stack=exp_stack, line_num=4379, add=1)
+        cls_get_caller_info1.get_caller_info_s1bo(exp_stack=exp_stack,
+                                                  capsys=capsys)
+
+        # call overloaded base class class method
+        update_stack(exp_stack=exp_stack, line_num=4384, add=1)
+        ClassGetCallerInfo1.get_caller_info_c1bo(exp_stack=exp_stack,
+                                                 capsys=capsys)
+
+        # call subclass method
+        cls_get_caller_info1s = ClassGetCallerInfo1S()
+        update_stack(exp_stack=exp_stack, line_num=4390, add=1)
+        cls_get_caller_info1s.get_caller_info_m1s(exp_stack=exp_stack,
+                                                  capsys=capsys)
+
+        # call subclass static method
+        update_stack(exp_stack=exp_stack, line_num=4395, add=1)
+        cls_get_caller_info1s.get_caller_info_s1s(exp_stack=exp_stack,
+                                                  capsys=capsys)
+
+        # call subclass class method
+        update_stack(exp_stack=exp_stack, line_num=4400, add=1)
+        ClassGetCallerInfo1S.get_caller_info_c1s(exp_stack=exp_stack,
+                                                 capsys=capsys)
+
+        # call overloaded subclass method
+        update_stack(exp_stack=exp_stack, line_num=4405, add=1)
+        cls_get_caller_info1s.get_caller_info_m1bo(exp_stack=exp_stack,
+                                                   capsys=capsys)
+
+        # call overloaded subclass static method
+        update_stack(exp_stack=exp_stack, line_num=4410, add=1)
+        cls_get_caller_info1s.get_caller_info_s1bo(exp_stack=exp_stack,
+                                                   capsys=capsys)
+
+        # call overloaded subclass class method
+        update_stack(exp_stack=exp_stack, line_num=4415, add=1)
+        ClassGetCallerInfo1S.get_caller_info_c1bo(exp_stack=exp_stack,
+                                                  capsys=capsys)
+
+        # call base method from subclass method
+        update_stack(exp_stack=exp_stack, line_num=4420, add=1)
+        cls_get_caller_info1s.get_caller_info_m1sb(exp_stack=exp_stack,
+                                                   capsys=capsys)
+
+        # call base static method from subclass static method
+        update_stack(exp_stack=exp_stack, line_num=4425, add=1)
+        cls_get_caller_info1s.get_caller_info_s1sb(exp_stack=exp_stack,
+                                                   capsys=capsys)
+
+        # call base class method from subclass class method
+        update_stack(exp_stack=exp_stack, line_num=4430, add=1)
+        ClassGetCallerInfo1S.get_caller_info_c1sb(exp_stack=exp_stack,
+                                                  capsys=capsys)
+
+        exp_stack.pop()
+
+    ####################################################################
+    # Class 0 Method 10
+    ####################################################################
+    @classmethod
+    def get_caller_info_c0bt(cls,
+                             exp_stack: Optional[Deque[CallerInfo]],
+                             capsys: pytest.CaptureFixture[str]
+                             ) -> None:
+        """Get caller info overloaded class method 0.
+
+        Args:
             exp_stack: The expected call stack
             capsys: Pytest fixture that captures output
 
         """
         if not exp_stack:
             exp_stack = deque()
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='TestClassGetCallerInfo0',
-                                     func_name='test_get_caller_info_c0bt',
+                                     func_name='get_caller_info_c0bt',
                                      line_num=2567)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=4330, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4461, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=4337, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4468, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         # test diag_msg
-        update_stack(exp_stack=exp_stack, line_num=4344, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4475, add=0)
         before_time = datetime.now()
         diag_msg('message 1', 1, depth=len(exp_stack))
         after_time = datetime.now()
 
         diag_msg_args = TestDiagMsg.get_diag_msg_args(depth_arg=len(exp_stack),
                                                       msg_arg=['message 1', 1])
         verify_diag_msg(exp_stack=exp_stack,
                         before_time=before_time,
                         after_time=after_time,
                         capsys=capsys,
                         diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=4357, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4488, add=0)
         func_get_caller_info_1(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info1 = ClassGetCallerInfo1()
-        update_stack(exp_stack=exp_stack, line_num=4362, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4493, add=1)
         cls_get_caller_info1.get_caller_info_m1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=4367, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4498, add=1)
         cls_get_caller_info1.get_caller_info_s1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=4372, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4503, add=1)
         ClassGetCallerInfo1.get_caller_info_c1(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=4377, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4508, add=1)
         cls_get_caller_info1.get_caller_info_m1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=4382, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4513, add=1)
         cls_get_caller_info1.get_caller_info_s1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=4387, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4518, add=1)
         ClassGetCallerInfo1.get_caller_info_c1bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info1s = ClassGetCallerInfo1S()
-        update_stack(exp_stack=exp_stack, line_num=4393, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4524, add=1)
         cls_get_caller_info1s.get_caller_info_m1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=4398, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4529, add=1)
         cls_get_caller_info1s.get_caller_info_s1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=4403, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4534, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=4408, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4539, add=1)
         cls_get_caller_info1s.get_caller_info_m1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=4413, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4544, add=1)
         cls_get_caller_info1s.get_caller_info_s1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=4418, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4549, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=4423, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4554, add=1)
         cls_get_caller_info1s.get_caller_info_m1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=4428, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4559, add=1)
         cls_get_caller_info1s.get_caller_info_s1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=4433, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4564, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
 
 ########################################################################
@@ -4454,121 +4585,121 @@
         """
         exp_stack: Deque[CallerInfo] = deque()
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='TestClassGetCallerInfo0S',
                                      func_name='test_get_caller_info_m0s',
                                      line_num=2701)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=4465, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4596, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=4472, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4603, add=0)
         call_seq = get_formatted_call_sequence(depth=1)
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         # test diag_msg
-        update_stack(exp_stack=exp_stack, line_num=4479, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4610, add=0)
         before_time = datetime.now()
         diag_msg('message 1', 1, depth=1)
         after_time = datetime.now()
 
         diag_msg_args = TestDiagMsg.get_diag_msg_args(depth_arg=1,
                                                       msg_arg=['message 1', 1])
         verify_diag_msg(exp_stack=exp_stack,
                         before_time=before_time,
                         after_time=after_time,
                         capsys=capsys,
                         diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=4492, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4623, add=0)
         func_get_caller_info_1(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info1 = ClassGetCallerInfo1()
-        update_stack(exp_stack=exp_stack, line_num=4497, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4628, add=1)
         cls_get_caller_info1.get_caller_info_m1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=4502, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4633, add=1)
         cls_get_caller_info1.get_caller_info_s1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=4507, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4638, add=1)
         ClassGetCallerInfo1.get_caller_info_c1(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=4512, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4643, add=1)
         cls_get_caller_info1.get_caller_info_m1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=4517, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4648, add=1)
         cls_get_caller_info1.get_caller_info_s1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=4522, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4653, add=1)
         ClassGetCallerInfo1.get_caller_info_c1bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info1s = ClassGetCallerInfo1S()
-        update_stack(exp_stack=exp_stack, line_num=4528, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4659, add=1)
         cls_get_caller_info1s.get_caller_info_m1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=4533, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4664, add=1)
         cls_get_caller_info1s.get_caller_info_s1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=4538, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4669, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=4543, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4674, add=1)
         cls_get_caller_info1s.get_caller_info_m1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=4548, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4679, add=1)
         cls_get_caller_info1s.get_caller_info_s1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=4553, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4684, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=4558, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4689, add=1)
         cls_get_caller_info1s.get_caller_info_m1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=4563, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4694, add=1)
         cls_get_caller_info1s.get_caller_info_s1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=4568, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4699, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 0S Method 2
@@ -4583,121 +4714,121 @@
         """
         exp_stack: Deque[CallerInfo] = deque()
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='TestClassGetCallerInfo0S',
                                      func_name='test_get_caller_info_s0s',
                                      line_num=2829)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=4594, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4725, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=4601, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4732, add=0)
         call_seq = get_formatted_call_sequence(depth=1)
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         # test diag_msg
-        update_stack(exp_stack=exp_stack, line_num=4608, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4739, add=0)
         before_time = datetime.now()
         diag_msg('message 1', 1, depth=1)
         after_time = datetime.now()
 
         diag_msg_args = TestDiagMsg.get_diag_msg_args(depth_arg=1,
                                                       msg_arg=['message 1', 1])
         verify_diag_msg(exp_stack=exp_stack,
                         before_time=before_time,
                         after_time=after_time,
                         capsys=capsys,
                         diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=4621, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4752, add=0)
         func_get_caller_info_1(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info1 = ClassGetCallerInfo1()
-        update_stack(exp_stack=exp_stack, line_num=4626, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4757, add=1)
         cls_get_caller_info1.get_caller_info_m1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=4631, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4762, add=1)
         cls_get_caller_info1.get_caller_info_s1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=4636, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4767, add=1)
         ClassGetCallerInfo1.get_caller_info_c1(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=4641, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4772, add=1)
         cls_get_caller_info1.get_caller_info_m1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=4646, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4777, add=1)
         cls_get_caller_info1.get_caller_info_s1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=4651, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4782, add=1)
         ClassGetCallerInfo1.get_caller_info_c1bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info1s = ClassGetCallerInfo1S()
-        update_stack(exp_stack=exp_stack, line_num=4657, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4788, add=1)
         cls_get_caller_info1s.get_caller_info_m1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=4662, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4793, add=1)
         cls_get_caller_info1s.get_caller_info_s1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=4667, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4798, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=4672, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4803, add=1)
         cls_get_caller_info1s.get_caller_info_m1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=4677, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4808, add=1)
         cls_get_caller_info1s.get_caller_info_s1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=4682, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4813, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=4687, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4818, add=1)
         cls_get_caller_info1s.get_caller_info_m1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=4692, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4823, add=1)
         cls_get_caller_info1s.get_caller_info_s1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=4697, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4828, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 0S Method 3
@@ -4713,121 +4844,121 @@
         """
         exp_stack: Deque[CallerInfo] = deque()
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='TestClassGetCallerInfo0S',
                                      func_name='test_get_caller_info_c0s',
                                      line_num=2958)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=4724, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4855, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=4731, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4862, add=0)
         call_seq = get_formatted_call_sequence(depth=1)
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         # test diag_msg
-        update_stack(exp_stack=exp_stack, line_num=4738, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4869, add=0)
         before_time = datetime.now()
         diag_msg('message 1', 1, depth=1)
         after_time = datetime.now()
 
         diag_msg_args = TestDiagMsg.get_diag_msg_args(depth_arg=1,
                                                       msg_arg=['message 1', 1])
         verify_diag_msg(exp_stack=exp_stack,
                         before_time=before_time,
                         after_time=after_time,
                         capsys=capsys,
                         diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=4751, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4882, add=0)
         func_get_caller_info_1(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info1 = ClassGetCallerInfo1()
-        update_stack(exp_stack=exp_stack, line_num=4756, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4887, add=1)
         cls_get_caller_info1.get_caller_info_m1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=4761, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4892, add=1)
         cls_get_caller_info1.get_caller_info_s1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=4766, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4897, add=1)
         ClassGetCallerInfo1.get_caller_info_c1(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=4771, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4902, add=1)
         cls_get_caller_info1.get_caller_info_m1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=4776, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4907, add=1)
         cls_get_caller_info1.get_caller_info_s1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=4781, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4912, add=1)
         ClassGetCallerInfo1.get_caller_info_c1bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info1s = ClassGetCallerInfo1S()
-        update_stack(exp_stack=exp_stack, line_num=4787, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4918, add=1)
         cls_get_caller_info1s.get_caller_info_m1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=4792, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4923, add=1)
         cls_get_caller_info1s.get_caller_info_s1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=4797, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4928, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=4802, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4933, add=1)
         cls_get_caller_info1s.get_caller_info_m1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=4807, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4938, add=1)
         cls_get_caller_info1s.get_caller_info_s1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=4812, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4943, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=4817, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4948, add=1)
         cls_get_caller_info1s.get_caller_info_m1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=4822, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4953, add=1)
         cls_get_caller_info1s.get_caller_info_s1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=4827, add=1)
+        update_stack(exp_stack=exp_stack, line_num=4958, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 0S Method 4
@@ -4842,121 +4973,121 @@
         """
         exp_stack: Deque[CallerInfo] = deque()
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='TestClassGetCallerInfo0S',
                                      func_name='test_get_caller_info_m0bo',
                                      line_num=3086)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=4853, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4984, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=4860, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4991, add=0)
         call_seq = get_formatted_call_sequence(depth=1)
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         # test diag_msg
-        update_stack(exp_stack=exp_stack, line_num=4867, add=0)
+        update_stack(exp_stack=exp_stack, line_num=4998, add=0)
         before_time = datetime.now()
         diag_msg('message 1', 1, depth=1)
         after_time = datetime.now()
 
         diag_msg_args = TestDiagMsg.get_diag_msg_args(depth_arg=1,
                                                       msg_arg=['message 1', 1])
         verify_diag_msg(exp_stack=exp_stack,
                         before_time=before_time,
                         after_time=after_time,
                         capsys=capsys,
                         diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=4880, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5011, add=0)
         func_get_caller_info_1(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info1 = ClassGetCallerInfo1()
-        update_stack(exp_stack=exp_stack, line_num=4885, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5016, add=1)
         cls_get_caller_info1.get_caller_info_m1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=4890, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5021, add=1)
         cls_get_caller_info1.get_caller_info_s1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=4895, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5026, add=1)
         ClassGetCallerInfo1.get_caller_info_c1(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=4900, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5031, add=1)
         cls_get_caller_info1.get_caller_info_m1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=4905, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5036, add=1)
         cls_get_caller_info1.get_caller_info_s1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=4910, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5041, add=1)
         ClassGetCallerInfo1.get_caller_info_c1bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info1s = ClassGetCallerInfo1S()
-        update_stack(exp_stack=exp_stack, line_num=4916, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5047, add=1)
         cls_get_caller_info1s.get_caller_info_m1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=4921, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5052, add=1)
         cls_get_caller_info1s.get_caller_info_s1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=4926, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5057, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=4931, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5062, add=1)
         cls_get_caller_info1s.get_caller_info_m1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=4936, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5067, add=1)
         cls_get_caller_info1s.get_caller_info_s1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=4941, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5072, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=4946, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5077, add=1)
         cls_get_caller_info1s.get_caller_info_m1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=4951, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5082, add=1)
         cls_get_caller_info1s.get_caller_info_s1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=4956, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5087, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 0S Method 5
@@ -4971,121 +5102,121 @@
         """
         exp_stack: Deque[CallerInfo] = deque()
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='TestClassGetCallerInfo0S',
                                      func_name='test_get_caller_info_s0bo',
                                      line_num=3214)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=4982, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5113, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=4989, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5120, add=0)
         call_seq = get_formatted_call_sequence(depth=1)
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         # test diag_msg
-        update_stack(exp_stack=exp_stack, line_num=4996, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5127, add=0)
         before_time = datetime.now()
         diag_msg('message 1', 1, depth=1)
         after_time = datetime.now()
 
         diag_msg_args = TestDiagMsg.get_diag_msg_args(depth_arg=1,
                                                       msg_arg=['message 1', 1])
         verify_diag_msg(exp_stack=exp_stack,
                         before_time=before_time,
                         after_time=after_time,
                         capsys=capsys,
                         diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=5009, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5140, add=0)
         func_get_caller_info_1(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info1 = ClassGetCallerInfo1()
-        update_stack(exp_stack=exp_stack, line_num=5014, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5145, add=1)
         cls_get_caller_info1.get_caller_info_m1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=5019, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5150, add=1)
         cls_get_caller_info1.get_caller_info_s1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=5024, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5155, add=1)
         ClassGetCallerInfo1.get_caller_info_c1(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=5029, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5160, add=1)
         cls_get_caller_info1.get_caller_info_m1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=5034, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5165, add=1)
         cls_get_caller_info1.get_caller_info_s1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=5039, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5170, add=1)
         ClassGetCallerInfo1.get_caller_info_c1bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info1s = ClassGetCallerInfo1S()
-        update_stack(exp_stack=exp_stack, line_num=5045, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5176, add=1)
         cls_get_caller_info1s.get_caller_info_m1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5050, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5181, add=1)
         cls_get_caller_info1s.get_caller_info_s1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5055, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5186, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=5060, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5191, add=1)
         cls_get_caller_info1s.get_caller_info_m1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5065, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5196, add=1)
         cls_get_caller_info1s.get_caller_info_s1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5070, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5201, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=5075, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5206, add=1)
         cls_get_caller_info1s.get_caller_info_m1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5080, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5211, add=1)
         cls_get_caller_info1s.get_caller_info_s1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5085, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5216, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 0S Method 6
@@ -5101,121 +5232,121 @@
         """
         exp_stack: Deque[CallerInfo] = deque()
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='TestClassGetCallerInfo0S',
                                      func_name='test_get_caller_info_c0bo',
                                      line_num=3343)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=5112, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5243, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=5119, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5250, add=0)
         call_seq = get_formatted_call_sequence(depth=1)
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         # test diag_msg
-        update_stack(exp_stack=exp_stack, line_num=5126, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5257, add=0)
         before_time = datetime.now()
         diag_msg('message 1', 1, depth=1)
         after_time = datetime.now()
 
         diag_msg_args = TestDiagMsg.get_diag_msg_args(depth_arg=1,
                                                       msg_arg=['message 1', 1])
         verify_diag_msg(exp_stack=exp_stack,
                         before_time=before_time,
                         after_time=after_time,
                         capsys=capsys,
                         diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=5139, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5270, add=0)
         func_get_caller_info_1(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info1 = ClassGetCallerInfo1()
-        update_stack(exp_stack=exp_stack, line_num=5144, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5275, add=1)
         cls_get_caller_info1.get_caller_info_m1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=5149, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5280, add=1)
         cls_get_caller_info1.get_caller_info_s1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=5154, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5285, add=1)
         ClassGetCallerInfo1.get_caller_info_c1(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=5159, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5290, add=1)
         cls_get_caller_info1.get_caller_info_m1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=5164, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5295, add=1)
         cls_get_caller_info1.get_caller_info_s1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=5169, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5300, add=1)
         ClassGetCallerInfo1.get_caller_info_c1bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info1s = ClassGetCallerInfo1S()
-        update_stack(exp_stack=exp_stack, line_num=5175, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5306, add=1)
         cls_get_caller_info1s.get_caller_info_m1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5180, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5311, add=1)
         cls_get_caller_info1s.get_caller_info_s1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5185, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5316, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=5190, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5321, add=1)
         cls_get_caller_info1s.get_caller_info_m1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5195, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5326, add=1)
         cls_get_caller_info1s.get_caller_info_s1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5200, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5331, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=5205, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5336, add=1)
         cls_get_caller_info1s.get_caller_info_m1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5210, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5341, add=1)
         cls_get_caller_info1s.get_caller_info_s1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5215, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5346, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 0S Method 7
@@ -5230,153 +5361,153 @@
         """
         exp_stack: Deque[CallerInfo] = deque()
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='TestClassGetCallerInfo0S',
                                      func_name='test_get_caller_info_m0sb',
                                      line_num=3471)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=5241, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5372, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=5248, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5379, add=0)
         call_seq = get_formatted_call_sequence(depth=1)
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         # test diag_msg
-        update_stack(exp_stack=exp_stack, line_num=5255, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5386, add=0)
         before_time = datetime.now()
         diag_msg('message 1', 1, depth=1)
         after_time = datetime.now()
 
         diag_msg_args = TestDiagMsg.get_diag_msg_args(depth_arg=1,
                                                       msg_arg=['message 1', 1])
         verify_diag_msg(exp_stack=exp_stack,
                         before_time=before_time,
                         after_time=after_time,
                         capsys=capsys,
                         diag_msg_args=diag_msg_args)
 
         # call base class normal method target
-        update_stack(exp_stack=exp_stack, line_num=5268, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5399, add=0)
         self.test_get_caller_info_m0bt(capsys=capsys)
         tst_cls_get_caller_info0 = TestClassGetCallerInfo0()
-        update_stack(exp_stack=exp_stack, line_num=5271, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5402, add=0)
         tst_cls_get_caller_info0.test_get_caller_info_m0bt(capsys=capsys)
         tst_cls_get_caller_info0s = TestClassGetCallerInfo0S()
-        update_stack(exp_stack=exp_stack, line_num=5274, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5405, add=0)
         tst_cls_get_caller_info0s.test_get_caller_info_m0bt(capsys=capsys)
 
         # call base class static method target
-        update_stack(exp_stack=exp_stack, line_num=5278, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5409, add=0)
         self.get_caller_info_s0bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=5280, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5411, add=0)
         super().get_caller_info_s0bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=5282, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5413, add=1)
         TestClassGetCallerInfo0.get_caller_info_s0bt(exp_stack=exp_stack,
                                                      capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=5285, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5416, add=1)
         TestClassGetCallerInfo0S.get_caller_info_s0bt(exp_stack=exp_stack,
                                                       capsys=capsys)
 
         # call base class class method target
-        update_stack(exp_stack=exp_stack, line_num=5290, add=0)
-        super().test_get_caller_info_c0bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=5292, add=1)
-        TestClassGetCallerInfo0.test_get_caller_info_c0bt(exp_stack=exp_stack,
-                                                          capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=5295, add=1)
-        TestClassGetCallerInfo0S.test_get_caller_info_c0bt(exp_stack=exp_stack,
-                                                           capsys=capsys)
+        update_stack(exp_stack=exp_stack, line_num=5421, add=0)
+        super().get_caller_info_c0bt(exp_stack=exp_stack, capsys=capsys)
+        update_stack(exp_stack=exp_stack, line_num=5423, add=1)
+        TestClassGetCallerInfo0.get_caller_info_c0bt(exp_stack=exp_stack,
+                                                     capsys=capsys)
+        update_stack(exp_stack=exp_stack, line_num=5426, add=1)
+        TestClassGetCallerInfo0S.get_caller_info_c0bt(exp_stack=exp_stack,
+                                                      capsys=capsys)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=5300, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5431, add=0)
         func_get_caller_info_1(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info1 = ClassGetCallerInfo1()
-        update_stack(exp_stack=exp_stack, line_num=5305, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5436, add=1)
         cls_get_caller_info1.get_caller_info_m1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=5310, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5441, add=1)
         cls_get_caller_info1.get_caller_info_s1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=5315, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5446, add=1)
         ClassGetCallerInfo1.get_caller_info_c1(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=5320, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5451, add=1)
         cls_get_caller_info1.get_caller_info_m1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=5325, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5456, add=1)
         cls_get_caller_info1.get_caller_info_s1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=5330, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5461, add=1)
         ClassGetCallerInfo1.get_caller_info_c1bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info1s = ClassGetCallerInfo1S()
-        update_stack(exp_stack=exp_stack, line_num=5336, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5467, add=1)
         cls_get_caller_info1s.get_caller_info_m1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5341, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5472, add=1)
         cls_get_caller_info1s.get_caller_info_s1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5346, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5477, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=5351, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5482, add=1)
         cls_get_caller_info1s.get_caller_info_m1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5356, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5487, add=1)
         cls_get_caller_info1s.get_caller_info_s1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5361, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5492, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=5366, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5497, add=1)
         cls_get_caller_info1s.get_caller_info_m1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5371, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5502, add=1)
         cls_get_caller_info1s.get_caller_info_s1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5376, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5507, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 0S Method 8
@@ -5391,145 +5522,145 @@
         """
         exp_stack: Deque[CallerInfo] = deque()
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='TestClassGetCallerInfo0S',
                                      func_name='test_get_caller_info_s0sb',
                                      line_num=3631)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=5402, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5533, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=5409, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5540, add=0)
         call_seq = get_formatted_call_sequence(depth=1)
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         # test diag_msg
-        update_stack(exp_stack=exp_stack, line_num=5416, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5547, add=0)
         before_time = datetime.now()
         diag_msg('message 1', 1, depth=1)
         after_time = datetime.now()
 
         diag_msg_args = TestDiagMsg.get_diag_msg_args(depth_arg=1,
                                                       msg_arg=['message 1', 1])
         verify_diag_msg(exp_stack=exp_stack,
                         before_time=before_time,
                         after_time=after_time,
                         capsys=capsys,
                         diag_msg_args=diag_msg_args)
 
         # call base class normal method target
         tst_cls_get_caller_info0 = TestClassGetCallerInfo0()
-        update_stack(exp_stack=exp_stack, line_num=5430, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5561, add=0)
         tst_cls_get_caller_info0.test_get_caller_info_m0bt(capsys=capsys)
         tst_cls_get_caller_info0s = TestClassGetCallerInfo0S()
-        update_stack(exp_stack=exp_stack, line_num=5433, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5564, add=0)
         tst_cls_get_caller_info0s.test_get_caller_info_m0bt(capsys=capsys)
 
         # call base class static method target
-        update_stack(exp_stack=exp_stack, line_num=5437, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5568, add=1)
         TestClassGetCallerInfo0.get_caller_info_s0bt(exp_stack=exp_stack,
                                                      capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=5440, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5571, add=1)
         TestClassGetCallerInfo0S.get_caller_info_s0bt(exp_stack=exp_stack,
                                                       capsys=capsys)
 
         # call base class class method target
-        update_stack(exp_stack=exp_stack, line_num=5445, add=1)
-        TestClassGetCallerInfo0.test_get_caller_info_c0bt(exp_stack=exp_stack,
-                                                          capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=5448, add=1)
-        TestClassGetCallerInfo0S.test_get_caller_info_c0bt(exp_stack=exp_stack,
-                                                           capsys=capsys)
+        update_stack(exp_stack=exp_stack, line_num=5576, add=1)
+        TestClassGetCallerInfo0.get_caller_info_c0bt(exp_stack=exp_stack,
+                                                     capsys=capsys)
+        update_stack(exp_stack=exp_stack, line_num=5579, add=1)
+        TestClassGetCallerInfo0S.get_caller_info_c0bt(exp_stack=exp_stack,
+                                                      capsys=capsys)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=5453, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5584, add=0)
         func_get_caller_info_1(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info1 = ClassGetCallerInfo1()
-        update_stack(exp_stack=exp_stack, line_num=5458, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5589, add=1)
         cls_get_caller_info1.get_caller_info_m1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=5463, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5594, add=1)
         cls_get_caller_info1.get_caller_info_s1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=5468, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5599, add=1)
         ClassGetCallerInfo1.get_caller_info_c1(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=5473, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5604, add=1)
         cls_get_caller_info1.get_caller_info_m1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=5478, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5609, add=1)
         cls_get_caller_info1.get_caller_info_s1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=5483, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5614, add=1)
         ClassGetCallerInfo1.get_caller_info_c1bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info1s = ClassGetCallerInfo1S()
-        update_stack(exp_stack=exp_stack, line_num=5489, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5620, add=1)
         cls_get_caller_info1s.get_caller_info_m1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5494, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5625, add=1)
         cls_get_caller_info1s.get_caller_info_s1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5499, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5630, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=5504, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5635, add=1)
         cls_get_caller_info1s.get_caller_info_m1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5509, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5640, add=1)
         cls_get_caller_info1s.get_caller_info_s1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5514, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5645, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=5519, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5650, add=1)
         cls_get_caller_info1s.get_caller_info_m1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5524, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5655, add=1)
         cls_get_caller_info1s.get_caller_info_s1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5529, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5660, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 0S Method 9
@@ -5545,141 +5676,141 @@
         """
         exp_stack: Deque[CallerInfo] = deque()
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='TestClassGetCallerInfo0S',
                                      func_name='test_get_caller_info_c0sb',
                                      line_num=3784)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=5556, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5687, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=5563, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5694, add=0)
         call_seq = get_formatted_call_sequence(depth=1)
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         # test diag_msg
-        update_stack(exp_stack=exp_stack, line_num=5570, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5701, add=0)
         before_time = datetime.now()
         diag_msg('message 1', 1, depth=1)
         after_time = datetime.now()
 
         diag_msg_args = TestDiagMsg.get_diag_msg_args(depth_arg=1,
                                                       msg_arg=['message 1', 1])
         verify_diag_msg(exp_stack=exp_stack,
                         before_time=before_time,
                         after_time=after_time,
                         capsys=capsys,
                         diag_msg_args=diag_msg_args)
 
         # call base class normal method target
         tst_cls_get_caller_info0 = TestClassGetCallerInfo0()
-        update_stack(exp_stack=exp_stack, line_num=5584, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5715, add=0)
         tst_cls_get_caller_info0.test_get_caller_info_m0bt(capsys=capsys)
         tst_cls_get_caller_info0s = TestClassGetCallerInfo0S()
-        update_stack(exp_stack=exp_stack, line_num=5587, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5718, add=0)
         tst_cls_get_caller_info0s.test_get_caller_info_m0bt(capsys=capsys)
 
         # call base class static method target
-        update_stack(exp_stack=exp_stack, line_num=5591, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5722, add=1)
         cls.get_caller_info_s0bt(exp_stack=exp_stack,
                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=5594, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5725, add=0)
         super().get_caller_info_s0bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=5596, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5727, add=1)
         TestClassGetCallerInfo0.get_caller_info_s0bt(exp_stack=exp_stack,
                                                      capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=5599, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5730, add=1)
         TestClassGetCallerInfo0S.get_caller_info_s0bt(exp_stack=exp_stack,
                                                       capsys=capsys)
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=5603, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5734, add=0)
         func_get_caller_info_1(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info1 = ClassGetCallerInfo1()
-        update_stack(exp_stack=exp_stack, line_num=5608, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5739, add=1)
         cls_get_caller_info1.get_caller_info_m1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=5613, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5744, add=1)
         cls_get_caller_info1.get_caller_info_s1(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=5618, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5749, add=1)
         ClassGetCallerInfo1.get_caller_info_c1(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=5623, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5754, add=1)
         cls_get_caller_info1.get_caller_info_m1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=5628, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5759, add=1)
         cls_get_caller_info1.get_caller_info_s1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=5633, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5764, add=1)
         ClassGetCallerInfo1.get_caller_info_c1bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info1s = ClassGetCallerInfo1S()
-        update_stack(exp_stack=exp_stack, line_num=5639, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5770, add=1)
         cls_get_caller_info1s.get_caller_info_m1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5644, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5775, add=1)
         cls_get_caller_info1s.get_caller_info_s1s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5649, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5780, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=5654, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5785, add=1)
         cls_get_caller_info1s.get_caller_info_m1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5659, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5790, add=1)
         cls_get_caller_info1s.get_caller_info_s1bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5664, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5795, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=5669, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5800, add=1)
         cls_get_caller_info1s.get_caller_info_m1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5674, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5805, add=1)
         cls_get_caller_info1s.get_caller_info_s1sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5679, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5810, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
 
 ########################################################################
@@ -5707,31 +5838,31 @@
         """
         self.var1 += 1
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1',
                                      func_name='get_caller_info_m1',
                                      line_num=3945)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=5718, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5849, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=5725, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5856, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=5732, add=0)
+            update_stack(exp_stack=exp_stack, line_num=5863, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -5739,91 +5870,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=5747, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5878, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=5752, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5883, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=5757, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5888, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=5762, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5893, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=5767, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5898, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=5772, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5903, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=5777, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5908, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=5783, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5914, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5788, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5919, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5793, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5924, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=5798, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5929, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5803, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5934, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5808, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5939, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=5813, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5944, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5818, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5949, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5823, add=1)
+        update_stack(exp_stack=exp_stack, line_num=5954, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 1 Method 2
@@ -5839,31 +5970,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1',
                                      func_name='get_caller_info_s1',
                                      line_num=4076)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=5850, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5981, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=5857, add=0)
+        update_stack(exp_stack=exp_stack, line_num=5988, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=5864, add=0)
+            update_stack(exp_stack=exp_stack, line_num=5995, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -5871,91 +6002,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=5879, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6010, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=5884, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6015, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=5889, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6020, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=5894, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6025, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=5899, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6030, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=5904, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6035, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=5909, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6040, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=5915, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6046, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5920, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6051, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5925, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6056, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=5930, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6061, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5935, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6066, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5940, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6071, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=5945, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6076, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=5950, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6081, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=5955, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6086, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 1 Method 3
@@ -5971,31 +6102,31 @@
             capsys: Pytest fixture that captures output
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1',
                                      func_name='get_caller_info_c1',
                                      line_num=4207)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=5982, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6113, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=5989, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6120, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=5996, add=0)
+            update_stack(exp_stack=exp_stack, line_num=6127, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -6003,91 +6134,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=6011, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6142, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=6016, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6147, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=6021, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6152, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=6026, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6157, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=6031, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6162, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=6036, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6167, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=6041, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6172, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=6047, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6178, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6052, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6183, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6057, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6188, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=6062, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6193, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6067, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6198, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6072, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6203, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=6077, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6208, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6082, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6213, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6087, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6218, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 1 Method 4
@@ -6103,31 +6234,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1',
                                      func_name='get_caller_info_m1bo',
                                      line_num=4338)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=6114, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6245, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=6121, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6252, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=6128, add=0)
+            update_stack(exp_stack=exp_stack, line_num=6259, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -6135,91 +6266,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=6143, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6274, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=6148, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6279, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=6153, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6284, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=6158, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6289, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=6163, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6294, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=6168, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6299, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=6173, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6304, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=6179, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6310, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6184, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6315, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6189, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6320, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=6194, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6325, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6199, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6330, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6204, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6335, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=6209, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6340, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6214, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6345, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6219, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6350, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 1 Method 5
@@ -6235,31 +6366,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1',
                                      func_name='get_caller_info_s1bo',
                                      line_num=4469)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=6246, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6377, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=6253, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6384, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=6260, add=0)
+            update_stack(exp_stack=exp_stack, line_num=6391, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -6267,91 +6398,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=6275, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6406, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=6280, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6411, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=6285, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6416, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=6290, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6421, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=6295, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6426, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=6300, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6431, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=6305, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6436, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=6311, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6442, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6316, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6447, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6321, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6452, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=6326, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6457, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6331, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6462, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6336, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6467, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=6341, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6472, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6346, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6477, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6351, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6482, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 1 Method 6
@@ -6368,31 +6499,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1',
                                      func_name='get_caller_info_c1bo',
                                      line_num=4601)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=6379, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6510, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=6386, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6517, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=6393, add=0)
+            update_stack(exp_stack=exp_stack, line_num=6524, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -6400,91 +6531,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=6408, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6539, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=6413, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6544, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=6418, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6549, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=6423, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6554, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=6428, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6559, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=6433, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6564, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=6438, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6569, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=6444, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6575, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6449, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6580, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6454, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6585, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=6459, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6590, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6464, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6595, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6469, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6600, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=6474, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6605, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6479, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6610, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6484, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6615, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 1 Method 7
@@ -6501,31 +6632,31 @@
         """
         self.var1 += 1
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1',
                                      func_name='get_caller_info_m1bt',
                                      line_num=4733)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=6512, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6643, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=6519, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6650, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=6526, add=0)
+            update_stack(exp_stack=exp_stack, line_num=6657, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -6533,91 +6664,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=6541, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6672, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=6546, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6677, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=6551, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6682, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=6556, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6687, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=6561, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6692, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=6566, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6697, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=6571, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6702, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=6577, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6708, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6582, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6713, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6587, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6718, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=6592, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6723, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6597, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6728, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6602, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6733, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=6607, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6738, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6612, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6743, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6617, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6748, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 1 Method 8
@@ -6633,31 +6764,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1',
                                      func_name='get_caller_info_s1bt',
                                      line_num=4864)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=6644, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6775, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=6651, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6782, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=6658, add=0)
+            update_stack(exp_stack=exp_stack, line_num=6789, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -6665,91 +6796,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=6673, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6804, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=6678, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6809, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=6683, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6814, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=6688, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6819, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=6693, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6824, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=6698, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6829, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=6703, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6834, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=6709, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6840, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6714, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6845, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6719, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6850, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=6724, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6855, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6729, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6860, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6734, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6865, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=6739, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6870, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6744, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6875, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6749, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6880, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 1 Method 9
@@ -6766,31 +6897,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1',
                                      func_name='get_caller_info_c1bt',
                                      line_num=4996)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=6777, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6908, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=6784, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6915, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=6791, add=0)
+            update_stack(exp_stack=exp_stack, line_num=6922, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -6798,91 +6929,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=6806, add=0)
+        update_stack(exp_stack=exp_stack, line_num=6937, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=6811, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6942, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=6816, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6947, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=6821, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6952, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=6826, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6957, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=6831, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6962, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=6836, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6967, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=6842, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6973, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6847, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6978, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6852, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6983, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=6857, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6988, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6862, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6993, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6867, add=1)
+        update_stack(exp_stack=exp_stack, line_num=6998, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=6872, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7003, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6877, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7008, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6882, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7013, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
 
 ########################################################################
@@ -6910,31 +7041,31 @@
         """
         self.var1 += 1
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1S',
                                      func_name='get_caller_info_m1s',
                                      line_num=5139)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=6921, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7052, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=6928, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7059, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=6935, add=0)
+            update_stack(exp_stack=exp_stack, line_num=7066, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -6942,91 +7073,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=6950, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7081, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=6955, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7086, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=6960, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7091, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=6965, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7096, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=6970, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7101, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=6975, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7106, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=6980, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7111, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=6986, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7117, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=6991, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7122, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=6996, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7127, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=7001, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7132, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7006, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7137, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7011, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7142, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=7016, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7147, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7021, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7152, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7026, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7157, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 1S Method 2
@@ -7042,31 +7173,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1S',
                                      func_name='get_caller_info_s1s',
                                      line_num=5270)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=7053, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7184, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=7060, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7191, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=7067, add=0)
+            update_stack(exp_stack=exp_stack, line_num=7198, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -7074,91 +7205,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=7082, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7213, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=7087, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7218, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=7092, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7223, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=7097, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7228, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=7102, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7233, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=7107, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7238, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=7112, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7243, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=7118, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7249, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7123, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7254, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7128, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7259, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=7133, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7264, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7138, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7269, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7143, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7274, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=7148, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7279, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7153, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7284, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7158, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7289, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 1S Method 3
@@ -7175,31 +7306,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1S',
                                      func_name='get_caller_info_c1s',
                                      line_num=5402)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=7186, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7317, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=7193, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7324, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=7200, add=0)
+            update_stack(exp_stack=exp_stack, line_num=7331, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -7207,91 +7338,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=7215, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7346, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=7220, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7351, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=7225, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7356, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=7230, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7361, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=7235, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7366, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=7240, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7371, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=7245, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7376, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=7251, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7382, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7256, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7387, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7261, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7392, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=7266, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7397, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7271, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7402, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7276, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7407, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=7281, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7412, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7286, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7417, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7291, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7422, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 1S Method 4
@@ -7307,31 +7438,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1S',
                                      func_name='get_caller_info_m1bo',
                                      line_num=5533)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=7318, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7449, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=7325, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7456, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=7332, add=0)
+            update_stack(exp_stack=exp_stack, line_num=7463, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -7339,91 +7470,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=7347, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7478, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=7352, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7483, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=7357, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7488, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=7362, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7493, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=7367, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7498, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=7372, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7503, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=7377, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7508, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=7383, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7514, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7388, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7519, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7393, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7524, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=7398, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7529, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7403, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7534, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7408, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7539, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=7413, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7544, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7418, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7549, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7423, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7554, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 1S Method 5
@@ -7439,31 +7570,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1S',
                                      func_name='get_caller_info_s1bo',
                                      line_num=5664)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=7450, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7581, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=7457, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7588, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=7464, add=0)
+            update_stack(exp_stack=exp_stack, line_num=7595, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -7471,91 +7602,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=7479, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7610, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=7484, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7615, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=7489, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7620, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=7494, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7625, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=7499, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7630, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=7504, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7635, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=7509, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7640, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=7515, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7646, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7520, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7651, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7525, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7656, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=7530, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7661, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7535, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7666, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7540, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7671, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=7545, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7676, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7550, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7681, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7555, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7686, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 1S Method 6
@@ -7572,31 +7703,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1S',
                                      func_name='get_caller_info_c1bo',
                                      line_num=5796)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=7583, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7714, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=7590, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7721, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=7597, add=0)
+            update_stack(exp_stack=exp_stack, line_num=7728, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -7604,91 +7735,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=7612, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7743, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=7617, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7748, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=7622, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7753, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=7627, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7758, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=7632, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7763, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=7637, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7768, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=7642, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7773, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=7648, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7779, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7653, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7784, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7658, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7789, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=7663, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7794, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7668, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7799, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7673, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7804, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=7678, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7809, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7683, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7814, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7688, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7819, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 1S Method 7
@@ -7704,31 +7835,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1S',
                                      func_name='get_caller_info_m1sb',
                                      line_num=5927)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=7715, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7846, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=7722, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7853, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=7729, add=0)
+            update_stack(exp_stack=exp_stack, line_num=7860, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -7736,125 +7867,125 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call base class normal method target
-        update_stack(exp_stack=exp_stack, line_num=7744, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7875, add=0)
         self.get_caller_info_m1bt(exp_stack=exp_stack, capsys=capsys)
         cls_get_caller_info1 = ClassGetCallerInfo1()
-        update_stack(exp_stack=exp_stack, line_num=7747, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7878, add=1)
         cls_get_caller_info1.get_caller_info_m1bt(exp_stack=exp_stack,
                                                   capsys=capsys)
         cls_get_caller_info1s = ClassGetCallerInfo1S()
-        update_stack(exp_stack=exp_stack, line_num=7751, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7882, add=1)
         cls_get_caller_info1s.get_caller_info_m1bt(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class static method target
-        update_stack(exp_stack=exp_stack, line_num=7756, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7887, add=0)
         self.get_caller_info_s1bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=7758, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7889, add=0)
         super().get_caller_info_s1bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=7760, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7891, add=1)
         ClassGetCallerInfo1.get_caller_info_s1bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=7763, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7894, add=1)
         ClassGetCallerInfo1S.get_caller_info_s1bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base class class method target
-        update_stack(exp_stack=exp_stack, line_num=7768, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7899, add=0)
         super().get_caller_info_c1bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=7770, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7901, add=1)
         ClassGetCallerInfo1.get_caller_info_c1bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=7773, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7904, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=7778, add=0)
+        update_stack(exp_stack=exp_stack, line_num=7909, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=7783, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7914, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=7788, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7919, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=7793, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7924, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=7798, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7929, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=7803, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7934, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=7808, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7939, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=7814, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7945, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7819, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7950, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7824, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7955, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=7829, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7960, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7834, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7965, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7839, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7970, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=7844, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7975, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7849, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7980, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7854, add=1)
+        update_stack(exp_stack=exp_stack, line_num=7985, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 1S Method 8
@@ -7870,31 +8001,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1S',
                                      func_name='get_caller_info_s1sb',
                                      line_num=6092)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=7881, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8012, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=7888, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8019, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=7895, add=0)
+            update_stack(exp_stack=exp_stack, line_num=8026, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -7903,116 +8034,116 @@
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call base class normal method target
         cls_get_caller_info1 = ClassGetCallerInfo1()
-        update_stack(exp_stack=exp_stack, line_num=7911, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8042, add=1)
         cls_get_caller_info1.get_caller_info_m1bt(exp_stack=exp_stack,
                                                   capsys=capsys)
         cls_get_caller_info1s = ClassGetCallerInfo1S()
-        update_stack(exp_stack=exp_stack, line_num=7915, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8046, add=1)
         cls_get_caller_info1s.get_caller_info_m1bt(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class static method target
-        update_stack(exp_stack=exp_stack, line_num=7920, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8051, add=1)
         ClassGetCallerInfo1.get_caller_info_s1bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=7923, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8054, add=1)
         ClassGetCallerInfo1S.get_caller_info_s1bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base class class method target
-        update_stack(exp_stack=exp_stack, line_num=7928, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8059, add=1)
         ClassGetCallerInfo1.get_caller_info_c1bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=7931, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8062, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=7936, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8067, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=7941, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8072, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=7946, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8077, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=7951, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8082, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=7956, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8087, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=7961, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8092, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=7966, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8097, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=7972, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8103, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7977, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8108, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7982, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8113, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=7987, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8118, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=7992, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8123, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=7997, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8128, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=8002, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8133, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8007, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8138, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8012, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8143, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 1S Method 9
@@ -8029,31 +8160,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo1S',
                                      func_name='get_caller_info_c1sb',
                                      line_num=6250)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=8040, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8171, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=8047, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8178, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=8054, add=0)
+            update_stack(exp_stack=exp_stack, line_num=8185, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -8062,125 +8193,125 @@
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call base class normal method target
         cls_get_caller_info1 = ClassGetCallerInfo1()
-        update_stack(exp_stack=exp_stack, line_num=8070, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8201, add=1)
         cls_get_caller_info1.get_caller_info_m1bt(exp_stack=exp_stack,
                                                   capsys=capsys)
         cls_get_caller_info1s = ClassGetCallerInfo1S()
-        update_stack(exp_stack=exp_stack, line_num=8074, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8205, add=1)
         cls_get_caller_info1s.get_caller_info_m1bt(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class static method target
-        update_stack(exp_stack=exp_stack, line_num=8079, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8210, add=1)
         cls.get_caller_info_s1bt(exp_stack=exp_stack,
                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=8082, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8213, add=0)
         super().get_caller_info_s1bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=8084, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8215, add=1)
         ClassGetCallerInfo1.get_caller_info_s1bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=8087, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8218, add=1)
         ClassGetCallerInfo1S.get_caller_info_s1bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base class class method target
-        update_stack(exp_stack=exp_stack, line_num=8092, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8223, add=0)
         cls.get_caller_info_c1bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=8094, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8225, add=0)
         super().get_caller_info_c1bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=8096, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8227, add=1)
         ClassGetCallerInfo1.get_caller_info_c1bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=8099, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8230, add=1)
         ClassGetCallerInfo1S.get_caller_info_c1bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=8104, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8235, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=8109, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8240, add=1)
         cls_get_caller_info2.get_caller_info_m2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=8114, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8245, add=1)
         cls_get_caller_info2.get_caller_info_s2(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=8119, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8250, add=1)
         ClassGetCallerInfo2.get_caller_info_c2(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=8124, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8255, add=1)
         cls_get_caller_info2.get_caller_info_m2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=8129, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8260, add=1)
         cls_get_caller_info2.get_caller_info_s2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=8134, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8265, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=8140, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8271, add=1)
         cls_get_caller_info2s.get_caller_info_m2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8145, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8276, add=1)
         cls_get_caller_info2s.get_caller_info_s2s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8150, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8281, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=8155, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8286, add=1)
         cls_get_caller_info2s.get_caller_info_m2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8160, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8291, add=1)
         cls_get_caller_info2s.get_caller_info_s2bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8165, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8296, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=8170, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8301, add=1)
         cls_get_caller_info2s.get_caller_info_m2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8175, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8306, add=1)
         cls_get_caller_info2s.get_caller_info_s2sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8180, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8311, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
 
 ########################################################################
@@ -8208,31 +8339,31 @@
         """
         self.var1 += 1
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2',
                                      func_name='get_caller_info_m2',
                                      line_num=6428)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=8219, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8350, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=8226, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8357, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=8233, add=0)
+            update_stack(exp_stack=exp_stack, line_num=8364, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -8240,91 +8371,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=8248, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8379, add=0)
         func_get_caller_info_3(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=8253, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8384, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=8258, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8389, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=8263, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8394, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=8268, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8399, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=8273, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8404, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=8278, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8409, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=8284, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8415, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8289, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8420, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8294, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8425, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=8299, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8430, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8304, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8435, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8309, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8440, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=8314, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8445, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8319, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8450, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8324, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8455, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 2 Method 2
@@ -8340,31 +8471,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2',
                                      func_name='get_caller_info_s2',
                                      line_num=6559)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=8351, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8482, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=8358, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8489, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=8365, add=0)
+            update_stack(exp_stack=exp_stack, line_num=8496, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -8372,91 +8503,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=8380, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8511, add=0)
         func_get_caller_info_3(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=8385, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8516, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=8390, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8521, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=8395, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8526, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=8400, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8531, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=8405, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8536, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=8410, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8541, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=8416, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8547, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8421, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8552, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8426, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8557, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=8431, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8562, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8436, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8567, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8441, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8572, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=8446, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8577, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8451, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8582, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8456, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8587, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 2 Method 3
@@ -8472,31 +8603,31 @@
             capsys: Pytest fixture that captures output
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2',
                                      func_name='get_caller_info_c2',
                                      line_num=6690)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=8483, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8614, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=8490, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8621, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=8497, add=0)
+            update_stack(exp_stack=exp_stack, line_num=8628, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -8504,91 +8635,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=8512, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8643, add=0)
         func_get_caller_info_3(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=8517, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8648, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=8522, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8653, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=8527, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8658, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=8532, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8663, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=8537, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8668, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=8542, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8673, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=8548, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8679, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8553, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8684, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8558, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8689, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=8563, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8694, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8568, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8699, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8573, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8704, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=8578, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8709, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8583, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8714, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8588, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8719, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 2 Method 4
@@ -8604,31 +8735,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2',
                                      func_name='get_caller_info_m2bo',
                                      line_num=6821)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=8615, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8746, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=8622, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8753, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=8629, add=0)
+            update_stack(exp_stack=exp_stack, line_num=8760, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -8636,91 +8767,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=8644, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8775, add=0)
         func_get_caller_info_3(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=8649, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8780, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=8654, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8785, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=8659, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8790, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=8664, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8795, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=8669, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8800, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=8674, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8805, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=8680, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8811, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8685, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8816, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8690, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8821, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=8695, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8826, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8700, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8831, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8705, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8836, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=8710, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8841, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8715, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8846, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8720, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8851, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 2 Method 5
@@ -8736,31 +8867,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2',
                                      func_name='get_caller_info_s2bo',
                                      line_num=6952)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=8747, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8878, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=8754, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8885, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=8761, add=0)
+            update_stack(exp_stack=exp_stack, line_num=8892, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -8768,91 +8899,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=8776, add=0)
+        update_stack(exp_stack=exp_stack, line_num=8907, add=0)
         func_get_caller_info_3(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=8781, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8912, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=8786, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8917, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=8791, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8922, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=8796, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8927, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=8801, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8932, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=8806, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8937, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=8812, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8943, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8817, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8948, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8822, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8953, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=8827, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8958, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8832, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8963, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8837, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8968, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=8842, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8973, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8847, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8978, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8852, add=1)
+        update_stack(exp_stack=exp_stack, line_num=8983, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 2 Method 6
@@ -8869,31 +9000,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2',
                                      func_name='get_caller_info_c2bo',
                                      line_num=7084)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=8880, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9011, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=8887, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9018, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=8894, add=0)
+            update_stack(exp_stack=exp_stack, line_num=9025, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -8901,91 +9032,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=8909, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9040, add=0)
         func_get_caller_info_3(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=8914, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9045, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=8919, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9050, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=8924, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9055, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=8929, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9060, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=8934, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9065, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=8939, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9070, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=8945, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9076, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8950, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9081, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8955, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9086, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=8960, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9091, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8965, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9096, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8970, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9101, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=8975, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9106, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=8980, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9111, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=8985, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9116, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 2 Method 7
@@ -9002,31 +9133,31 @@
         """
         self.var1 += 1
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2',
                                      func_name='get_caller_info_m2bt',
                                      line_num=7216)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=9013, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9144, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=9020, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9151, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=9027, add=0)
+            update_stack(exp_stack=exp_stack, line_num=9158, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -9034,91 +9165,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=9042, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9173, add=0)
         func_get_caller_info_3(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=9047, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9178, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=9052, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9183, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=9057, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9188, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=9062, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9193, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=9067, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9198, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=9072, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9203, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=9078, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9209, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9083, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9214, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9088, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9219, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=9093, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9224, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9098, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9229, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9103, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9234, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=9108, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9239, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9113, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9244, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9118, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9249, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 2 Method 8
@@ -9134,31 +9265,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2',
                                      func_name='get_caller_info_s2bt',
                                      line_num=7347)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=9145, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9276, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=9152, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9283, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=9159, add=0)
+            update_stack(exp_stack=exp_stack, line_num=9290, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -9166,91 +9297,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=9174, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9305, add=0)
         func_get_caller_info_3(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=9179, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9310, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=9184, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9315, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=9189, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9320, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=9194, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9325, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=9199, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9330, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=9204, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9335, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=9210, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9341, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9215, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9346, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9220, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9351, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=9225, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9356, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9230, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9361, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9235, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9366, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=9240, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9371, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9245, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9376, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9250, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9381, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 2 Method 9
@@ -9267,31 +9398,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2',
                                      func_name='get_caller_info_c2bt',
                                      line_num=7479)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=9278, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9409, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=9285, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9416, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=9292, add=0)
+            update_stack(exp_stack=exp_stack, line_num=9423, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -9299,91 +9430,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=9307, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9438, add=0)
         func_get_caller_info_3(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=9312, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9443, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=9317, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9448, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=9322, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9453, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=9327, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9458, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=9332, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9463, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=9337, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9468, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=9343, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9474, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9348, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9479, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9353, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9484, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=9358, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9489, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9363, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9494, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9368, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9499, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=9373, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9504, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9378, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9509, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9383, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9514, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
 
 ########################################################################
@@ -9411,31 +9542,31 @@
         """
         self.var1 += 1
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2S',
                                      func_name='get_caller_info_m2s',
                                      line_num=7622)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=9422, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9553, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=9429, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9560, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=9436, add=0)
+            update_stack(exp_stack=exp_stack, line_num=9567, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -9443,91 +9574,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=9451, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9582, add=0)
         func_get_caller_info_3(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=9456, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9587, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=9461, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9592, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=9466, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9597, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=9471, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9602, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=9476, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9607, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=9481, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9612, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=9487, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9618, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9492, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9623, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9497, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9628, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=9502, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9633, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9507, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9638, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9512, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9643, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=9517, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9648, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9522, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9653, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9527, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9658, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 2S Method 2
@@ -9543,31 +9674,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2S',
                                      func_name='get_caller_info_s2s',
                                      line_num=7753)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=9554, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9685, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=9561, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9692, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=9568, add=0)
+            update_stack(exp_stack=exp_stack, line_num=9699, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -9575,91 +9706,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=9583, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9714, add=0)
         func_get_caller_info_3(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=9588, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9719, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=9593, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9724, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=9598, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9729, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=9603, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9734, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=9608, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9739, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=9613, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9744, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=9619, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9750, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9624, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9755, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9629, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9760, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=9634, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9765, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9639, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9770, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9644, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9775, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=9649, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9780, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9654, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9785, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9659, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9790, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 2S Method 3
@@ -9676,31 +9807,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2S',
                                      func_name='get_caller_info_c2s',
                                      line_num=7885)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=9687, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9818, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=9694, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9825, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=9701, add=0)
+            update_stack(exp_stack=exp_stack, line_num=9832, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -9708,91 +9839,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=9716, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9847, add=0)
         func_get_caller_info_3(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=9721, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9852, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=9726, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9857, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=9731, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9862, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=9736, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9867, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=9741, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9872, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=9746, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9877, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=9752, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9883, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9757, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9888, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9762, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9893, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=9767, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9898, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9772, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9903, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9777, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9908, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=9782, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9913, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9787, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9918, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9792, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9923, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 2S Method 4
@@ -9808,31 +9939,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2S',
                                      func_name='get_caller_info_m2bo',
                                      line_num=8016)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=9819, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9950, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=9826, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9957, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=9833, add=0)
+            update_stack(exp_stack=exp_stack, line_num=9964, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -9840,91 +9971,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=9848, add=0)
+        update_stack(exp_stack=exp_stack, line_num=9979, add=0)
         func_get_caller_info_3(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=9853, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9984, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=9858, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9989, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=9863, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9994, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=9868, add=1)
+        update_stack(exp_stack=exp_stack, line_num=9999, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=9873, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10004, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=9878, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10009, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=9884, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10015, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9889, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10020, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9894, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10025, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=9899, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10030, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9904, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10035, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9909, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10040, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=9914, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10045, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=9919, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10050, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=9924, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10055, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 2S Method 5
@@ -9940,31 +10071,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2S',
                                      func_name='get_caller_info_s2bo',
                                      line_num=8147)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=9951, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10082, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=9958, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10089, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=9965, add=0)
+            update_stack(exp_stack=exp_stack, line_num=10096, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -9972,91 +10103,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=9980, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10111, add=0)
         func_get_caller_info_3(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=9985, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10116, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=9990, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10121, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=9995, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10126, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=10000, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10131, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=10005, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10136, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=10010, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10141, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=10016, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10147, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=10021, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10152, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=10026, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10157, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=10031, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10162, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=10036, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10167, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=10041, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10172, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=10046, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10177, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=10051, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10182, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=10056, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10187, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 2S Method 6
@@ -10073,31 +10204,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2S',
                                      func_name='get_caller_info_c2bo',
                                      line_num=8279)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=10084, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10215, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=10091, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10222, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=10098, add=0)
+            update_stack(exp_stack=exp_stack, line_num=10229, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -10105,91 +10236,91 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=10113, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10244, add=0)
         func_get_caller_info_3(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=10118, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10249, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=10123, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10254, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=10128, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10259, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=10133, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10264, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=10138, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10269, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=10143, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10274, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=10149, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10280, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=10154, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10285, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=10159, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10290, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=10164, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10295, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=10169, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10300, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=10174, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10305, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=10179, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10310, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=10184, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10315, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=10189, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10320, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 2S Method 7
@@ -10205,31 +10336,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2S',
                                      func_name='get_caller_info_m2sb',
                                      line_num=8410)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=10216, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10347, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=10223, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10354, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=10230, add=0)
+            update_stack(exp_stack=exp_stack, line_num=10361, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -10237,125 +10368,125 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call base class normal method target
-        update_stack(exp_stack=exp_stack, line_num=10245, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10376, add=0)
         self.get_caller_info_m2bt(exp_stack=exp_stack, capsys=capsys)
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=10248, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10379, add=1)
         cls_get_caller_info2.get_caller_info_m2bt(exp_stack=exp_stack,
                                                   capsys=capsys)
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=10252, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10383, add=1)
         cls_get_caller_info2s.get_caller_info_m2bt(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class static method target
-        update_stack(exp_stack=exp_stack, line_num=10257, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10388, add=0)
         self.get_caller_info_s2bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=10259, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10390, add=0)
         super().get_caller_info_s2bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=10261, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10392, add=1)
         ClassGetCallerInfo2.get_caller_info_s2bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=10264, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10395, add=1)
         ClassGetCallerInfo2S.get_caller_info_s2bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base class class method target
-        update_stack(exp_stack=exp_stack, line_num=10269, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10400, add=0)
         super().get_caller_info_c2bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=10271, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10402, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=10274, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10405, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=10279, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10410, add=0)
         func_get_caller_info_2(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=10284, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10415, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=10289, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10420, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=10294, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10425, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=10299, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10430, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=10304, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10435, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=10309, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10440, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=10315, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10446, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=10320, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10451, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=10325, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10456, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=10330, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10461, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=10335, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10466, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=10340, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10471, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=10345, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10476, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=10350, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10481, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=10355, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10486, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 2S Method 8
@@ -10371,31 +10502,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2S',
                                      func_name='get_caller_info_s2sb',
                                      line_num=8575)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=10382, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10513, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=10389, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10520, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=10396, add=0)
+            update_stack(exp_stack=exp_stack, line_num=10527, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -10404,116 +10535,116 @@
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call base class normal method target
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=10412, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10543, add=1)
         cls_get_caller_info2.get_caller_info_m2bt(exp_stack=exp_stack,
                                                   capsys=capsys)
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=10416, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10547, add=1)
         cls_get_caller_info2s.get_caller_info_m2bt(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class static method target
-        update_stack(exp_stack=exp_stack, line_num=10421, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10552, add=1)
         ClassGetCallerInfo2.get_caller_info_s2bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=10424, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10555, add=1)
         ClassGetCallerInfo2S.get_caller_info_s2bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base class class method target
-        update_stack(exp_stack=exp_stack, line_num=10429, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10560, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=10432, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10563, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=10437, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10568, add=0)
         func_get_caller_info_3(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=10442, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10573, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=10447, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10578, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=10452, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10583, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=10457, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10588, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=10462, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10593, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=10467, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10598, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=10473, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10604, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=10478, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10609, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=10483, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10614, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=10488, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10619, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=10493, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10624, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=10498, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10629, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=10503, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10634, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=10508, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10639, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=10513, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10644, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 2S Method 9
@@ -10530,31 +10661,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo2S',
                                      func_name='get_caller_info_c2sb',
                                      line_num=8733)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=10541, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10672, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=10548, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10679, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=10555, add=0)
+            update_stack(exp_stack=exp_stack, line_num=10686, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -10563,125 +10694,125 @@
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call base class normal method target
         cls_get_caller_info2 = ClassGetCallerInfo2()
-        update_stack(exp_stack=exp_stack, line_num=10571, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10702, add=1)
         cls_get_caller_info2.get_caller_info_m2bt(exp_stack=exp_stack,
                                                   capsys=capsys)
         cls_get_caller_info2s = ClassGetCallerInfo2S()
-        update_stack(exp_stack=exp_stack, line_num=10575, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10706, add=1)
         cls_get_caller_info2s.get_caller_info_m2bt(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class static method target
-        update_stack(exp_stack=exp_stack, line_num=10580, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10711, add=1)
         cls.get_caller_info_s2bt(exp_stack=exp_stack,
                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=10583, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10714, add=0)
         super().get_caller_info_s2bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=10585, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10716, add=1)
         ClassGetCallerInfo2.get_caller_info_s2bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=10588, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10719, add=1)
         ClassGetCallerInfo2S.get_caller_info_s2bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base class class method target
-        update_stack(exp_stack=exp_stack, line_num=10593, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10724, add=0)
         cls.get_caller_info_c2bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=10595, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10726, add=0)
         super().get_caller_info_c2bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=10597, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10728, add=1)
         ClassGetCallerInfo2.get_caller_info_c2bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=10600, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10731, add=1)
         ClassGetCallerInfo2S.get_caller_info_c2bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call module level function
-        update_stack(exp_stack=exp_stack, line_num=10605, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10736, add=0)
         func_get_caller_info_3(exp_stack=exp_stack, capsys=capsys)
 
         # call method
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=10610, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10741, add=1)
         cls_get_caller_info3.get_caller_info_m3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call static method
-        update_stack(exp_stack=exp_stack, line_num=10615, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10746, add=1)
         cls_get_caller_info3.get_caller_info_s3(exp_stack=exp_stack,
                                                 capsys=capsys)
 
         # call class method
-        update_stack(exp_stack=exp_stack, line_num=10620, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10751, add=1)
         ClassGetCallerInfo3.get_caller_info_c3(exp_stack=exp_stack,
                                                capsys=capsys)
 
         # call overloaded base class method
-        update_stack(exp_stack=exp_stack, line_num=10625, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10756, add=1)
         cls_get_caller_info3.get_caller_info_m3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class static method
-        update_stack(exp_stack=exp_stack, line_num=10630, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10761, add=1)
         cls_get_caller_info3.get_caller_info_s3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call overloaded base class class method
-        update_stack(exp_stack=exp_stack, line_num=10635, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10766, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bo(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call subclass method
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=10641, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10772, add=1)
         cls_get_caller_info3s.get_caller_info_m3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass static method
-        update_stack(exp_stack=exp_stack, line_num=10646, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10777, add=1)
         cls_get_caller_info3s.get_caller_info_s3s(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call subclass class method
-        update_stack(exp_stack=exp_stack, line_num=10651, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10782, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3s(exp_stack=exp_stack,
                                                  capsys=capsys)
 
         # call overloaded subclass method
-        update_stack(exp_stack=exp_stack, line_num=10656, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10787, add=1)
         cls_get_caller_info3s.get_caller_info_m3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass static method
-        update_stack(exp_stack=exp_stack, line_num=10661, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10792, add=1)
         cls_get_caller_info3s.get_caller_info_s3bo(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call overloaded subclass class method
-        update_stack(exp_stack=exp_stack, line_num=10666, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10797, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bo(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base method from subclass method
-        update_stack(exp_stack=exp_stack, line_num=10671, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10802, add=1)
         cls_get_caller_info3s.get_caller_info_m3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base static method from subclass static method
-        update_stack(exp_stack=exp_stack, line_num=10676, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10807, add=1)
         cls_get_caller_info3s.get_caller_info_s3sb(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class method from subclass class method
-        update_stack(exp_stack=exp_stack, line_num=10681, add=1)
+        update_stack(exp_stack=exp_stack, line_num=10812, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3sb(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
 
 ########################################################################
@@ -10709,31 +10840,31 @@
         """
         self.var1 += 1
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3',
                                      func_name='get_caller_info_m3',
                                      line_num=8911)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=10720, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10851, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=10727, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10858, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=10734, add=0)
+            update_stack(exp_stack=exp_stack, line_num=10865, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -10760,31 +10891,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3',
                                      func_name='get_caller_info_s3',
                                      line_num=8961)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=10771, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10902, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=10778, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10909, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=10785, add=0)
+            update_stack(exp_stack=exp_stack, line_num=10916, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -10811,31 +10942,31 @@
             capsys: Pytest fixture that captures output
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3',
                                      func_name='get_caller_info_c3',
                                      line_num=9011)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=10822, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10953, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=10829, add=0)
+        update_stack(exp_stack=exp_stack, line_num=10960, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=10836, add=0)
+            update_stack(exp_stack=exp_stack, line_num=10967, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -10862,31 +10993,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3',
                                      func_name='get_caller_info_m3bo',
                                      line_num=9061)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=10873, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11004, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=10880, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11011, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=10887, add=0)
+            update_stack(exp_stack=exp_stack, line_num=11018, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -10913,31 +11044,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3',
                                      func_name='get_caller_info_s3bo',
                                      line_num=9111)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=10924, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11055, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=10931, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11062, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=10938, add=0)
+            update_stack(exp_stack=exp_stack, line_num=11069, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -10965,31 +11096,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3',
                                      func_name='get_caller_info_c3bo',
                                      line_num=9162)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=10976, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11107, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=10983, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11114, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=10990, add=0)
+            update_stack(exp_stack=exp_stack, line_num=11121, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -11017,31 +11148,31 @@
         """
         self.var1 += 1
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3',
                                      func_name='get_caller_info_m3bt',
                                      line_num=9213)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=11028, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11159, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=11035, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11166, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=11042, add=0)
+            update_stack(exp_stack=exp_stack, line_num=11173, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -11068,31 +11199,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3',
                                      func_name='get_caller_info_s3bt',
                                      line_num=9263)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=11079, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11210, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=11086, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11217, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=11093, add=0)
+            update_stack(exp_stack=exp_stack, line_num=11224, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -11120,31 +11251,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3',
                                      func_name='get_caller_info_c3bt',
                                      line_num=9314)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=11131, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11262, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=11138, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11269, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=11145, add=0)
+            update_stack(exp_stack=exp_stack, line_num=11276, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -11183,31 +11314,31 @@
         """
         self.var1 += 1
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3S',
                                      func_name='get_caller_info_m3s',
                                      line_num=9376)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=11194, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11325, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=11201, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11332, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=11208, add=0)
+            update_stack(exp_stack=exp_stack, line_num=11339, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -11234,31 +11365,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3S',
                                      func_name='get_caller_info_s3s',
                                      line_num=9426)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=11245, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11376, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=11252, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11383, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=11259, add=0)
+            update_stack(exp_stack=exp_stack, line_num=11390, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -11286,31 +11417,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3S',
                                      func_name='get_caller_info_c3s',
                                      line_num=9477)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=11297, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11428, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=11304, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11435, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=11311, add=0)
+            update_stack(exp_stack=exp_stack, line_num=11442, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -11337,31 +11468,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3S',
                                      func_name='get_caller_info_m3bo',
                                      line_num=9527)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=11348, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11479, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=11355, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11486, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=11362, add=0)
+            update_stack(exp_stack=exp_stack, line_num=11493, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -11388,31 +11519,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3S',
                                      func_name='get_caller_info_s3bo',
                                      line_num=9577)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=11399, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11530, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=11406, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11537, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=11413, add=0)
+            update_stack(exp_stack=exp_stack, line_num=11544, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -11440,31 +11571,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3S',
                                      func_name='get_caller_info_c3bo',
                                      line_num=9628)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=11451, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11582, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=11458, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11589, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=11465, add=0)
+            update_stack(exp_stack=exp_stack, line_num=11596, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -11491,31 +11622,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3S',
                                      func_name='get_caller_info_m3sb',
                                      line_num=9678)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=11502, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11633, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=11509, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11640, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=11516, add=0)
+            update_stack(exp_stack=exp_stack, line_num=11647, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -11523,44 +11654,44 @@
             verify_diag_msg(exp_stack=exp_stack,
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call base class normal method target
-        update_stack(exp_stack=exp_stack, line_num=11531, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11662, add=0)
         self.get_caller_info_m3bt(exp_stack=exp_stack, capsys=capsys)
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=11534, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11665, add=1)
         cls_get_caller_info3.get_caller_info_m3bt(exp_stack=exp_stack,
                                                   capsys=capsys)
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=11538, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11669, add=1)
         cls_get_caller_info3s.get_caller_info_m3bt(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class static method target
-        update_stack(exp_stack=exp_stack, line_num=11543, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11674, add=0)
         self.get_caller_info_s3bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=11545, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11676, add=0)
         super().get_caller_info_s3bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=11547, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11678, add=1)
         ClassGetCallerInfo3.get_caller_info_s3bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=11550, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11681, add=1)
         ClassGetCallerInfo3S.get_caller_info_s3bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base class class method target
-        update_stack(exp_stack=exp_stack, line_num=11555, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11686, add=0)
         super().get_caller_info_c3bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=11557, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11688, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=11560, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11691, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 3S Method 8
@@ -11576,31 +11707,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3S',
                                      func_name='get_caller_info_s3sb',
                                      line_num=9762)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=11587, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11718, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=11594, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11725, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=11601, add=0)
+            update_stack(exp_stack=exp_stack, line_num=11732, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -11609,35 +11740,35 @@
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call base class normal method target
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=11617, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11748, add=1)
         cls_get_caller_info3.get_caller_info_m3bt(exp_stack=exp_stack,
                                                   capsys=capsys)
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=11621, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11752, add=1)
         cls_get_caller_info3s.get_caller_info_m3bt(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class static method target
-        update_stack(exp_stack=exp_stack, line_num=11626, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11757, add=1)
         ClassGetCallerInfo3.get_caller_info_s3bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=11629, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11760, add=1)
         ClassGetCallerInfo3S.get_caller_info_s3bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base class class method target
-        update_stack(exp_stack=exp_stack, line_num=11634, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11765, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=11637, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11768, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
     ####################################################################
     # Class 3S Method 9
@@ -11654,31 +11785,31 @@
 
         """
         exp_caller_info = CallerInfo(mod_name='test_diag_msg.py',
                                      cls_name='ClassGetCallerInfo3S',
                                      func_name='get_caller_info_c3sb',
                                      line_num=9839)
         exp_stack.append(exp_caller_info)
-        update_stack(exp_stack=exp_stack, line_num=11665, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11796, add=0)
         for i, expected_caller_info in enumerate(list(reversed(exp_stack))):
             try:
                 frame = _getframe(i)
                 caller_info = get_caller_info(frame)
             finally:
                 del frame
             assert caller_info == expected_caller_info
 
         # test call sequence
-        update_stack(exp_stack=exp_stack, line_num=11672, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11803, add=0)
         call_seq = get_formatted_call_sequence(depth=len(exp_stack))
 
         assert call_seq == get_exp_seq(exp_stack=exp_stack)
 
         if capsys:  # if capsys, test diag_msg
-            update_stack(exp_stack=exp_stack, line_num=11679, add=0)
+            update_stack(exp_stack=exp_stack, line_num=11810, add=0)
             before_time = datetime.now()
             diag_msg('message 1', 1, depth=len(exp_stack))
             after_time = datetime.now()
 
             diag_msg_args = TestDiagMsg.get_diag_msg_args(
                 depth_arg=len(exp_stack),
                 msg_arg=['message 1', 1])
@@ -11687,77 +11818,77 @@
                             before_time=before_time,
                             after_time=after_time,
                             capsys=capsys,
                             diag_msg_args=diag_msg_args)
 
         # call base class normal method target
         cls_get_caller_info3 = ClassGetCallerInfo3()
-        update_stack(exp_stack=exp_stack, line_num=11695, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11826, add=1)
         cls_get_caller_info3.get_caller_info_m3bt(exp_stack=exp_stack,
                                                   capsys=capsys)
         cls_get_caller_info3s = ClassGetCallerInfo3S()
-        update_stack(exp_stack=exp_stack, line_num=11699, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11830, add=1)
         cls_get_caller_info3s.get_caller_info_m3bt(exp_stack=exp_stack,
                                                    capsys=capsys)
 
         # call base class static method target
-        update_stack(exp_stack=exp_stack, line_num=11704, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11835, add=1)
         cls.get_caller_info_s3bt(exp_stack=exp_stack,
                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=11707, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11838, add=0)
         super().get_caller_info_s3bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=11709, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11840, add=1)
         ClassGetCallerInfo3.get_caller_info_s3bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=11712, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11843, add=1)
         ClassGetCallerInfo3S.get_caller_info_s3bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         # call base class class method target
-        update_stack(exp_stack=exp_stack, line_num=11717, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11848, add=0)
         cls.get_caller_info_c3bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=11719, add=0)
+        update_stack(exp_stack=exp_stack, line_num=11850, add=0)
         super().get_caller_info_c3bt(exp_stack=exp_stack, capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=11721, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11852, add=1)
         ClassGetCallerInfo3.get_caller_info_c3bt(exp_stack=exp_stack,
                                                  capsys=capsys)
-        update_stack(exp_stack=exp_stack, line_num=11724, add=1)
+        update_stack(exp_stack=exp_stack, line_num=11855, add=1)
         ClassGetCallerInfo3S.get_caller_info_c3bt(exp_stack=exp_stack,
                                                   capsys=capsys)
 
         exp_stack.pop()
 
 
 ########################################################################
-# following tests needs to be at module level (i.e., script form)
+# following tests need to be at module level (i.e., script form)
 ########################################################################
 
 ########################################################################
 # test get_caller_info from module (script) level
 ########################################################################
 exp_stack0: Deque[CallerInfo] = deque()
 exp_caller_info0 = CallerInfo(mod_name='test_diag_msg.py',
                               cls_name='',
                               func_name='',
                               line_num=9921)
 
 exp_stack0.append(exp_caller_info0)
-update_stack(exp_stack=exp_stack0, line_num=11748, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11879, add=0)
 for i0, expected_caller_info0 in enumerate(list(reversed(exp_stack0))):
     try:
         frame0 = _getframe(i0)
         caller_info0 = get_caller_info(frame0)
     finally:
         del frame0
     assert caller_info0 == expected_caller_info0
 
 ########################################################################
 # test get_formatted_call_sequence from module (script) level
 ########################################################################
-update_stack(exp_stack=exp_stack0, line_num=11757, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11888, add=0)
 call_seq0 = get_formatted_call_sequence(depth=1)
 
 assert call_seq0 == get_exp_seq(exp_stack=exp_stack0)
 
 ########################################################################
 # test diag_msg from module (script) level
 # note that this is just a smoke test and is only visually verified
@@ -11766,71 +11897,71 @@
 diag_msg('hello')
 diag_msg(depth=2)
 diag_msg('hello2', depth=3)
 diag_msg(depth=4, end='\n\n')
 diag_msg('hello3', depth=5, end='\n\n')
 
 # call module level function
-update_stack(exp_stack=exp_stack0, line_num=11774, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11905, add=0)
 func_get_caller_info_1(exp_stack=exp_stack0, capsys=None)
 
 # call method
 cls_get_caller_info01 = ClassGetCallerInfo1()
-update_stack(exp_stack=exp_stack0, line_num=11779, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11910, add=0)
 cls_get_caller_info01.get_caller_info_m1(exp_stack=exp_stack0, capsys=None)
 
 # call static method
-update_stack(exp_stack=exp_stack0, line_num=11783, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11914, add=0)
 cls_get_caller_info01.get_caller_info_s1(exp_stack=exp_stack0, capsys=None)
 
 # call class method
-update_stack(exp_stack=exp_stack0, line_num=11787, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11918, add=0)
 ClassGetCallerInfo1.get_caller_info_c1(exp_stack=exp_stack0, capsys=None)
 
 # call overloaded base class method
-update_stack(exp_stack=exp_stack0, line_num=11791, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11922, add=0)
 cls_get_caller_info01.get_caller_info_m1bo(exp_stack=exp_stack0, capsys=None)
 
 # call overloaded base class static method
-update_stack(exp_stack=exp_stack0, line_num=11795, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11926, add=0)
 cls_get_caller_info01.get_caller_info_s1bo(exp_stack=exp_stack0, capsys=None)
 
 # call overloaded base class class method
-update_stack(exp_stack=exp_stack0, line_num=11799, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11930, add=0)
 ClassGetCallerInfo1.get_caller_info_c1bo(exp_stack=exp_stack0, capsys=None)
 
 # call subclass method
 cls_get_caller_info01S = ClassGetCallerInfo1S()
-update_stack(exp_stack=exp_stack0, line_num=11804, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11935, add=0)
 cls_get_caller_info01S.get_caller_info_m1s(exp_stack=exp_stack0, capsys=None)
 
 # call subclass static method
-update_stack(exp_stack=exp_stack0, line_num=11808, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11939, add=0)
 cls_get_caller_info01S.get_caller_info_s1s(exp_stack=exp_stack0, capsys=None)
 
 # call subclass class method
-update_stack(exp_stack=exp_stack0, line_num=11812, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11943, add=0)
 ClassGetCallerInfo1S.get_caller_info_c1s(exp_stack=exp_stack0, capsys=None)
 
 # call overloaded subclass method
-update_stack(exp_stack=exp_stack0, line_num=11816, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11947, add=0)
 cls_get_caller_info01S.get_caller_info_m1bo(exp_stack=exp_stack0, capsys=None)
 
 # call overloaded subclass static method
-update_stack(exp_stack=exp_stack0, line_num=11820, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11951, add=0)
 cls_get_caller_info01S.get_caller_info_s1bo(exp_stack=exp_stack0, capsys=None)
 
 # call overloaded subclass class method
-update_stack(exp_stack=exp_stack0, line_num=11824, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11955, add=0)
 ClassGetCallerInfo1S.get_caller_info_c1bo(exp_stack=exp_stack0, capsys=None)
 
 # call base method from subclass method
-update_stack(exp_stack=exp_stack0, line_num=11828, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11959, add=0)
 cls_get_caller_info01S.get_caller_info_m1sb(exp_stack=exp_stack0, capsys=None)
 
 # call base static method from subclass static method
-update_stack(exp_stack=exp_stack0, line_num=11832, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11963, add=0)
 cls_get_caller_info01S.get_caller_info_s1sb(exp_stack=exp_stack0, capsys=None)
 
 # call base class method from subclass class method
-update_stack(exp_stack=exp_stack0, line_num=11836, add=0)
+update_stack(exp_stack=exp_stack0, line_num=11967, add=0)
 ClassGetCallerInfo1S.get_caller_info_c1sb(exp_stack=exp_stack0, capsys=None)
```

### Comparing `scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_file_catalog.py` & `scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_file_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                     'file2': Path('/run/media/file2.csv'),
                     'file3': Path('/run/media/file3.csv'),
                     'file4': Path('/run/media/file4.csv'),
                     'file5': Path('/run/media/file5.csv')}
                    ]
 
 
-@pytest.fixture(params=file_specs_list)  # type: ignore
+@pytest.fixture(params=file_specs_list)
 def file_specs(request: Any) -> Dict[str, Path]:
     """Pytest fixture for different file_specs args.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
```

### Comparing `scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_flower_box.py` & `scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_flower_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from scottbrian_utils.flower_box import print_flower_box_msg \
     as print_flower_box_msg
 
 file_num_list = [0, 1, 2, 3]
 
 
-@pytest.fixture(params=file_num_list)  # type: ignore
+@pytest.fixture(params=file_num_list)
 def file_num(request: Any) -> int:
     """Using different file arg.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -172,15 +172,15 @@
                   '*************************\n'
                   '* AB                    *\n'
                   '*  CDEF HIJ             *\n'
                   '* One long line to test *\n'
                   '*************************\n'
                   )]
 
-    @pytest.mark.parametrize('msg_list, expected_result',  # type: ignore
+    @pytest.mark.parametrize('msg_list, expected_result',
                              case_list)
     def test_flower_box(self, capsys: Any, msg_list: List[str],
                         expected_result: str,
                         file_num: int) -> None:
         """test_flower_box method.
 
         Args:
```

### Comparing `scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_log_verifier.py` & `scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_log_verifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 ########################################################################
 # log_enabled_arg
 ########################################################################
 log_enabled_arg_list = [True, False]
 
 
-@pytest.fixture(params=log_enabled_arg_list)  # type: ignore
+@pytest.fixture(params=log_enabled_arg_list)
 def log_enabled_arg(request: Any) -> bool:
     """Using enabled and disabled logging.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -61,15 +61,15 @@
 
 ########################################################################
 # simple_str_arg
 ########################################################################
 simple_str_arg_list = ['a', 'ab', 'a1', 'xyz123']
 
 
-@pytest.fixture(params=simple_str_arg_list)  # type: ignore
+@pytest.fixture(params=simple_str_arg_list)
 def simple_str_arg(request: Any) -> str:
     """Using different string messages.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -80,80 +80,80 @@
 
 ########################################################################
 # number of log messages arg fixtures
 ########################################################################
 num_msgs_arg_list = [0, 1, 2, 3]
 
 
-@pytest.fixture(params=num_msgs_arg_list)  # type: ignore
+@pytest.fixture(params=num_msgs_arg_list)
 def num_exp_msgs1(request: Any) -> int:
     """Using different number of messages.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
         The params values are returned one at a time
     """
     return cast(int, request.param)
 
 
-@pytest.fixture(params=num_msgs_arg_list)  # type: ignore
+@pytest.fixture(params=num_msgs_arg_list)
 def num_exp_msgs2(request: Any) -> int:
     """Using different number of messages.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
         The params values are returned one at a time
     """
     return cast(int, request.param)
 
 
-@pytest.fixture(params=num_msgs_arg_list)  # type: ignore
+@pytest.fixture(params=num_msgs_arg_list)
 def num_exp_msgs3(request: Any) -> int:
     """Using different number of messages.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
         The params values are returned one at a time
     """
     return cast(int, request.param)
 
 
-@pytest.fixture(params=num_msgs_arg_list)  # type: ignore
+@pytest.fixture(params=num_msgs_arg_list)
 def num_act_msgs1(request: Any) -> int:
     """Using different number of messages.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
         The params values are returned one at a time
     """
     return cast(int, request.param)
 
 
-@pytest.fixture(params=num_msgs_arg_list)  # type: ignore
+@pytest.fixture(params=num_msgs_arg_list)
 def num_act_msgs2(request: Any) -> int:
     """Using different number of messages.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
         The params values are returned one at a time
     """
     return cast(int, request.param)
 
 
-@pytest.fixture(params=num_msgs_arg_list)  # type: ignore
+@pytest.fixture(params=num_msgs_arg_list)
 def num_act_msgs3(request: Any) -> int:
     """Using different number of messages.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -169,15 +169,15 @@
     """Test examples of LogVer."""
 
     ####################################################################
     # test_log_verifier_example1
     ####################################################################
     def test_log_verifier_example1(self,
                                    capsys: pytest.CaptureFixture[str],
-                                   caplog: pytest.CaptureFixture[str]
+                                   caplog: pytest.LogCaptureFixture
                                    ) -> None:
         """Test log_verifier example1.
 
         Args:
             capsys: pytest fixture to capture print output
             caplog: pytest fixture to capture log output
 
@@ -222,15 +222,15 @@
         assert captured == expected_result
 
     ####################################################################
     # test_log_verifier_example2
     ####################################################################
     def test_log_verifier_example2(self,
                                    capsys: pytest.CaptureFixture[str],
-                                   caplog: pytest.CaptureFixture[str]
+                                   caplog: pytest.LogCaptureFixture
                                    ) -> None:
         """Test log_verifier example2.
 
         Args:
             capsys: pytest fixture to capture print output
             caplog: pytest fixture to capture log output
 
@@ -279,15 +279,15 @@
         assert captured == expected_result
 
     ####################################################################
     # test_log_verifier_example3
     ####################################################################
     def test_log_verifier_example3(self,
                                    capsys: pytest.CaptureFixture[str],
-                                   caplog: pytest.CaptureFixture[str]
+                                   caplog: pytest.LogCaptureFixture
                                    ) -> None:
         """Test log_verifier example3.
 
         Args:
             capsys: pytest fixture to capture print output
             caplog: pytest fixture to capture log output
 
@@ -336,15 +336,15 @@
         assert captured == expected_result
 
     ####################################################################
     # test_log_verifier_example4
     ####################################################################
     def test_log_verifier_example4(self,
                                    capsys: pytest.CaptureFixture[str],
-                                   caplog: pytest.CaptureFixture[str]
+                                   caplog: pytest.LogCaptureFixture
                                    ) -> None:
         """Test log_verifier example4.
 
         Args:
             capsys: pytest fixture to capture print output
             caplog: pytest fixture to capture log output
 
@@ -397,15 +397,15 @@
         assert captured == expected_result
 
     ####################################################################
     # test_log_verifier_example5
     ####################################################################
     def test_log_verifier_example5(self,
                                    capsys: pytest.CaptureFixture[str],
-                                   caplog: pytest.CaptureFixture[str]
+                                   caplog: pytest.LogCaptureFixture
                                    ) -> None:
         """Test log_verifier example5 for add_msg.
 
         Args:
             capsys: pytest fixture to capture print output
             caplog: pytest fixture to capture log output
 
@@ -457,15 +457,15 @@
 ########################################################################
 # TestLogVerBasic class
 ########################################################################
 class TestLogVerBasic:
     """Test basic functions of LogVer."""
 
     ####################################################################
-    # test_log_verifier_time_match
+    # test_log_verifier_repr
     ####################################################################
     def test_log_verifier_repr(self,
                                capsys: pytest.CaptureFixture[str]
                                ) -> None:
         """Test log_verifier repr function.
 
         Args:
@@ -484,20 +484,21 @@
         print(log_ver2)  # test of __repr__
         captured = capsys.readouterr().out
 
         expected = "LogVer(log_name='simple_repr2_log_name')\n"
         assert captured == expected
 
     ####################################################################
-    # test_log_verifier_time_match
+    # test_log_verifier_simple_match
     ####################################################################
+    @pytest.mark.parametrize("simple_str_arg", simple_str_arg_list)
     def test_log_verifier_simple_match(self,
                                        simple_str_arg: str,
                                        capsys: pytest.CaptureFixture[str],
-                                       caplog: pytest.CaptureFixture[str]
+                                       caplog: pytest.LogCaptureFixture
                                        ) -> None:
         """Test log_verifier time match.
 
         Args:
             simple_str_arg: string to use in the message
             capsys: pytest fixture to capture print output
             caplog: pytest fixture to capture log output
@@ -537,19 +538,313 @@
         expected_result += f"('simple_match', 10, '{simple_str_arg}')\n"
 
         captured = capsys.readouterr().out
 
         assert captured == expected_result
 
     ####################################################################
+    # test_log_verifier_print_matched
+    ####################################################################
+    @pytest.mark.parametrize("print_matched_arg", (None, True, False))
+    @pytest.mark.parametrize("num_msgs_arg", (1, 2, 3))
+    def test_log_verifier_print_matched(
+            self,
+            print_matched_arg: Union[bool, None],
+            num_msgs_arg: int,
+            capsys: pytest.CaptureFixture[str],
+            caplog: pytest.LogCaptureFixture
+            ) -> None:
+        """Test log_verifier with print_matched args.
+
+        Args:
+            print_matched_arg: specifies whether to print the matched
+                records
+            num_msgs_arg: number of log messages
+            capsys: pytest fixture to capture print output
+            caplog: pytest fixture to capture log output
+        """
+        log_name = 'print_matched'
+        t_logger = logging.getLogger(log_name)
+        log_ver = LogVer(log_name=log_name)
+
+        log_msgs: list[str] = []
+        for idx in range(num_msgs_arg):
+            log_msgs.append(f'log_msg_{idx}')
+            log_ver.add_msg(log_msg=log_msgs[idx])
+            t_logger.debug(log_msgs[idx])
+
+        log_results = log_ver.get_match_results(caplog)
+        if print_matched_arg is None:
+            log_ver.print_match_results(log_results)
+        else:
+            log_ver.print_match_results(log_results,
+                                        print_matched=print_matched_arg)
+        log_ver.verify_log_results(log_results)
+
+        expected_result = '\n'
+        expected_result += '**********************************\n'
+        expected_result += f'* number expected log records: {num_msgs_arg} *\n'
+        expected_result += '* number expected unmatched  : 0 *\n'
+        expected_result += f'* number actual log records  : {num_msgs_arg} *\n'
+        expected_result += '* number actual unmatched    : 0 *\n'
+        expected_result += f'* number matched records     : {num_msgs_arg} *\n'
+        expected_result += '**********************************\n'
+        expected_result += '\n'
+        expected_result += '*********************************\n'
+        expected_result += '* unmatched expected records    *\n'
+        expected_result += '* (logger name, level, message) *\n'
+        expected_result += '*********************************\n'
+        expected_result += '\n'
+        expected_result += '*********************************\n'
+        expected_result += '* unmatched actual records      *\n'
+        expected_result += '* (logger name, level, message) *\n'
+        expected_result += '*********************************\n'
+
+        if print_matched_arg is None or print_matched_arg is True:
+            expected_result += '\n'
+            expected_result += '*********************************\n'
+            expected_result += '* matched records               *\n'
+            expected_result += '* (logger name, level, message) *\n'
+            expected_result += '*********************************\n'
+
+            for log_msg in log_msgs:
+                expected_result += f"('{log_name}', 10, '{log_msg}')\n"
+
+        captured = capsys.readouterr().out
+
+        assert captured == expected_result
+
+    ####################################################################
+    # test_log_verifier_simple_fullmatch
+    ####################################################################
+    double_str_arg_list = [('a1', 'a12'),
+                           ('b_2', 'b_23'),
+                           ('xyz_567', 'xyz_5678')]
+
+    @pytest.mark.parametrize("double_str_arg", double_str_arg_list)
+    def test_log_verifier_simple_fullmatch(self,
+                                           double_str_arg: str,
+                                           capsys: pytest.CaptureFixture[str],
+                                           caplog: pytest.LogCaptureFixture
+                                           ) -> None:
+        """Test log_verifier time match.
+
+        Args:
+            double_str_arg: string to use in the message
+            capsys: pytest fixture to capture print output
+            caplog: pytest fixture to capture log output
+        """
+        ################################################################
+        # step 0: use non-fullmatch in controlled way to cause success
+        ################################################################
+        log_name = 'fullmatch_0'
+        t_logger = logging.getLogger(log_name)
+        log_ver = LogVer(log_name=log_name)
+
+        log_ver.add_msg(log_msg=double_str_arg[0])
+        log_ver.add_msg(log_msg=double_str_arg[1])
+
+        t_logger.debug(double_str_arg[0])
+        t_logger.debug(double_str_arg[1])
+
+        log_ver.print_match_results(
+            log_results := log_ver.get_match_results(caplog))
+        log_ver.verify_log_results(log_results)
+
+        expected_result = '\n'
+        expected_result += '**********************************\n'
+        expected_result += '* number expected log records: 2 *\n'
+        expected_result += '* number expected unmatched  : 0 *\n'
+        expected_result += '* number actual log records  : 2 *\n'
+        expected_result += '* number actual unmatched    : 0 *\n'
+        expected_result += '* number matched records     : 2 *\n'
+        expected_result += '**********************************\n'
+        expected_result += '\n'
+        expected_result += '*********************************\n'
+        expected_result += '* unmatched expected records    *\n'
+        expected_result += '* (logger name, level, message) *\n'
+        expected_result += '*********************************\n'
+        expected_result += '\n'
+        expected_result += '*********************************\n'
+        expected_result += '* unmatched actual records      *\n'
+        expected_result += '* (logger name, level, message) *\n'
+        expected_result += '*********************************\n'
+        expected_result += '\n'
+        expected_result += '*********************************\n'
+        expected_result += '* matched records               *\n'
+        expected_result += '* (logger name, level, message) *\n'
+        expected_result += '*********************************\n'
+        expected_result += f"('fullmatch_0', 10, '{double_str_arg[0]}')\n"
+        expected_result += f"('fullmatch_0', 10, '{double_str_arg[1]}')\n"
+
+        captured = capsys.readouterr().out
+
+        assert captured == expected_result
+
+        ################################################################
+        # step 1: use non-fullmatch in controlled way to cause error
+        ################################################################
+        caplog.clear()
+
+        log_name = 'fullmatch_1'
+        t_logger = logging.getLogger(log_name)
+        log_ver = LogVer(log_name=log_name)
+
+        log_ver.add_msg(log_msg=double_str_arg[0])
+        log_ver.add_msg(log_msg=double_str_arg[1])
+
+        t_logger.debug(double_str_arg[1])
+        t_logger.debug(double_str_arg[0])
+
+        log_ver.print_match_results(
+            log_results := log_ver.get_match_results(caplog))
+
+        with pytest.raises(UnmatchedExpectedMessages):
+            log_ver.verify_log_results(log_results)
+
+        expected_result = '\n'
+        expected_result += '**********************************\n'
+        expected_result += '* number expected log records: 2 *\n'
+        expected_result += '* number expected unmatched  : 1 *\n'
+        expected_result += '* number actual log records  : 2 *\n'
+        expected_result += '* number actual unmatched    : 1 *\n'
+        expected_result += '* number matched records     : 1 *\n'
+        expected_result += '**********************************\n'
+        expected_result += '\n'
+        expected_result += '*********************************\n'
+        expected_result += '* unmatched expected records    *\n'
+        expected_result += '* (logger name, level, message) *\n'
+        expected_result += '*********************************\n'
+        expected_result += f"('fullmatch_1', 10, '{double_str_arg[1]}')\n"
+        expected_result += '\n'
+        expected_result += '*********************************\n'
+        expected_result += '* unmatched actual records      *\n'
+        expected_result += '* (logger name, level, message) *\n'
+        expected_result += '*********************************\n'
+        expected_result += f"('fullmatch_1', 10, '{double_str_arg[0]}')\n"
+        expected_result += '\n'
+        expected_result += '*********************************\n'
+        expected_result += '* matched records               *\n'
+        expected_result += '* (logger name, level, message) *\n'
+        expected_result += '*********************************\n'
+        expected_result += f"('fullmatch_1', 10, '{double_str_arg[1]}')\n"
+
+        captured = capsys.readouterr().out
+
+        assert captured == expected_result
+
+        ################################################################
+        # step 2: use fullmatch in controlled way - should succeed
+        ################################################################
+        caplog.clear()
+
+        log_name = 'fullmatch_2'
+        t_logger = logging.getLogger(log_name)
+        log_ver = LogVer(log_name=log_name)
+
+        log_ver.add_msg(log_msg=double_str_arg[0],
+                        fullmatch=True)
+        log_ver.add_msg(log_msg=double_str_arg[1],
+                        fullmatch=True)
+
+        t_logger.debug(double_str_arg[0])
+        t_logger.debug(double_str_arg[1])
+
+        log_ver.print_match_results(
+            log_results := log_ver.get_match_results(caplog))
+        log_ver.verify_log_results(log_results)
+
+        expected_result = '\n'
+        expected_result += '**********************************\n'
+        expected_result += '* number expected log records: 2 *\n'
+        expected_result += '* number expected unmatched  : 0 *\n'
+        expected_result += '* number actual log records  : 2 *\n'
+        expected_result += '* number actual unmatched    : 0 *\n'
+        expected_result += '* number matched records     : 2 *\n'
+        expected_result += '**********************************\n'
+        expected_result += '\n'
+        expected_result += '*********************************\n'
+        expected_result += '* unmatched expected records    *\n'
+        expected_result += '* (logger name, level, message) *\n'
+        expected_result += '*********************************\n'
+        expected_result += '\n'
+        expected_result += '*********************************\n'
+        expected_result += '* unmatched actual records      *\n'
+        expected_result += '* (logger name, level, message) *\n'
+        expected_result += '*********************************\n'
+        expected_result += '\n'
+        expected_result += '*********************************\n'
+        expected_result += '* matched records               *\n'
+        expected_result += '* (logger name, level, message) *\n'
+        expected_result += '*********************************\n'
+        expected_result += f"('fullmatch_2', 10, '{double_str_arg[0]}')\n"
+        expected_result += f"('fullmatch_2', 10, '{double_str_arg[1]}')\n"
+
+        captured = capsys.readouterr().out
+
+        assert captured == expected_result
+
+        ################################################################
+        # step 3: use fullmatch in error case and expect success
+        ################################################################
+        caplog.clear()
+
+        log_name = 'fullmatch_3'
+        t_logger = logging.getLogger(log_name)
+        log_ver = LogVer(log_name=log_name)
+
+        log_ver.add_msg(log_msg=double_str_arg[0],
+                        fullmatch=True)
+        log_ver.add_msg(log_msg=double_str_arg[1],
+                        fullmatch=True)
+
+        t_logger.debug(double_str_arg[1])
+        t_logger.debug(double_str_arg[0])
+
+        log_ver.print_match_results(
+            log_results := log_ver.get_match_results(caplog))
+
+        log_ver.verify_log_results(log_results)
+
+        expected_result = '\n'
+        expected_result += '**********************************\n'
+        expected_result += '* number expected log records: 2 *\n'
+        expected_result += '* number expected unmatched  : 0 *\n'
+        expected_result += '* number actual log records  : 2 *\n'
+        expected_result += '* number actual unmatched    : 0 *\n'
+        expected_result += '* number matched records     : 2 *\n'
+        expected_result += '**********************************\n'
+        expected_result += '\n'
+        expected_result += '*********************************\n'
+        expected_result += '* unmatched expected records    *\n'
+        expected_result += '* (logger name, level, message) *\n'
+        expected_result += '*********************************\n'
+        expected_result += '\n'
+        expected_result += '*********************************\n'
+        expected_result += '* unmatched actual records      *\n'
+        expected_result += '* (logger name, level, message) *\n'
+        expected_result += '*********************************\n'
+        expected_result += '\n'
+        expected_result += '*********************************\n'
+        expected_result += '* matched records               *\n'
+        expected_result += '* (logger name, level, message) *\n'
+        expected_result += '*********************************\n'
+        expected_result += f"('fullmatch_3', 10, '{double_str_arg[1]}')\n"
+        expected_result += f"('fullmatch_3', 10, '{double_str_arg[0]}')\n"
+
+        captured = capsys.readouterr().out
+
+        assert captured == expected_result
+
+    ####################################################################
     # test_log_verifier_time_match
     ####################################################################
     def test_log_verifier_time_match(self,
                                      capsys: pytest.CaptureFixture[str],
-                                     caplog: pytest.CaptureFixture[str]
+                                     caplog: pytest.LogCaptureFixture
                                      ) -> None:
         """Test log_verifier time match.
 
         Args:
             capsys: pytest fixture to capture print output
             caplog: pytest fixture to capture log output
         """
@@ -600,15 +895,15 @@
 
     ####################################################################
     # test_log_verifier_add_call_seq
     ####################################################################
     def test_log_verifier_add_call_seq(self,
                                        simple_str_arg: str,
                                        capsys: pytest.CaptureFixture[str],
-                                       caplog: pytest.CaptureFixture[str]
+                                       caplog: pytest.LogCaptureFixture
                                        ) -> None:
         """Test log_verifier add_call_seq method.
 
         Args:
             simple_str_arg: string to use in the message
             capsys: pytest fixture to capture print output
             caplog: pytest fixture to capture log output
@@ -655,15 +950,15 @@
 
     ####################################################################
     # test_log_verifier_add_call_seq2
     ####################################################################
     def test_log_verifier_add_call_seq2(self,
                                         simple_str_arg: str,
                                         capsys: pytest.CaptureFixture[str],
-                                        caplog: pytest.CaptureFixture[str]
+                                        caplog: pytest.LogCaptureFixture
                                         ) -> None:
         """Test log_verifier add_call_seq method.
 
         Args:
             simple_str_arg: string to use in the message
             capsys: pytest fixture to capture print output
             caplog: pytest fixture to capture log output
@@ -714,15 +1009,15 @@
 
     ####################################################################
     # test_log_verifier_add_call_seq3
     ####################################################################
     def test_log_verifier_add_call_seq3(self,
                                         simple_str_arg: str,
                                         capsys: pytest.CaptureFixture[str],
-                                        caplog: pytest.CaptureFixture[str]
+                                        caplog: pytest.LogCaptureFixture
                                         ) -> None:
         """Test log_verifier add_call_seq method.
 
         Args:
             simple_str_arg: string to use in the message
             capsys: pytest fixture to capture print output
             caplog: pytest fixture to capture log output
@@ -781,15 +1076,15 @@
 
     ####################################################################
     # test_log_verifier_no_log
     ####################################################################
     def test_log_verifier_no_log(self,
                                  log_enabled_arg: bool,
                                  capsys: pytest.CaptureFixture[str],
-                                 caplog: pytest.CaptureFixture[str]
+                                 caplog: pytest.LogCaptureFixture
                                  ) -> None:
         """Test log_verifier with logging disabled and enabled.
 
         Args:
             log_enabled_arg: fixture to indicate whether log is enabled
             capsys: pytest fixture to capture print output
             caplog: pytest fixture to capture log output
@@ -873,15 +1168,15 @@
                                  num_exp_msgs1: int,
                                  num_exp_msgs2: int,
                                  num_exp_msgs3: int,
                                  num_act_msgs1: int,
                                  num_act_msgs2: int,
                                  num_act_msgs3: int,
                                  capsys: pytest.CaptureFixture[str],
-                                 caplog: pytest.CaptureFixture[str]
+                                 caplog: pytest.LogCaptureFixture
                                  ) -> None:
         """Test log_verifier combos.
 
         Args:
             num_exp_msgs1: number of expected messages for msg1
             num_exp_msgs2: number of expected messages for msg2
             num_exp_msgs3: number of expected messages for msg3
```

### Comparing `scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_msgs.py` & `scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_msgs.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 ########################################################################
 # timeout_arg fixture
 ########################################################################
 timeout_arg_list = [0.0, 0.3, 0.5, 1, 2, 4]
 
 
-@pytest.fixture(params=timeout_arg_list)  # type: ignore
+@pytest.fixture(params=timeout_arg_list)
 def timeout_arg(request: Any) -> float:
     """Using different seconds for timeout.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -62,15 +62,15 @@
 
 ########################################################################
 # who_arg fixture
 ########################################################################
 who_arg_list = ['beta', 'charlie', 'both']
 
 
-@pytest.fixture(params=who_arg_list)  # type: ignore
+@pytest.fixture(params=who_arg_list)
 def who_arg(request: Any) -> str:
     """Using different msg targets.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -81,15 +81,15 @@
 
 #######################################################################
 # msg_arg fixture
 ########################################################################
 msg_arg_list = [0, '0', 0.0, 'hello', 1, [1, 2, 3], ('a', 'b', 'c')]
 
 
-@pytest.fixture(params=msg_arg_list)  # type: ignore
+@pytest.fixture(params=msg_arg_list)
 def msg_arg(request: Any) -> Any:
     """Using different msgs.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -100,15 +100,15 @@
 
 #######################################################################
 # start_arg fixture
 ########################################################################
 start_arg_list = ['before', 'mid1', 'mid2', 'after']
 
 
-@pytest.fixture(params=start_arg_list)  # type: ignore
+@pytest.fixture(params=start_arg_list)
 def start_arg(request: Any) -> str:
     """Using different remote thread start points.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -120,15 +120,15 @@
 ########################################################################
 # TestMsgsErrors class
 ########################################################################
 class TestMsgsErrors:
     """TestMsgsErrors class."""
     def test_msgs_timeout(self,
                           timeout_arg: float,
-                          caplog: pytest.CaptureFixture[str]) -> None:
+                          caplog: pytest.LogCaptureFixture) -> None:
         """test_msgs_timeout.
 
         Args:
             timeout_arg: number of seconds to use for timeout value
                            on get_msg request
             caplog: pytest fixture to capture log output
```

### Comparing `scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_pauser.py` & `scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_pauser.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 ########################################################################
 # interval_arg fixture
 ########################################################################
 interval_arg_list = [0.0, 0.001, 0.010, 0.100, 0.500, 0.900, 1, 2, 5]
 
 
-@pytest.fixture(params=interval_arg_list)  # type: ignore
+@pytest.fixture(params=interval_arg_list)
 def interval_arg(request: Any) -> IntFloat:
     """Using different seconds for interval.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -68,15 +68,15 @@
 min_max_interval_msecs_arg_list = [(1, 1),
                                    (1, 2),
                                    (1, 3),
                                    (1, 100),
                                    (101, 200)]
 
 
-@pytest.fixture(params=min_max_interval_msecs_arg_list)  # type: ignore
+@pytest.fixture(params=min_max_interval_msecs_arg_list)
 def min_max_interval_msecs_arg(request: Any) -> tuple[int, int]:
     """Using different interval ranges.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -87,15 +87,15 @@
 
 #######################################################################
 # increment_arg
 ########################################################################
 increment_arg_list = [1, 2, 3, 5]
 
 
-@pytest.fixture(params=increment_arg_list)  # type: ignore
+@pytest.fixture(params=increment_arg_list)
 def increment_arg(request: Any) -> int:
     """Using different increments.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -106,15 +106,15 @@
 
 #######################################################################
 # part_time_factor_arg
 ########################################################################
 part_time_factor_arg_list = [0.3, 0.4, 0.5]
 
 
-@pytest.fixture(params=part_time_factor_arg_list)  # type: ignore
+@pytest.fixture(params=part_time_factor_arg_list)
 def part_time_factor_arg(request: Any) -> float:
     """Using different part time ratios.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -125,15 +125,15 @@
 
 #######################################################################
 # sleep_late_ratio_arg
 ########################################################################
 sleep_late_ratio_arg_list = [0.90, 1.0]
 
 
-@pytest.fixture(params=sleep_late_ratio_arg_list)  # type: ignore
+@pytest.fixture(params=sleep_late_ratio_arg_list)
 def sleep_late_ratio_arg(request: Any) -> float:
     """Using different sleep ratios.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -144,15 +144,15 @@
 
 #######################################################################
 # iterations_arg
 ########################################################################
 iterations_arg_list = [1, 2, 3]
 
 
-@pytest.fixture(params=iterations_arg_list)  # type: ignore
+@pytest.fixture(params=iterations_arg_list)
 def iterations_arg(request: Any) -> int:
     """Using different calibration iterations.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
```

### Comparing `scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_stop_watch.py` & `scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_stop_watch.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 ########################################################################
 # timeout_arg fixture
 ########################################################################
 timeout_arg_list = [0.0, 0.3, 0.5, 1, 2, 4]
 
 
-@pytest.fixture(params=timeout_arg_list)  # type: ignore
+@pytest.fixture(params=timeout_arg_list)
 def timeout_arg(request: Any) -> float:
     """Using different seconds for timeout.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -65,15 +65,15 @@
 
 #######################################################################
 # sleep_arg fixture
 ########################################################################
 sleep_arg_list = [0.3, 1.0, 2, 2.5]
 
 
-@pytest.fixture(params=sleep_arg_list)  # type: ignore
+@pytest.fixture(params=sleep_arg_list)
 def sleep_arg(request: Any) -> float:
     """Using different remote thread start points.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
```

### Comparing `scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_time_hdr.py` & `scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_time_hdr.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                       '%a %b %d %Y %H:%M:%S',
                       '%a %b %d %H:%M:%S.%f',
                       '%A %b %d %H:%M:%S.%f',
                       '%A %B %d %H:%M:%S.%f'
                       ]
 
 
-@pytest.fixture(params=dt_format_arg_list)  # type: ignore
+@pytest.fixture(params=dt_format_arg_list)
 def dt_format_arg(request: Any) -> str:
     """Using different time formats.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -91,15 +91,15 @@
                            '%X',
                            '%%',
                            '%G',
                            '%u',
                            '%V']
 
 
-@pytest.fixture(params=dt_format_char_arg_list)  # type: ignore
+@pytest.fixture(params=dt_format_char_arg_list)
 def dt_format_char_arg(request: Any) -> str:
     """Using different time formats.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -142,15 +142,15 @@
                                  ),
                         datetime(2022, 12, 31, 23, 59, 59, 999999,
                                  tzinfo=timezone(timedelta(hours=23,
                                                            minutes=59)),
                                  )]
 
 
-@pytest.fixture(params=dt_datetime_arg_list)  # type: ignore
+@pytest.fixture(params=dt_datetime_arg_list)
 def dt_datetime_arg(request: Any) -> datetime:
     """Using different time formats.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -158,15 +158,15 @@
     """
     return cast(datetime, request.param)
 
 
 dt_datetime_month_arg_list = [1, 5, 9, 10, 11, 12]
 
 
-@pytest.fixture(params=dt_datetime_month_arg_list)  # type: ignore
+@pytest.fixture(params=dt_datetime_month_arg_list)
 def dt_datetime_month_arg(request: Any) -> int:
     """Using different time formats.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -174,15 +174,15 @@
     """
     return cast(int, request.param)
 
 
 dt_datetime_day_arg_list = [1, 2, 9, 10, 11, 19, 20, 21, 29, 30, 31]
 
 
-@pytest.fixture(params=dt_datetime_day_arg_list)  # type: ignore
+@pytest.fixture(params=dt_datetime_day_arg_list)
 def dt_datetime_day_arg(request: Any) -> int:
     """Using different time formats.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -212,28 +212,28 @@
                            '%I:%M:%S %p',
                            '%H:%M:%S.%f',
                            '%H:%M:%S.%f%z',
                            '%H:%M:%S.%f %Z'
                            ]
 
 
-@pytest.fixture(params=dt_format_date_arg_list)  # type: ignore
+@pytest.fixture(params=dt_format_date_arg_list)
 def dt_format_date_arg(request: Any) -> str:
     """Using different time formats.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
         The params values are returned one at a time
     """
     return cast(str, request.param)
 
 
-@pytest.fixture(params=dt_format_time_arg_list)  # type: ignore
+@pytest.fixture(params=dt_format_time_arg_list)
 def dt_format_time_arg(request: Any) -> str:
     """Using different time formats.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -241,15 +241,15 @@
     """
     return cast(str, request.param)
 
 
 style_num_list = [1, 2, 3]
 
 
-@pytest.fixture(params=style_num_list)  # type: ignore
+@pytest.fixture(params=style_num_list)
 def style_num(request: Any) -> int:
     """Using different time_box styles.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -257,15 +257,15 @@
     """
     return cast(int, request.param)
 
 
 end_arg_list = ['0', '\n', '\n\n']
 
 
-@pytest.fixture(params=end_arg_list)  # type: ignore
+@pytest.fixture(params=end_arg_list)
 def end_arg(request: Any) -> str:
     """Choose single or double space.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -273,15 +273,15 @@
     """
     return cast(str, request.param)
 
 
 file_arg_list = ['0', 'None', 'sys.stdout', 'sys.stderr']
 
 
-@pytest.fixture(params=file_arg_list)  # type: ignore
+@pytest.fixture(params=file_arg_list)
 def file_arg(request: Any) -> str:
     """Using different file arg.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -289,15 +289,15 @@
     """
     return cast(str, request.param)
 
 
 flush_arg_list = ['0', 'True', 'False']
 
 
-@pytest.fixture(params=flush_arg_list)  # type: ignore
+@pytest.fixture(params=flush_arg_list)
 def flush_arg(request: Any) -> str:
     """False: do not flush print stream, True: flush print stream.
 
      Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -310,15 +310,15 @@
                     'static_true',
                     'static_false',
                     'dynamic_true',
                     'dynamic_false'
                     ]
 
 
-@pytest.fixture(params=enabled_arg_list)  # type: ignore
+@pytest.fixture(params=enabled_arg_list)
 def enabled_arg(request: Any) -> str:
     """Determines how to specify time_box_enabled.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -495,15 +495,15 @@
 
         assert formatted_new_dt == adjusted_old_dt
 
 
 class TestStartStopHeader:
     """TestStartStopHeader class."""
 
-    @pytest.fixture(scope='class')  # type: ignore
+    @pytest.fixture(scope='class')
     def hdr(self) -> "StartStopHeader":
         """Method hdr.
 
         Returns:
             StartStopHeader instance
         """
         return StartStopHeader('TestName')
```

### Comparing `scottbrian_utils-2.3.0/tests/test_scottbrian_utils/test_timer.py` & `scottbrian_utils-2.4.0/tests/test_scottbrian_utils/test_timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 zero_or_less_timeout_arg_list = [-1.1, -1, 0, 0.0]
 greater_than_zero_timeout_arg_list = [0.3, 0.5, 1, 1.5, 2, 4]
 
 
 ########################################################################
 # timeout_arg fixture
 ########################################################################
-@pytest.fixture(params=greater_than_zero_timeout_arg_list)  # type: ignore
+@pytest.fixture(params=greater_than_zero_timeout_arg_list)
 def timeout_arg(request: Any) -> IntFloat:
     """Using different seconds for timeout.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -61,15 +61,15 @@
     """
     return cast(IntFloat, request.param)
 
 
 ########################################################################
 # zero_or_less_timeout_arg fixture
 ########################################################################
-@pytest.fixture(params=zero_or_less_timeout_arg_list)  # type: ignore
+@pytest.fixture(params=zero_or_less_timeout_arg_list)
 def zero_or_less_timeout_arg(request: Any) -> IntFloat:
     """Using different seconds for timeout.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -77,15 +77,15 @@
     """
     return cast(IntFloat, request.param)
 
 
 ########################################################################
 # greater_than_zero_timeout_arg fixture
 ########################################################################
-@pytest.fixture(params=greater_than_zero_timeout_arg_list)  # type: ignore
+@pytest.fixture(params=greater_than_zero_timeout_arg_list)
 def greater_than_zero_timeout_arg(request: Any) -> IntFloat:
     """Using different seconds for timeout.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -93,15 +93,15 @@
     """
     return cast(IntFloat, request.param)
 
 
 ########################################################################
 # zero_or_less_default_timeout_arg fixture
 ########################################################################
-@pytest.fixture(params=zero_or_less_timeout_arg_list)  # type: ignore
+@pytest.fixture(params=zero_or_less_timeout_arg_list)
 def zero_or_less_default_timeout_arg(request: Any) -> IntFloat:
     """Using different seconds for timeout_default.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
@@ -109,15 +109,15 @@
     """
     return cast(IntFloat, request.param)
 
 
 ########################################################################
 # greater_than_zero_default_timeout_arg fixture
 ########################################################################
-@pytest.fixture(params=greater_than_zero_timeout_arg_list)  # type: ignore
+@pytest.fixture(params=greater_than_zero_timeout_arg_list)
 def greater_than_zero_default_timeout_arg(request: Any) -> IntFloat:
     """Using different seconds for timeout_default.
 
     Args:
         request: special fixture that returns the fixture params
 
     Returns:
```

### Comparing `scottbrian_utils-2.3.0/tox.ini` & `scottbrian_utils-2.4.0/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -65,16 +65,19 @@
     # darglint -v 2 tests/test_scottbrian_utils/
 
 [testenv:mypy]
 description = invoke mypy to check types
 
 deps =
     mypy
+    pytest
 
 commands =
+    python -m pip show mypy
+    python -m pip show pytest
     mypy src/scottbrian_utils/
     mypy tests/test_scottbrian_utils/ --cache-dir=/dev/null --show-absolute-path
 ;    mypy src/scottbrian_utils/diag_msg.py
 ;    mypy src/scottbrian_utils/file_catalog.py
 ;    mypy src/scottbrian_utils/flower_box.py
 ;    mypy src/scottbrian_utils/log_verifier.py
 ;    mypy src/scottbrian_utils/msgs.py
@@ -91,14 +94,15 @@
 ;    mypy tests/test_scottbrian_utils/test_timer.py --cache-dir=/dev/null
 
 [testenv:py{39, 310, 311}-mypywrapt]
 description = invoke mypy to check types with wrapt stubs
 
 deps =
     mypy
+    pytest
     type_stubs/mypywrapt
 
 commands =
     mypy src/scottbrian_utils/diag_msg.py
     mypy src/scottbrian_utils/file_catalog.py
     mypy src/scottbrian_utils/flower_box.py
     adjust_src --pre src/scottbrian_utils/time_hdr.py type_stubs/mypywrapt/time_hdr.py
@@ -149,18 +153,18 @@
 
 commands =
     pytest --cov=scottbrian_utils --cov-report=term --cov-report=html -p no:threadexception {posargs}
 
 
 [testenv:docs]
 description = invoke sphinx-build to build the HTML docs
-basepython = 
+basepython =
     python3.9
-deps = 
-    sphinx
+deps =
+    sphinx==6.2.1  # can't use later version - 7.0.1 produces error: UndefinedError("'style' is undefined")
     sphinx-autodoc-typehints
     sphinx_rtd_theme
     pytest
 
 commands =
     sphinx-build -b html docs/source docs/build -W -a -E
     python -c 'import pathlib; print("documentation available under file://\{0\}".format(pathlib.Path(r"docs") / "build" / "index.html"))'
```

### Comparing `scottbrian_utils-2.3.0/type_stubs/mypywrapt/adjust_src/adjust_src.py` & `scottbrian_utils-2.4.0/type_stubs/mypywrapt/adjust_src/adjust_src.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-2.3.0/type_stubs/mypywrapt/build/lib/adjust_src/adjust_src.py` & `scottbrian_utils-2.4.0/type_stubs/mypywrapt/build/lib/adjust_src/adjust_src.py`

 * *Files identical despite different names*

