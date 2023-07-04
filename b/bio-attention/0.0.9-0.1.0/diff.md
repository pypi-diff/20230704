# Comparing `tmp/bio-attention-0.0.9.tar.gz` & `tmp/bio-attention-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio-attention-0.0.9.tar", last modified: Fri Jun 30 08:37:26 2023, max compression
+gzip compressed data, was "bio-attention-0.1.0.tar", last modified: Tue Jul  4 09:12:16 2023, max compression
```

## Comparing `bio-attention-0.0.9.tar` & `bio-attention-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:37:26.067799 bio-attention-0.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:37:26.063799 bio-attention-0.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:37:26.063799 bio-attention-0.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-30 08:37:18.000000 bio-attention-0.0.9/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-30 08:37:18.000000 bio-attention-0.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 08:37:18.000000 bio-attention-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-30 08:37:26.067799 bio-attention-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-30 08:37:18.000000 bio-attention-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:37:26.063799 bio-attention-0.0.9/bio_attention/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 08:37:18.000000 bio-attention-0.0.9/bio_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17847 2023-06-30 08:37:18.000000 bio-attention-0.0.9/bio_attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-06-30 08:37:18.000000 bio-attention-0.0.9/bio_attention/embed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:37:26.067799 bio-attention-0.0.9/bio_attention/img/
--rw-r--r--   0 runner    (1001) docker     (123)  2372654 2023-06-30 08:37:18.000000 bio-attention-0.0.9/bio_attention/img/2Dslidingwindow-attention.png
--rw-r--r--   0 runner    (1001) docker     (123)   118589 2023-06-30 08:37:18.000000 bio-attention-0.0.9/bio_attention/img/windowed_implementation.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23235 2023-06-30 08:37:18.000000 bio-attention-0.0.9/bio_attention/positional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:37:26.063799 bio-attention-0.0.9/bio_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-30 08:37:26.000000 bio-attention-0.0.9/bio_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-30 08:37:26.000000 bio-attention-0.0.9/bio_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 08:37:26.000000 bio-attention-0.0.9/bio_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 08:37:26.000000 bio-attention-0.0.9/bio_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 08:37:26.000000 bio-attention-0.0.9/bio_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 08:37:18.000000 bio-attention-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-30 08:37:26.067799 bio-attention-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:12:16.878276 bio-attention-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:12:16.862276 bio-attention-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:12:16.870276 bio-attention-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-04 09:12:06.000000 bio-attention-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-04 09:12:06.000000 bio-attention-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-04 09:12:06.000000 bio-attention-0.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-04 09:12:06.000000 bio-attention-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-04 09:12:16.878276 bio-attention-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-04 09:12:06.000000 bio-attention-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:12:16.870276 bio-attention-0.1.0/bio_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-04 09:12:06.000000 bio-attention-0.1.0/bio_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31836 2023-07-04 09:12:06.000000 bio-attention-0.1.0/bio_attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-07-04 09:12:06.000000 bio-attention-0.1.0/bio_attention/embed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:12:16.874276 bio-attention-0.1.0/bio_attention/img/
+-rw-r--r--   0 runner    (1001) docker     (123)  2372654 2023-07-04 09:12:06.000000 bio-attention-0.1.0/bio_attention/img/2Dslidingwindow-attention.png
+-rw-r--r--   0 runner    (1001) docker     (123)   118589 2023-07-04 09:12:06.000000 bio-attention-0.1.0/bio_attention/img/windowed_implementation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    27683 2023-07-04 09:12:06.000000 bio-attention-0.1.0/bio_attention/positional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:12:16.874276 bio-attention-0.1.0/bio_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-04 09:12:16.000000 bio-attention-0.1.0/bio_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-04 09:12:16.000000 bio-attention-0.1.0/bio_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 09:12:16.000000 bio-attention-0.1.0/bio_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 09:12:16.000000 bio-attention-0.1.0/bio_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-04 09:12:16.000000 bio-attention-0.1.0/bio_attention.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:12:16.878276 bio-attention-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-04 09:12:06.000000 bio-attention-0.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-04 09:12:06.000000 bio-attention-0.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-04 09:12:06.000000 bio-attention-0.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:12:16.878276 bio-attention-0.1.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-04 09:12:06.000000 bio-attention-0.1.0/docs/source/bio-attention.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-04 09:12:06.000000 bio-attention-0.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-04 09:12:06.000000 bio-attention-0.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 09:12:06.000000 bio-attention-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-04 09:12:16.878276 bio-attention-0.1.0/setup.cfg
```

### Comparing `bio-attention-0.0.9/.github/workflows/publish.yml` & `bio-attention-0.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.9/.gitignore` & `bio-attention-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.9/LICENSE` & `bio-attention-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.9/PKG-INFO` & `bio-attention-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: bio-attention
-Version: 0.0.9
+Version: 0.1.0
 Summary: Simple implementations of attention modules adapted for the biological data domain
 Home-page: https://github.com/gdewael/bio-attention
 Author: Gaetan De Waele
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 <h1>bio-attention</h1>
 
 Simple implementations of attention modules adapted for the biological data domain.
 
 [![PyPi Version](https://img.shields.io/pypi/v/bio-attention.svg)](https://pypi.python.org/pypi/bio-attention/)
 [![GitHub license](https://img.shields.io/github/license/gdewael/bio-attention)](https://github.com/gdewael/bio-attention/blob/main/LICENSE)
+[![Documentation](https://readthedocs.org/projects/bio-attention/badge/?version=latest&style=flat-default)](https://bio-attention.readthedocs.io/en/latest/index.html)
 
 </div>
 
 # :construction: THIS CODE IS BEING ACTIVELY DEVELOPED :construction:
 
 Don't look for stability here (yet).
 
@@ -65,9 +66,9 @@
   - [x] Encoder
   - [x] Decoder
   - [ ] Cross
   - [x] Support for multi-dim inputs
 - [ ] Add a warning if non-increasing positional indices are used with a decoder attention
 - [ ] Add docs clarifying that clf tokens are automatically accounted for if no pos is provided for them
 - [ ] Tests
-- [ ] Typing
+- [x] Typing
 - [ ] Docs
```

### Comparing `bio-attention-0.0.9/README.md` & `bio-attention-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 <div align="center">
 <h1>bio-attention</h1>
 
 Simple implementations of attention modules adapted for the biological data domain.
 
 [![PyPi Version](https://img.shields.io/pypi/v/bio-attention.svg)](https://pypi.python.org/pypi/bio-attention/)
 [![GitHub license](https://img.shields.io/github/license/gdewael/bio-attention)](https://github.com/gdewael/bio-attention/blob/main/LICENSE)
+[![Documentation](https://readthedocs.org/projects/bio-attention/badge/?version=latest&style=flat-default)](https://bio-attention.readthedocs.io/en/latest/index.html)
 
 </div>
 
 # :construction: THIS CODE IS BEING ACTIVELY DEVELOPED :construction:
 
 Don't look for stability here (yet).
 
@@ -55,9 +56,9 @@
   - [x] Encoder
   - [x] Decoder
   - [ ] Cross
   - [x] Support for multi-dim inputs
 - [ ] Add a warning if non-increasing positional indices are used with a decoder attention
 - [ ] Add docs clarifying that clf tokens are automatically accounted for if no pos is provided for them
 - [ ] Tests
-- [ ] Typing
+- [x] Typing
 - [ ] Docs
```

### Comparing `bio-attention-0.0.9/bio_attention/img/2Dslidingwindow-attention.png` & `bio-attention-0.1.0/bio_attention/img/2Dslidingwindow-attention.png`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.9/bio_attention/img/windowed_implementation.svg` & `bio-attention-0.1.0/bio_attention/img/windowed_implementation.svg`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.9/bio_attention.egg-info/PKG-INFO` & `bio-attention-0.1.0/bio_attention.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: bio-attention
-Version: 0.0.9
+Version: 0.1.0
 Summary: Simple implementations of attention modules adapted for the biological data domain
 Home-page: https://github.com/gdewael/bio-attention
 Author: Gaetan De Waele
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 <h1>bio-attention</h1>
 
 Simple implementations of attention modules adapted for the biological data domain.
 
 [![PyPi Version](https://img.shields.io/pypi/v/bio-attention.svg)](https://pypi.python.org/pypi/bio-attention/)
 [![GitHub license](https://img.shields.io/github/license/gdewael/bio-attention)](https://github.com/gdewael/bio-attention/blob/main/LICENSE)
+[![Documentation](https://readthedocs.org/projects/bio-attention/badge/?version=latest&style=flat-default)](https://bio-attention.readthedocs.io/en/latest/index.html)
 
 </div>
 
 # :construction: THIS CODE IS BEING ACTIVELY DEVELOPED :construction:
 
 Don't look for stability here (yet).
 
@@ -65,9 +66,9 @@
   - [x] Encoder
   - [x] Decoder
   - [ ] Cross
   - [x] Support for multi-dim inputs
 - [ ] Add a warning if non-increasing positional indices are used with a decoder attention
 - [ ] Add docs clarifying that clf tokens are automatically accounted for if no pos is provided for them
 - [ ] Tests
-- [ ] Typing
+- [x] Typing
 - [ ] Docs
```

