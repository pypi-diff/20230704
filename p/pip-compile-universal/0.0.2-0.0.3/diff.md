# Comparing `tmp/pip_compile_universal-0.0.2.tar.gz` & `tmp/pip_compile_universal-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_compile_universal-0.0.2.tar", last modified: Tue Feb  7 05:30:08 2023, max compression
+gzip compressed data, was "pip_compile_universal-0.0.3.tar", last modified: Tue Jul  4 04:07:28 2023, max compression
```

## Comparing `pip_compile_universal-0.0.2.tar` & `pip_compile_universal-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-02-07 05:30:08.592918 pip_compile_universal-0.0.2/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      101 2023-02-05 17:29:27.000000 pip_compile_universal-0.0.2/.cz.toml
--rw-r--r--   0 mirec     (1000) mirec     (1000)      129 2023-02-05 17:18:58.000000 pip_compile_universal-0.0.2/.editorconfig
--rw-r--r--   0 mirec     (1000) mirec     (1000)       69 2023-02-05 15:44:34.000000 pip_compile_universal-0.0.2/.gitignore
--rw-r--r--   0 mirec     (1000) mirec     (1000)      822 2023-02-07 05:29:52.000000 pip_compile_universal-0.0.2/CHANGELOG.md
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2317 2023-02-07 05:30:08.592918 pip_compile_universal-0.0.2/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1640 2023-02-05 17:24:51.000000 pip_compile_universal-0.0.2/README.rst
--rwxr-xr-x   0 mirec     (1000) mirec     (1000)     8089 2023-02-06 15:49:42.000000 pip_compile_universal-0.0.2/pip_compile_universal
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-02-07 05:30:08.592918 pip_compile_universal-0.0.2/pip_compile_universal.egg-info/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2317 2023-02-07 05:30:08.000000 pip_compile_universal-0.0.2/pip_compile_universal.egg-info/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)      327 2023-02-07 05:30:08.000000 pip_compile_universal-0.0.2/pip_compile_universal.egg-info/SOURCES.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-02-07 05:30:08.000000 pip_compile_universal-0.0.2/pip_compile_universal.egg-info/dependency_links.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)       59 2023-02-07 05:30:08.000000 pip_compile_universal-0.0.2/pip_compile_universal.egg-info/requires.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-02-07 05:30:08.000000 pip_compile_universal-0.0.2/pip_compile_universal.egg-info/top_level.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1049 2023-02-07 05:29:52.000000 pip_compile_universal-0.0.2/pyproject.toml
--rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-02-07 05:30:08.592918 pip_compile_universal-0.0.2/setup.cfg
--rw-r--r--   0 mirec     (1000) mirec     (1000)       95 2023-02-05 15:42:57.000000 pip_compile_universal-0.0.2/setup.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-07-04 04:07:28.719385 pip_compile_universal-0.0.3/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      101 2023-02-05 17:29:27.000000 pip_compile_universal-0.0.3/.cz.toml
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      129 2023-02-05 17:18:58.000000 pip_compile_universal-0.0.3/.editorconfig
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       69 2023-02-05 15:44:34.000000 pip_compile_universal-0.0.3/.gitignore
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      912 2023-07-04 04:06:51.000000 pip_compile_universal-0.0.3/CHANGELOG.md
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2317 2023-07-04 04:07:28.719385 pip_compile_universal-0.0.3/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1640 2023-02-05 17:24:51.000000 pip_compile_universal-0.0.3/README.rst
+-rwxr-xr-x   0 mirec     (1000) mirec     (1000)    20451 2023-06-16 04:00:24.000000 pip_compile_universal-0.0.3/pip_compile_universal
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-07-04 04:07:28.719385 pip_compile_universal-0.0.3/pip_compile_universal.egg-info/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2317 2023-07-04 04:07:28.000000 pip_compile_universal-0.0.3/pip_compile_universal.egg-info/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      327 2023-07-04 04:07:28.000000 pip_compile_universal-0.0.3/pip_compile_universal.egg-info/SOURCES.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-07-04 04:07:28.000000 pip_compile_universal-0.0.3/pip_compile_universal.egg-info/dependency_links.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       59 2023-07-04 04:07:28.000000 pip_compile_universal-0.0.3/pip_compile_universal.egg-info/requires.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-07-04 04:07:28.000000 pip_compile_universal-0.0.3/pip_compile_universal.egg-info/top_level.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1049 2023-07-04 04:06:51.000000 pip_compile_universal-0.0.3/pyproject.toml
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-07-04 04:07:28.719385 pip_compile_universal-0.0.3/setup.cfg
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       95 2023-02-05 15:42:57.000000 pip_compile_universal-0.0.3/setup.py
```

### Comparing `pip_compile_universal-0.0.2/CHANGELOG.md` & `pip_compile_universal-0.0.3/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.0.3 (2023-07-04)
+
+### Feat
+
+- Interpret markers inside temporary requirements files
+
 ## 0.0.2 (2023-02-07)
 
 ### Fix
 
 - Fixed split regex
 
 ## 0.0.1 (2023-02-05)
```

### Comparing `pip_compile_universal-0.0.2/PKG-INFO` & `pip_compile_universal-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip_compile_universal
-Version: 0.0.2
+Version: 0.0.3
 Summary: Compile requirements.in using pip-tools for multiple python versions
 Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/mireq/pip-compile-universal
 Project-URL: documentation, https://github.com/mireq/pip-compile-universal
 Project-URL: repository, https://github.com/mireq/pip-compile-universal
 Project-URL: changelog, https://github.com/mireq/pip-compile-universal/blob/master/CHANGELOG.md
```

### Comparing `pip_compile_universal-0.0.2/README.rst` & `pip_compile_universal-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pip_compile_universal-0.0.2/pip_compile_universal.egg-info/PKG-INFO` & `pip_compile_universal-0.0.3/pip_compile_universal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-compile-universal
-Version: 0.0.2
+Version: 0.0.3
 Summary: Compile requirements.in using pip-tools for multiple python versions
 Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/mireq/pip-compile-universal
 Project-URL: documentation, https://github.com/mireq/pip-compile-universal
 Project-URL: repository, https://github.com/mireq/pip-compile-universal
 Project-URL: changelog, https://github.com/mireq/pip-compile-universal/blob/master/CHANGELOG.md
```

### Comparing `pip_compile_universal-0.0.2/pyproject.toml` & `pip_compile_universal-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,9 +34,9 @@
 
 [tool.setuptools]
 
 [tool.setuptools_scm]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.0.2"
+version = "0.0.3"
 tag_format = "$version"
```

