# Comparing `tmp/xilinx-language-server-0.0.1.tar.gz` & `tmp/xilinx-language-server-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xilinx-language-server-0.0.1.tar", last modified: Tue Jul  4 13:55:37 2023, max compression
+gzip compressed data, was "xilinx-language-server-0.0.2.tar", last modified: Tue Jul  4 14:11:00 2023, max compression
```

## Comparing `xilinx-language-server-0.0.1.tar` & `xilinx-language-server-0.0.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:55:37.552282 xilinx-language-server-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:55:37.544282 xilinx-language-server-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:55:37.544282 xilinx-language-server-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-07-04 13:55:37.552282 xilinx-language-server-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:55:37.544282 xilinx-language-server-0.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:55:37.544282 xilinx-language-server-0.0.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/docs/api/xilinx-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:55:37.548282 xilinx-language-server-0.0.1/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/docs/resources/requirements.md
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:55:37.548282 xilinx-language-server-0.0.1/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:55:37.548282 xilinx-language-server-0.0.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/scripts/generate-api.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/scripts/generate-requirements.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/scripts/vivado.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/scripts/xilinx.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/scripts/xsct.tcl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 13:55:37.552282 xilinx-language-server-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:55:37.544282 xilinx-language-server-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:55:37.548282 xilinx-language-server-0.0.1/src/xilinx_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/src/xilinx_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/src/xilinx_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-04 13:55:37.000000 xilinx-language-server-0.0.1/src/xilinx_language_server/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:55:37.544282 xilinx-language-server-0.0.1/src/xilinx_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:55:37.552282 xilinx-language-server-0.0.1/src/xilinx_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (123)  2991295 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/src/xilinx_language_server/assets/json/vivado.json
--rw-r--r--   0 runner    (1001) docker     (123)   111383 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/src/xilinx_language_server/assets/json/xsct.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/src/xilinx_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/src/xilinx_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:55:37.548282 xilinx-language-server-0.0.1/src/xilinx_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-07-04 13:55:37.000000 xilinx-language-server-0.0.1/src/xilinx_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-04 13:55:37.000000 xilinx-language-server-0.0.1/src/xilinx_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:55:37.000000 xilinx-language-server-0.0.1/src/xilinx_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-04 13:55:37.000000 xilinx-language-server-0.0.1/src/xilinx_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-04 13:55:37.000000 xilinx-language-server-0.0.1/src/xilinx_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 13:55:37.000000 xilinx-language-server-0.0.1/src/xilinx_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:55:37.552282 xilinx-language-server-0.0.1/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:55:37.552282 xilinx-language-server-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-04 13:55:27.000000 xilinx-language-server-0.0.1/tests/server_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:11:00.495085 xilinx-language-server-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:11:00.483085 xilinx-language-server-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:11:00.483085 xilinx-language-server-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-07-04 14:11:00.495085 xilinx-language-server-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:11:00.483085 xilinx-language-server-0.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:11:00.483085 xilinx-language-server-0.0.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/docs/api/xilinx-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:11:00.483085 xilinx-language-server-0.0.2/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:11:00.483085 xilinx-language-server-0.0.2/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:11:00.487085 xilinx-language-server-0.0.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/scripts/generate-api.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/scripts/generate-requirements.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/scripts/vivado.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/scripts/xilinx.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/scripts/xsct.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 14:11:00.495085 xilinx-language-server-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:11:00.479085 xilinx-language-server-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:11:00.487085 xilinx-language-server-0.0.2/src/xilinx_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/src/xilinx_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/src/xilinx_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-04 14:11:00.000000 xilinx-language-server-0.0.2/src/xilinx_language_server/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:11:00.479085 xilinx-language-server-0.0.2/src/xilinx_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:11:00.491085 xilinx-language-server-0.0.2/src/xilinx_language_server/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)  2991295 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/src/xilinx_language_server/assets/json/vivado.json
+-rw-r--r--   0 runner    (1001) docker     (123)   111383 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/src/xilinx_language_server/assets/json/xsct.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/src/xilinx_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/src/xilinx_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:11:00.487085 xilinx-language-server-0.0.2/src/xilinx_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-07-04 14:11:00.000000 xilinx-language-server-0.0.2/src/xilinx_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-04 14:11:00.000000 xilinx-language-server-0.0.2/src/xilinx_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:11:00.000000 xilinx-language-server-0.0.2/src/xilinx_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-04 14:11:00.000000 xilinx-language-server-0.0.2/src/xilinx_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-04 14:11:00.000000 xilinx-language-server-0.0.2/src/xilinx_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 14:11:00.000000 xilinx-language-server-0.0.2/src/xilinx_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:11:00.491085 xilinx-language-server-0.0.2/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:11:00.495085 xilinx-language-server-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-04 14:10:47.000000 xilinx-language-server-0.0.2/tests/server_test.py
```

### Comparing `xilinx-language-server-0.0.1/.github/workflows/main.yml` & `xilinx-language-server-0.0.2/.github/workflows/main.yml`

 * *Files 4% similar despite different names*

```diff
@@ -88,9 +88,9 @@
   deploy:
     needs: build
     runs-on: ubuntu-latest
     if: startsWith(github.ref, 'refs/tags/')
     steps:
       - uses: Freed-Wu/update-aur-package@v1.0.11
         with:
-          package_name: python-autoconf-language-server
+          package_name: python-xilinx-language-server
           ssh_private_key: ${{secrets.AUR_SSH_PRIVATE_KEY}}
```

### Comparing `xilinx-language-server-0.0.1/.gitignore` & `xilinx-language-server-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.1/.pre-commit-config.yaml` & `xilinx-language-server-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.1/LICENSE` & `xilinx-language-server-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.1/PKG-INFO` & `xilinx-language-server-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xilinx-language-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: xilinx language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://xilinx-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/xilinx-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/xilinx-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/xilinx-language-server
```

### Comparing `xilinx-language-server-0.0.1/README.md` & `xilinx-language-server-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.1/docs/conf.py` & `xilinx-language-server-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.1/docs/resources/configure.md` & `xilinx-language-server-0.0.2/docs/resources/configure.md`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.1/docs/resources/install.md` & `xilinx-language-server-0.0.2/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.1/flake.nix` & `xilinx-language-server-0.0.2/flake.nix`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.1/pyproject.toml` & `xilinx-language-server-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.1/scripts/xilinx.tcl` & `xilinx-language-server-0.0.2/scripts/xilinx.tcl`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.1/src/xilinx_language_server/__main__.py` & `xilinx-language-server-0.0.2/src/xilinx_language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.1/src/xilinx_language_server/assets/json/vivado.json` & `xilinx-language-server-0.0.2/src/xilinx_language_server/assets/json/vivado.json`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.1/src/xilinx_language_server/assets/json/xsct.json` & `xilinx-language-server-0.0.2/src/xilinx_language_server/assets/json/xsct.json`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.1/src/xilinx_language_server/server.py` & `xilinx-language-server-0.0.2/src/xilinx_language_server/server.py`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.1/src/xilinx_language_server.egg-info/PKG-INFO` & `xilinx-language-server-0.0.2/src/xilinx_language_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xilinx-language-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: xilinx language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://xilinx-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/xilinx-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/xilinx-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/xilinx-language-server
```

### Comparing `xilinx-language-server-0.0.1/src/xilinx_language_server.egg-info/SOURCES.txt` & `xilinx-language-server-0.0.2/src/xilinx_language_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

