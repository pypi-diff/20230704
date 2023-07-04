# Comparing `tmp/luucy_python-0.1.0.tar.gz` & `tmp/luucy_python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luucy_python-0.1.0.tar", last modified: Mon Jul  3 19:40:11 2023, max compression
+gzip compressed data, was "luucy_python-0.2.0.tar", last modified: Tue Jul  4 14:32:47 2023, max compression
```

## Comparing `luucy_python-0.1.0.tar` & `luucy_python-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6181 2023-07-03 15:38:04.555956 luucy_python-0.1.0/README.md
--rw-r--r--   0        0        0     1270 2023-07-03 19:40:11.292427 luucy_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      251 2023-07-03 18:52:11.126113 luucy_python-0.1.0/src/luucy/__init__.py
--rw-r--r--   0        0        0       22 2023-07-03 19:25:42.817887 luucy_python-0.1.0/src/luucy/__version__.py
--rw-r--r--   0        0        0      453 2023-07-03 18:48:57.747657 luucy_python-0.1.0/tests/features/login/init.feature
--rw-r--r--   0        0        0      628 2023-07-03 18:49:13.760880 luucy_python-0.1.0/tests/test_init_with_username_and_password.py
--rw-r--r--   0        0        0      582 2023-07-03 18:51:32.452394 luucy_python-0.1.0/tests/test_init_without_username_and_password copy.py
--rw-r--r--   0        0        0     6404 1970-01-01 00:00:00.000000 luucy_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      182 2023-07-04 14:32:20.588575 luucy_python-0.2.0/README.md
+-rw-r--r--   0        0        0     1390 2023-07-04 14:32:47.379634 luucy_python-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      538 2023-07-04 14:32:20.589575 luucy_python-0.2.0/src/luucy/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-04 14:32:20.589575 luucy_python-0.2.0/src/luucy/__version__.py
+-rw-r--r--   0        0        0      453 2023-07-04 14:32:20.590575 luucy_python-0.2.0/tests/features/login/init.feature
+-rw-r--r--   0        0        0      628 2023-07-04 14:32:20.590575 luucy_python-0.2.0/tests/test_init_with_username_and_password.py
+-rw-r--r--   0        0        0      582 2023-07-04 14:32:20.590575 luucy_python-0.2.0/tests/test_init_without_username_and_password copy.py
+-rw-r--r--   0        0        0      405 1970-01-01 00:00:00.000000 luucy_python-0.2.0/PKG-INFO
```

### Comparing `luucy_python-0.1.0/pyproject.toml` & `luucy_python-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "luucy-python"
-version = "0.1.0"
+version = "0.2.0"
 description = "LUUCY Python APIs"
 authors = [
     { name = "Thorben Westerhuys", email = "thorben.westerhuys@luucy.ch" },
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "README.md"
@@ -28,14 +28,18 @@
     "black>=23.3.0",
     "pre-commit>=3.3.3",
     "pytest>=7.4.0",
     "pytest-watch>=4.2.0",
     "pytest-cov>=4.1.0",
     "pytest-bdd>=6.1.1",
     "commitizen>=3.5.2",
+    "mkdocs-material>=9.1.18",
+    "mkdocstrings[python]>=0.22.0",
+    "mkdocstrings-python>=1.1.2",
+    "mike>=1.1.2",
 ]
 
 [tool.pylint]
 max-line-length = 88
 disable = [
     "W0613",
     "C0114",
```

### Comparing `luucy_python-0.1.0/tests/test_init_with_username_and_password.py` & `luucy_python-0.2.0/tests/test_init_with_username_and_password.py`

 * *Files identical despite different names*

### Comparing `luucy_python-0.1.0/tests/test_init_without_username_and_password copy.py` & `luucy_python-0.2.0/tests/test_init_without_username_and_password copy.py`

 * *Files identical despite different names*

