# Comparing `tmp/wiptools-1.1.8.dev0.tar.gz` & `tmp/wiptools-1.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiptools-1.1.8.dev0.tar", max compression
+gzip compressed data, was "wiptools-1.2.0.dev0.tar", max compression
```

## Comparing `wiptools-1.1.8.dev0.tar` & `wiptools-1.2.0.dev0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     5546 2023-06-29 19:52:45.482871 wiptools-1.1.8.dev0/README.md
--rw-r--r--   0        0        0      948 2023-07-04 06:15:15.636937 wiptools-1.1.8.dev0/pyproject.toml
--rw-r--r--   0        0        0      421 2023-07-03 17:45:37.564175 wiptools-1.1.8.dev0/wiptools/__init__.py
--rw-r--r--   0        0        0      314 2023-06-23 17:25:33.781000 wiptools-1.1.8.dev0/wiptools/cookiecutters/CLI/cookiecutter.json
--rw-r--r--   0        0        0      566 2023-06-23 17:29:04.291000 wiptools-1.1.8.dev0/wiptools/cookiecutters/CLI/{{cookiecutter.cli_name}}/__main__.py
--rw-r--r--   0        0        0      314 2023-06-23 17:06:47.262000 wiptools-1.1.8.dev0/wiptools/cookiecutters/CLI-tests/cookiecutter.json
--rw-r--r--   0        0        0      983 2023-06-25 07:36:17.254000 wiptools-1.1.8.dev0/wiptools/cookiecutters/CLI-tests/{{cookiecutter.cli_name}}/test_{{cookiecutter.cli_name}}.py
--rw-r--r--   0        0        0      314 2023-06-23 17:06:47.212000 wiptools-1.1.8.dev0/wiptools/cookiecutters/CLIsub/cookiecutter.json
--rw-r--r--   0        0        0     1152 2023-06-23 17:10:10.782000 wiptools-1.1.8.dev0/wiptools/cookiecutters/CLIsub/{{cookiecutter.cli_name}}/__main__.py
--rw-r--r--   0        0        0      314 2023-06-23 17:06:47.220000 wiptools-1.1.8.dev0/wiptools/cookiecutters/CLIsub-tests/cookiecutter.json
--rw-r--r--   0        0        0     1121 2023-06-25 07:36:17.262000 wiptools-1.1.8.dev0/wiptools/cookiecutters/CLIsub-tests/{{cookiecutter.cli_name}}/test_{{cookiecutter.cli_name}}.py
--rw-r--r--   0        0        0      359 2023-06-24 10:05:46.230000 wiptools-1.1.8.dev0/wiptools/cookiecutters/module-cpp/cookiecutter.json
--rw-r--r--   0        0        0     1282 2023-06-29 15:57:43.946774 wiptools-1.1.8.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/CMakeLists.txt
--rw-r--r--   0        0        0     2045 2023-06-26 13:34:36.443000 wiptools-1.1.8.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.cpp
--rw-r--r--   0        0        0      745 2023-06-23 17:08:39.250000 wiptools-1.1.8.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.md
--rw-r--r--   0        0        0      359 2023-06-24 10:05:46.299000 wiptools-1.1.8.dev0/wiptools/cookiecutters/module-cpp-tests/cookiecutter.json
--rw-r--r--   0        0        0     1116 2023-06-23 17:12:35.564000 wiptools-1.1.8.dev0/wiptools/cookiecutters/module-cpp-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py
--rw-r--r--   0        0        0      359 2023-06-24 10:05:46.139000 wiptools-1.1.8.dev0/wiptools/cookiecutters/module-f90/cookiecutter.json
--rw-r--r--   0        0        0    11792 2023-06-26 13:26:20.538000 wiptools-1.1.8.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/CMakeLists.txt
--rw-r--r--   0        0        0     1708 2023-06-23 17:15:31.403000 wiptools-1.1.8.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.f90
--rw-r--r--   0        0        0      740 2023-06-23 17:04:56.212000 wiptools-1.1.8.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.md
--rw-r--r--   0        0        0      359 2023-06-24 10:05:46.325000 wiptools-1.1.8.dev0/wiptools/cookiecutters/module-f90-tests/cookiecutter.json
--rw-r--r--   0        0        0     1070 2023-06-23 16:52:48.135000 wiptools-1.1.8.dev0/wiptools/cookiecutters/module-f90-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py
--rw-r--r--   0        0        0      392 2023-06-23 16:56:29.101000 wiptools-1.1.8.dev0/wiptools/cookiecutters/module-py/cookiecutter.json
--rw-r--r--   0        0        0      279 2023-06-23 16:54:10.188000 wiptools-1.1.8.dev0/wiptools/cookiecutters/module-py/{{cookiecutter.module_name}}/__init__.py
--rw-r--r--   0        0        0      395 2023-06-23 15:38:15.028000 wiptools-1.1.8.dev0/wiptools/cookiecutters/module-py-tests/cookiecutter.json
--rw-r--r--   0        0        0     1090 2023-06-23 16:56:29.088000 wiptools-1.1.8.dev0/wiptools/cookiecutters/module-py-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py
--rw-r--r--   0        0        0      288 2023-06-22 08:11:50.824000 wiptools-1.1.8.dev0/wiptools/cookiecutters/project/cookiecutter.json
--rw-r--r--   0        0        0      484 2023-06-20 09:30:08.312000 wiptools-1.1.8.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/.bumpversion.cfg
--rw-r--r--   0        0        0     1358 2023-06-15 12:46:19.330000 wiptools-1.1.8.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0        0        0       44 2023-06-20 09:43:36.153000 wiptools-1.1.8.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/CHANGELOG.md
--rw-r--r--   0        0        0       91 2023-06-27 08:35:24.530000 wiptools-1.1.8.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0      877 2023-06-23 13:33:37.094000 wiptools-1.1.8.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      998 2023-06-15 12:46:19.331000 wiptools-1.1.8.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/tests/{{cookiecutter.package_name}}/test_{{cookiecutter.package_name}}.py
--rw-r--r--   0        0        0      299 2023-06-22 13:58:15.183000 wiptools-1.1.8.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/{{cookiecutter.package_name}}/__init__.py
--rw-r--r--   0        0        0      288 2023-06-22 08:11:50.824000 wiptools-1.1.8.dev0/wiptools/cookiecutters/project-doc-md/cookiecutter.json
--rw-r--r--   0        0        0      230 2023-06-21 19:25:21.826000 wiptools-1.1.8.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/docs/api-reference.md
--rw-r--r--   0        0        0      175 2023-06-21 19:19:36.170000 wiptools-1.1.8.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/docs/index.md
--rw-r--r--   0        0        0       52 2023-06-22 14:00:42.520000 wiptools-1.1.8.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/docs/overview.md
--rw-r--r--   0        0        0     1306 2023-06-23 08:28:09.033000 wiptools-1.1.8.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/mkdocs.yml
--rw-r--r--   0        0        0     2906 2023-07-02 18:33:39.611013 wiptools-1.1.8.dev0/wiptools/messages.py
--rw-r--r--   0        0        0     8675 2023-07-03 13:05:00.070213 wiptools-1.1.8.dev0/wiptools/utils.py
--rw-r--r--   0        0        0     6206 2023-07-03 17:41:00.405537 wiptools-1.1.8.dev0/wiptools/wip/__main__.py
--rw-r--r--   0        0        0     5143 2023-06-29 11:14:02.842414 wiptools-1.1.8.dev0/wiptools/wip/wip_add.py
--rw-r--r--   0        0        0     2766 2023-07-02 18:58:31.016388 wiptools-1.1.8.dev0/wiptools/wip/wip_build.py
--rw-r--r--   0        0        0      701 2023-07-02 18:58:30.971107 wiptools-1.1.8.dev0/wiptools/wip/wip_bump.py
--rw-r--r--   0        0        0     4249 2023-07-02 16:31:00.183628 wiptools-1.1.8.dev0/wiptools/wip/wip_docs.py
--rw-r--r--   0        0        0      812 2023-06-23 08:39:24.708000 wiptools-1.1.8.dev0/wiptools/wip/wip_env.py
--rw-r--r--   0        0        0     5104 2023-07-03 17:46:33.347688 wiptools-1.1.8.dev0/wiptools/wip/wip_info.py
--rw-r--r--   0        0        0     5481 2023-07-03 17:32:56.506909 wiptools-1.1.8.dev0/wiptools/wip/wip_init.py
--rw-r--r--   0        0        0     1664 2023-07-02 19:05:31.243703 wiptools-1.1.8.dev0/wiptools/wip/wip_remote_repo.py
--rw-r--r--   0        0        0     6165 1970-01-01 00:00:00.000000 wiptools-1.1.8.dev0/PKG-INFO
+-rw-r--r--   0        0        0     5546 2023-06-29 19:52:45.482871 wiptools-1.2.0.dev0/README.md
+-rw-r--r--   0        0        0      965 2023-07-04 10:23:13.013933 wiptools-1.2.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0      421 2023-07-04 10:23:13.012984 wiptools-1.2.0.dev0/wiptools/__init__.py
+-rw-r--r--   0        0        0      314 2023-06-23 17:25:33.781000 wiptools-1.2.0.dev0/wiptools/cookiecutters/CLI/cookiecutter.json
+-rw-r--r--   0        0        0      566 2023-06-23 17:29:04.291000 wiptools-1.2.0.dev0/wiptools/cookiecutters/CLI/{{cookiecutter.cli_name}}/__main__.py
+-rw-r--r--   0        0        0      314 2023-06-23 17:06:47.262000 wiptools-1.2.0.dev0/wiptools/cookiecutters/CLI-tests/cookiecutter.json
+-rw-r--r--   0        0        0      983 2023-06-25 07:36:17.254000 wiptools-1.2.0.dev0/wiptools/cookiecutters/CLI-tests/{{cookiecutter.cli_name}}/test_{{cookiecutter.cli_name}}.py
+-rw-r--r--   0        0        0      314 2023-06-23 17:06:47.212000 wiptools-1.2.0.dev0/wiptools/cookiecutters/CLIsub/cookiecutter.json
+-rw-r--r--   0        0        0     1152 2023-06-23 17:10:10.782000 wiptools-1.2.0.dev0/wiptools/cookiecutters/CLIsub/{{cookiecutter.cli_name}}/__main__.py
+-rw-r--r--   0        0        0      314 2023-06-23 17:06:47.220000 wiptools-1.2.0.dev0/wiptools/cookiecutters/CLIsub-tests/cookiecutter.json
+-rw-r--r--   0        0        0     1121 2023-06-25 07:36:17.262000 wiptools-1.2.0.dev0/wiptools/cookiecutters/CLIsub-tests/{{cookiecutter.cli_name}}/test_{{cookiecutter.cli_name}}.py
+-rw-r--r--   0        0        0      359 2023-06-24 10:05:46.230000 wiptools-1.2.0.dev0/wiptools/cookiecutters/module-cpp/cookiecutter.json
+-rw-r--r--   0        0        0     1282 2023-06-29 15:57:43.946774 wiptools-1.2.0.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/CMakeLists.txt
+-rw-r--r--   0        0        0     2045 2023-06-26 13:34:36.443000 wiptools-1.2.0.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.cpp
+-rw-r--r--   0        0        0      745 2023-06-23 17:08:39.250000 wiptools-1.2.0.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.md
+-rw-r--r--   0        0        0      359 2023-06-24 10:05:46.299000 wiptools-1.2.0.dev0/wiptools/cookiecutters/module-cpp-tests/cookiecutter.json
+-rw-r--r--   0        0        0     1116 2023-06-23 17:12:35.564000 wiptools-1.2.0.dev0/wiptools/cookiecutters/module-cpp-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py
+-rw-r--r--   0        0        0      359 2023-06-24 10:05:46.139000 wiptools-1.2.0.dev0/wiptools/cookiecutters/module-f90/cookiecutter.json
+-rw-r--r--   0        0        0    11792 2023-06-26 13:26:20.538000 wiptools-1.2.0.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/CMakeLists.txt
+-rw-r--r--   0        0        0     1708 2023-06-23 17:15:31.403000 wiptools-1.2.0.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.f90
+-rw-r--r--   0        0        0      740 2023-06-23 17:04:56.212000 wiptools-1.2.0.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.md
+-rw-r--r--   0        0        0      359 2023-06-24 10:05:46.325000 wiptools-1.2.0.dev0/wiptools/cookiecutters/module-f90-tests/cookiecutter.json
+-rw-r--r--   0        0        0     1070 2023-06-23 16:52:48.135000 wiptools-1.2.0.dev0/wiptools/cookiecutters/module-f90-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py
+-rw-r--r--   0        0        0      392 2023-06-23 16:56:29.101000 wiptools-1.2.0.dev0/wiptools/cookiecutters/module-py/cookiecutter.json
+-rw-r--r--   0        0        0      279 2023-06-23 16:54:10.188000 wiptools-1.2.0.dev0/wiptools/cookiecutters/module-py/{{cookiecutter.module_name}}/__init__.py
+-rw-r--r--   0        0        0      395 2023-06-23 15:38:15.028000 wiptools-1.2.0.dev0/wiptools/cookiecutters/module-py-tests/cookiecutter.json
+-rw-r--r--   0        0        0     1090 2023-06-23 16:56:29.088000 wiptools-1.2.0.dev0/wiptools/cookiecutters/module-py-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py
+-rw-r--r--   0        0        0      288 2023-06-22 08:11:50.824000 wiptools-1.2.0.dev0/wiptools/cookiecutters/project/cookiecutter.json
+-rw-r--r--   0        0        0      484 2023-06-20 09:30:08.312000 wiptools-1.2.0.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/.bumpversion.cfg
+-rw-r--r--   0        0        0     1358 2023-06-15 12:46:19.330000 wiptools-1.2.0.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0       44 2023-06-20 09:43:36.153000 wiptools-1.2.0.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/CHANGELOG.md
+-rw-r--r--   0        0        0       91 2023-06-27 08:35:24.530000 wiptools-1.2.0.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0      877 2023-06-23 13:33:37.094000 wiptools-1.2.0.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      998 2023-06-15 12:46:19.331000 wiptools-1.2.0.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/tests/{{cookiecutter.package_name}}/test_{{cookiecutter.package_name}}.py
+-rw-r--r--   0        0        0      299 2023-06-22 13:58:15.183000 wiptools-1.2.0.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/{{cookiecutter.package_name}}/__init__.py
+-rw-r--r--   0        0        0      288 2023-06-22 08:11:50.824000 wiptools-1.2.0.dev0/wiptools/cookiecutters/project-doc-md/cookiecutter.json
+-rw-r--r--   0        0        0      230 2023-06-21 19:25:21.826000 wiptools-1.2.0.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/docs/api-reference.md
+-rw-r--r--   0        0        0      175 2023-06-21 19:19:36.170000 wiptools-1.2.0.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/docs/index.md
+-rw-r--r--   0        0        0       52 2023-06-22 14:00:42.520000 wiptools-1.2.0.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/docs/overview.md
+-rw-r--r--   0        0        0     1306 2023-06-23 08:28:09.033000 wiptools-1.2.0.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/mkdocs.yml
+-rw-r--r--   0        0        0     2906 2023-07-02 18:33:39.611013 wiptools-1.2.0.dev0/wiptools/messages.py
+-rw-r--r--   0        0        0     8558 2023-07-04 08:01:05.054352 wiptools-1.2.0.dev0/wiptools/utils.py
+-rw-r--r--   0        0        0     6206 2023-07-03 17:41:00.405537 wiptools-1.2.0.dev0/wiptools/wip/__main__.py
+-rw-r--r--   0        0        0     5111 2023-07-04 07:55:39.185284 wiptools-1.2.0.dev0/wiptools/wip/wip_add.py
+-rw-r--r--   0        0        0     2736 2023-07-04 07:55:39.097212 wiptools-1.2.0.dev0/wiptools/wip/wip_build.py
+-rw-r--r--   0        0        0      701 2023-07-02 18:58:30.971107 wiptools-1.2.0.dev0/wiptools/wip/wip_bump.py
+-rw-r--r--   0        0        0     4217 2023-07-04 08:01:04.936441 wiptools-1.2.0.dev0/wiptools/wip/wip_docs.py
+-rw-r--r--   0        0        0     4077 2023-07-04 10:12:07.181977 wiptools-1.2.0.dev0/wiptools/wip/wip_env.py
+-rw-r--r--   0        0        0     5104 2023-07-03 17:46:33.347688 wiptools-1.2.0.dev0/wiptools/wip/wip_info.py
+-rw-r--r--   0        0        0     5481 2023-07-03 17:32:56.506909 wiptools-1.2.0.dev0/wiptools/wip/wip_init.py
+-rw-r--r--   0        0        0     1664 2023-07-02 19:05:31.243703 wiptools-1.2.0.dev0/wiptools/wip/wip_remote_repo.py
+-rw-r--r--   0        0        0     6290 1970-01-01 00:00:00.000000 wiptools-1.2.0.dev0/PKG-INFO
```

### Comparing `wiptools-1.1.8.dev0/README.md` & `wiptools-1.2.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/pyproject.toml` & `wiptools-1.2.0.dev0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "wiptools"
-version = "1.1.8-dev"
+version = "1.2.0-dev"
 description = "Python project skeleton and management"
 authors = ["Bert Tijskens <engelbert.tijskens@uantwerpen.be>"]
 license = "MIT"
 
 readme = 'README.md'
 
 repository = "https://github.com/etijskens/wiptools"
 homepage = "https://etijskens.github.io/wiptools"
 
 keywords = []
 
 [tool.poetry.dependencies]
 python = "^3.9"
-
-[tool.poetry.group.dev.dependencies]
-bump2version = "^1.0.1"
-pytest = "^7.3.2"
 cookiecutter = "^2.1.1"
 tomlkit = "^0.11.8"
+click = "^8.1.3"
+
+[tool.poetry.group.dev.dependencies]
 nanobind = "^1.4.0"
 numpy = "^1.25.0"
+bump2version = "^1.0.1"
+pytest = "^7.3.2"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.3"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 mkdocs-material = "^9.1.16"
 mkdocs-autorefs = "^0.4.1"
 mkdocs-click = "^0.8.0"
```

### Comparing `wiptools-1.1.8.dev0/wiptools/cookiecutters/CLI/{{cookiecutter.cli_name}}/__main__.py` & `wiptools-1.2.0.dev0/wiptools/cookiecutters/CLI/{{cookiecutter.cli_name}}/__main__.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/cookiecutters/CLI-tests/{{cookiecutter.cli_name}}/test_{{cookiecutter.cli_name}}.py` & `wiptools-1.2.0.dev0/wiptools/cookiecutters/CLI-tests/{{cookiecutter.cli_name}}/test_{{cookiecutter.cli_name}}.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/cookiecutters/CLIsub/{{cookiecutter.cli_name}}/__main__.py` & `wiptools-1.2.0.dev0/wiptools/cookiecutters/CLIsub/{{cookiecutter.cli_name}}/__main__.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/cookiecutters/CLIsub-tests/{{cookiecutter.cli_name}}/test_{{cookiecutter.cli_name}}.py` & `wiptools-1.2.0.dev0/wiptools/cookiecutters/CLIsub-tests/{{cookiecutter.cli_name}}/test_{{cookiecutter.cli_name}}.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/CMakeLists.txt` & `wiptools-1.2.0.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.cpp` & `wiptools-1.2.0.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.cpp`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.md` & `wiptools-1.2.0.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.md`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/cookiecutters/module-cpp-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py` & `wiptools-1.2.0.dev0/wiptools/cookiecutters/module-cpp-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/CMakeLists.txt` & `wiptools-1.2.0.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.f90` & `wiptools-1.2.0.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.f90`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.md` & `wiptools-1.2.0.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.md`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/cookiecutters/module-f90-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py` & `wiptools-1.2.0.dev0/wiptools/cookiecutters/module-f90-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/cookiecutters/module-py-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py` & `wiptools-1.2.0.dev0/wiptools/cookiecutters/module-py-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/.gitignore` & `wiptools-1.2.0.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/pyproject.toml` & `wiptools-1.2.0.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/tests/{{cookiecutter.package_name}}/test_{{cookiecutter.package_name}}.py` & `wiptools-1.2.0.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/tests/{{cookiecutter.package_name}}/test_{{cookiecutter.package_name}}.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/mkdocs.yml` & `wiptools-1.2.0.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/messages.py` & `wiptools-1.2.0.dev0/wiptools/messages.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/utils.py` & `wiptools-1.2.0.dev0/wiptools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 from contextlib import contextmanager
 import json
 import os
 from pathlib import Path
 import re
 import subprocess
-
-# try:
-#     import tomllib
-# except ModuleNotFoundError:
-#     import tomli as tomllib
-# import tomli_w as tomli_w
-import tomlkit
 from typing import List, Union, Tuple, Callable
 
 import click
+import tomlkit
 
 import wiptools.messages as messages
 
 
 PROJECT_PATH = None
 # After succesfully executing read_wip_cookiecutter_json() this variabel contains the project path.
```

### Comparing `wiptools-1.1.8.dev0/wiptools/wip/__main__.py` & `wiptools-1.2.0.dev0/wiptools/wip/__main__.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/wip/wip_add.py` & `wiptools-1.2.0.dev0/wiptools/wip/wip_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # -*- coding: utf-8 -*-
 import os
 from pathlib import Path
-import shutil
-import subprocess
 
 import click
 from cookiecutter.main import cookiecutter
 
 import wiptools.messages as messages
 import wiptools.utils as utils
```

### Comparing `wiptools-1.1.8.dev0/wiptools/wip/wip_build.py` & `wiptools-1.2.0.dev0/wiptools/wip/wip_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # -*- coding: utf-8 -*-
-import json
 from pathlib import Path
-import subprocess
 
 import click
 
 import wiptools.messages as messages
 import wiptools.utils as utils
```

### Comparing `wiptools-1.1.8.dev0/wiptools/wip/wip_bump.py` & `wiptools-1.2.0.dev0/wiptools/wip/wip_bump.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/wip/wip_docs.py` & `wiptools-1.2.0.dev0/wiptools/wip/wip_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # -*- coding: utf-8 -*-
 
 import os
 from pathlib import Path
-import shutil
-import subprocess
 
 import click
 from cookiecutter.main import cookiecutter
 
 from wiptools import COMPONENT_TYPES, DOCUMENTATION_FORMATS
 import wiptools.messages as messages
 import wiptools.utils as utils
```

### Comparing `wiptools-1.1.8.dev0/wiptools/wip/wip_info.py` & `wiptools-1.2.0.dev0/wiptools/wip/wip_info.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/wip/wip_init.py` & `wiptools-1.2.0.dev0/wiptools/wip/wip_init.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/wiptools/wip/wip_remote_repo.py` & `wiptools-1.2.0.dev0/wiptools/wip/wip_remote_repo.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.1.8.dev0/PKG-INFO` & `wiptools-1.2.0.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: wiptools
-Version: 1.1.8.dev0
+Version: 1.2.0.dev0
 Summary: Python project skeleton and management
 Home-page: https://etijskens.github.io/wiptools
 License: MIT
 Author: Bert Tijskens
 Author-email: engelbert.tijskens@uantwerpen.be
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
+Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
 Project-URL: Repository, https://github.com/etijskens/wiptools
 Description-Content-Type: text/markdown
 
 # Python package wiptools
 
 Python project skeleton set up and management.
```

