# Comparing `tmp/wiptools-1.2.5.dev0.tar.gz` & `tmp/wiptools-1.2.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiptools-1.2.5.dev0.tar", max compression
+gzip compressed data, was "wiptools-1.2.6.dev0.tar", max compression
```

## Comparing `wiptools-1.2.5.dev0.tar` & `wiptools-1.2.6.dev0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     5546 2023-06-29 19:52:45.482871 wiptools-1.2.5.dev0/README.md
--rw-r--r--   0        0        0      985 2023-07-04 15:39:08.447403 wiptools-1.2.5.dev0/pyproject.toml
--rw-r--r--   0        0        0      421 2023-07-04 15:39:08.446396 wiptools-1.2.5.dev0/wiptools/__init__.py
--rw-r--r--   0        0        0      314 2023-06-23 17:25:33.781000 wiptools-1.2.5.dev0/wiptools/cookiecutters/CLI/cookiecutter.json
--rw-r--r--   0        0        0      566 2023-06-23 17:29:04.291000 wiptools-1.2.5.dev0/wiptools/cookiecutters/CLI/{{cookiecutter.cli_name}}/__main__.py
--rw-r--r--   0        0        0      314 2023-06-23 17:06:47.262000 wiptools-1.2.5.dev0/wiptools/cookiecutters/CLI-tests/cookiecutter.json
--rw-r--r--   0        0        0      983 2023-06-25 07:36:17.254000 wiptools-1.2.5.dev0/wiptools/cookiecutters/CLI-tests/{{cookiecutter.cli_name}}/test_{{cookiecutter.cli_name}}.py
--rw-r--r--   0        0        0      314 2023-06-23 17:06:47.212000 wiptools-1.2.5.dev0/wiptools/cookiecutters/CLIsub/cookiecutter.json
--rw-r--r--   0        0        0     1152 2023-06-23 17:10:10.782000 wiptools-1.2.5.dev0/wiptools/cookiecutters/CLIsub/{{cookiecutter.cli_name}}/__main__.py
--rw-r--r--   0        0        0      314 2023-06-23 17:06:47.220000 wiptools-1.2.5.dev0/wiptools/cookiecutters/CLIsub-tests/cookiecutter.json
--rw-r--r--   0        0        0     1121 2023-06-25 07:36:17.262000 wiptools-1.2.5.dev0/wiptools/cookiecutters/CLIsub-tests/{{cookiecutter.cli_name}}/test_{{cookiecutter.cli_name}}.py
--rw-r--r--   0        0        0      359 2023-06-24 10:05:46.230000 wiptools-1.2.5.dev0/wiptools/cookiecutters/module-cpp/cookiecutter.json
--rw-r--r--   0        0        0     1282 2023-06-29 15:57:43.946774 wiptools-1.2.5.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/CMakeLists.txt
--rw-r--r--   0        0        0     2045 2023-06-26 13:34:36.443000 wiptools-1.2.5.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.cpp
--rw-r--r--   0        0        0      745 2023-06-23 17:08:39.250000 wiptools-1.2.5.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.md
--rw-r--r--   0        0        0      359 2023-06-24 10:05:46.299000 wiptools-1.2.5.dev0/wiptools/cookiecutters/module-cpp-tests/cookiecutter.json
--rw-r--r--   0        0        0     1116 2023-06-23 17:12:35.564000 wiptools-1.2.5.dev0/wiptools/cookiecutters/module-cpp-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py
--rw-r--r--   0        0        0      359 2023-06-24 10:05:46.139000 wiptools-1.2.5.dev0/wiptools/cookiecutters/module-f90/cookiecutter.json
--rw-r--r--   0        0        0    11792 2023-06-26 13:26:20.538000 wiptools-1.2.5.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/CMakeLists.txt
--rw-r--r--   0        0        0     1708 2023-06-23 17:15:31.403000 wiptools-1.2.5.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.f90
--rw-r--r--   0        0        0      740 2023-06-23 17:04:56.212000 wiptools-1.2.5.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.md
--rw-r--r--   0        0        0      359 2023-06-24 10:05:46.325000 wiptools-1.2.5.dev0/wiptools/cookiecutters/module-f90-tests/cookiecutter.json
--rw-r--r--   0        0        0     1070 2023-06-23 16:52:48.135000 wiptools-1.2.5.dev0/wiptools/cookiecutters/module-f90-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py
--rw-r--r--   0        0        0      392 2023-06-23 16:56:29.101000 wiptools-1.2.5.dev0/wiptools/cookiecutters/module-py/cookiecutter.json
--rw-r--r--   0        0        0      279 2023-06-23 16:54:10.188000 wiptools-1.2.5.dev0/wiptools/cookiecutters/module-py/{{cookiecutter.module_name}}/__init__.py
--rw-r--r--   0        0        0      395 2023-06-23 15:38:15.028000 wiptools-1.2.5.dev0/wiptools/cookiecutters/module-py-tests/cookiecutter.json
--rw-r--r--   0        0        0     1090 2023-06-23 16:56:29.088000 wiptools-1.2.5.dev0/wiptools/cookiecutters/module-py-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py
--rw-r--r--   0        0        0      288 2023-06-22 08:11:50.824000 wiptools-1.2.5.dev0/wiptools/cookiecutters/project/cookiecutter.json
--rw-r--r--   0        0        0      484 2023-06-20 09:30:08.312000 wiptools-1.2.5.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/.bumpversion.cfg
--rw-r--r--   0        0        0     1358 2023-06-15 12:46:19.330000 wiptools-1.2.5.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0        0        0       44 2023-06-20 09:43:36.153000 wiptools-1.2.5.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/CHANGELOG.md
--rw-r--r--   0        0        0       91 2023-06-27 08:35:24.530000 wiptools-1.2.5.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0      877 2023-06-23 13:33:37.094000 wiptools-1.2.5.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      998 2023-06-15 12:46:19.331000 wiptools-1.2.5.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/tests/{{cookiecutter.package_name}}/test_{{cookiecutter.package_name}}.py
--rw-r--r--   0        0        0      299 2023-06-22 13:58:15.183000 wiptools-1.2.5.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/{{cookiecutter.package_name}}/__init__.py
--rw-r--r--   0        0        0      288 2023-06-22 08:11:50.824000 wiptools-1.2.5.dev0/wiptools/cookiecutters/project-doc-md/cookiecutter.json
--rw-r--r--   0        0        0      230 2023-06-21 19:25:21.826000 wiptools-1.2.5.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/docs/api-reference.md
--rw-r--r--   0        0        0      175 2023-06-21 19:19:36.170000 wiptools-1.2.5.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/docs/index.md
--rw-r--r--   0        0        0       52 2023-06-22 14:00:42.520000 wiptools-1.2.5.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/docs/overview.md
--rw-r--r--   0        0        0     1306 2023-06-23 08:28:09.033000 wiptools-1.2.5.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/mkdocs.yml
--rw-r--r--   0        0        0     2906 2023-07-02 18:33:39.611013 wiptools-1.2.5.dev0/wiptools/messages.py
--rw-r--r--   0        0        0     8558 2023-07-04 08:01:05.054352 wiptools-1.2.5.dev0/wiptools/utils.py
--rw-r--r--   0        0        0     6343 2023-07-04 15:10:38.448146 wiptools-1.2.5.dev0/wiptools/wip/__main__.py
--rw-r--r--   0        0        0     5111 2023-07-04 07:55:39.185284 wiptools-1.2.5.dev0/wiptools/wip/wip_add.py
--rw-r--r--   0        0        0     2736 2023-07-04 07:55:39.097212 wiptools-1.2.5.dev0/wiptools/wip/wip_build.py
--rw-r--r--   0        0        0      701 2023-07-02 18:58:30.971107 wiptools-1.2.5.dev0/wiptools/wip/wip_bump.py
--rw-r--r--   0        0        0     4217 2023-07-04 08:01:04.936441 wiptools-1.2.5.dev0/wiptools/wip/wip_docs.py
--rw-r--r--   0        0        0     4061 2023-07-04 15:38:05.273649 wiptools-1.2.5.dev0/wiptools/wip/wip_env.py
--rw-r--r--   0        0        0     5213 2023-07-04 15:10:38.335164 wiptools-1.2.5.dev0/wiptools/wip/wip_info.py
--rw-r--r--   0        0        0     5481 2023-07-03 17:32:56.506909 wiptools-1.2.5.dev0/wiptools/wip/wip_init.py
--rw-r--r--   0        0        0     1664 2023-07-02 19:05:31.243703 wiptools-1.2.5.dev0/wiptools/wip/wip_remote_repo.py
--rw-r--r--   0        0        0     6330 1970-01-01 00:00:00.000000 wiptools-1.2.5.dev0/PKG-INFO
+-rw-r--r--   0        0        0     5546 2023-06-29 19:52:45.482871 wiptools-1.2.6.dev0/README.md
+-rw-r--r--   0        0        0      985 2023-07-04 15:54:42.352450 wiptools-1.2.6.dev0/pyproject.toml
+-rw-r--r--   0        0        0      421 2023-07-04 15:54:42.351471 wiptools-1.2.6.dev0/wiptools/__init__.py
+-rw-r--r--   0        0        0      314 2023-06-23 17:25:33.781000 wiptools-1.2.6.dev0/wiptools/cookiecutters/CLI/cookiecutter.json
+-rw-r--r--   0        0        0      566 2023-06-23 17:29:04.291000 wiptools-1.2.6.dev0/wiptools/cookiecutters/CLI/{{cookiecutter.cli_name}}/__main__.py
+-rw-r--r--   0        0        0      314 2023-06-23 17:06:47.262000 wiptools-1.2.6.dev0/wiptools/cookiecutters/CLI-tests/cookiecutter.json
+-rw-r--r--   0        0        0      983 2023-06-25 07:36:17.254000 wiptools-1.2.6.dev0/wiptools/cookiecutters/CLI-tests/{{cookiecutter.cli_name}}/test_{{cookiecutter.cli_name}}.py
+-rw-r--r--   0        0        0      314 2023-06-23 17:06:47.212000 wiptools-1.2.6.dev0/wiptools/cookiecutters/CLIsub/cookiecutter.json
+-rw-r--r--   0        0        0     1152 2023-06-23 17:10:10.782000 wiptools-1.2.6.dev0/wiptools/cookiecutters/CLIsub/{{cookiecutter.cli_name}}/__main__.py
+-rw-r--r--   0        0        0      314 2023-06-23 17:06:47.220000 wiptools-1.2.6.dev0/wiptools/cookiecutters/CLIsub-tests/cookiecutter.json
+-rw-r--r--   0        0        0     1121 2023-06-25 07:36:17.262000 wiptools-1.2.6.dev0/wiptools/cookiecutters/CLIsub-tests/{{cookiecutter.cli_name}}/test_{{cookiecutter.cli_name}}.py
+-rw-r--r--   0        0        0      359 2023-06-24 10:05:46.230000 wiptools-1.2.6.dev0/wiptools/cookiecutters/module-cpp/cookiecutter.json
+-rw-r--r--   0        0        0     1282 2023-06-29 15:57:43.946774 wiptools-1.2.6.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/CMakeLists.txt
+-rw-r--r--   0        0        0     2045 2023-06-26 13:34:36.443000 wiptools-1.2.6.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.cpp
+-rw-r--r--   0        0        0      745 2023-06-23 17:08:39.250000 wiptools-1.2.6.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.md
+-rw-r--r--   0        0        0      359 2023-06-24 10:05:46.299000 wiptools-1.2.6.dev0/wiptools/cookiecutters/module-cpp-tests/cookiecutter.json
+-rw-r--r--   0        0        0     1116 2023-06-23 17:12:35.564000 wiptools-1.2.6.dev0/wiptools/cookiecutters/module-cpp-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py
+-rw-r--r--   0        0        0      359 2023-06-24 10:05:46.139000 wiptools-1.2.6.dev0/wiptools/cookiecutters/module-f90/cookiecutter.json
+-rw-r--r--   0        0        0    11792 2023-06-26 13:26:20.538000 wiptools-1.2.6.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/CMakeLists.txt
+-rw-r--r--   0        0        0     1708 2023-06-23 17:15:31.403000 wiptools-1.2.6.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.f90
+-rw-r--r--   0        0        0      740 2023-06-23 17:04:56.212000 wiptools-1.2.6.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.md
+-rw-r--r--   0        0        0      359 2023-06-24 10:05:46.325000 wiptools-1.2.6.dev0/wiptools/cookiecutters/module-f90-tests/cookiecutter.json
+-rw-r--r--   0        0        0     1070 2023-06-23 16:52:48.135000 wiptools-1.2.6.dev0/wiptools/cookiecutters/module-f90-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py
+-rw-r--r--   0        0        0      392 2023-06-23 16:56:29.101000 wiptools-1.2.6.dev0/wiptools/cookiecutters/module-py/cookiecutter.json
+-rw-r--r--   0        0        0      279 2023-06-23 16:54:10.188000 wiptools-1.2.6.dev0/wiptools/cookiecutters/module-py/{{cookiecutter.module_name}}/__init__.py
+-rw-r--r--   0        0        0      395 2023-06-23 15:38:15.028000 wiptools-1.2.6.dev0/wiptools/cookiecutters/module-py-tests/cookiecutter.json
+-rw-r--r--   0        0        0     1090 2023-06-23 16:56:29.088000 wiptools-1.2.6.dev0/wiptools/cookiecutters/module-py-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py
+-rw-r--r--   0        0        0      288 2023-06-22 08:11:50.824000 wiptools-1.2.6.dev0/wiptools/cookiecutters/project/cookiecutter.json
+-rw-r--r--   0        0        0      484 2023-06-20 09:30:08.312000 wiptools-1.2.6.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/.bumpversion.cfg
+-rw-r--r--   0        0        0     1358 2023-06-15 12:46:19.330000 wiptools-1.2.6.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0       44 2023-06-20 09:43:36.153000 wiptools-1.2.6.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/CHANGELOG.md
+-rw-r--r--   0        0        0       91 2023-06-27 08:35:24.530000 wiptools-1.2.6.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0      877 2023-06-23 13:33:37.094000 wiptools-1.2.6.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      998 2023-06-15 12:46:19.331000 wiptools-1.2.6.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/tests/{{cookiecutter.package_name}}/test_{{cookiecutter.package_name}}.py
+-rw-r--r--   0        0        0      299 2023-06-22 13:58:15.183000 wiptools-1.2.6.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/{{cookiecutter.package_name}}/__init__.py
+-rw-r--r--   0        0        0      288 2023-06-22 08:11:50.824000 wiptools-1.2.6.dev0/wiptools/cookiecutters/project-doc-md/cookiecutter.json
+-rw-r--r--   0        0        0      230 2023-06-21 19:25:21.826000 wiptools-1.2.6.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/docs/api-reference.md
+-rw-r--r--   0        0        0      175 2023-06-21 19:19:36.170000 wiptools-1.2.6.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/docs/index.md
+-rw-r--r--   0        0        0       52 2023-06-22 14:00:42.520000 wiptools-1.2.6.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/docs/overview.md
+-rw-r--r--   0        0        0     1306 2023-06-23 08:28:09.033000 wiptools-1.2.6.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/mkdocs.yml
+-rw-r--r--   0        0        0     2906 2023-07-02 18:33:39.611013 wiptools-1.2.6.dev0/wiptools/messages.py
+-rw-r--r--   0        0        0     8558 2023-07-04 08:01:05.054352 wiptools-1.2.6.dev0/wiptools/utils.py
+-rw-r--r--   0        0        0     6343 2023-07-04 15:10:38.448146 wiptools-1.2.6.dev0/wiptools/wip/__main__.py
+-rw-r--r--   0        0        0     5111 2023-07-04 07:55:39.185284 wiptools-1.2.6.dev0/wiptools/wip/wip_add.py
+-rw-r--r--   0        0        0     2736 2023-07-04 07:55:39.097212 wiptools-1.2.6.dev0/wiptools/wip/wip_build.py
+-rw-r--r--   0        0        0      701 2023-07-02 18:58:30.971107 wiptools-1.2.6.dev0/wiptools/wip/wip_bump.py
+-rw-r--r--   0        0        0     4217 2023-07-04 08:01:04.936441 wiptools-1.2.6.dev0/wiptools/wip/wip_docs.py
+-rw-r--r--   0        0        0     4652 2023-07-04 15:54:07.547600 wiptools-1.2.6.dev0/wiptools/wip/wip_env.py
+-rw-r--r--   0        0        0     5213 2023-07-04 15:10:38.335164 wiptools-1.2.6.dev0/wiptools/wip/wip_info.py
+-rw-r--r--   0        0        0     5481 2023-07-03 17:32:56.506909 wiptools-1.2.6.dev0/wiptools/wip/wip_init.py
+-rw-r--r--   0        0        0     1664 2023-07-02 19:05:31.243703 wiptools-1.2.6.dev0/wiptools/wip/wip_remote_repo.py
+-rw-r--r--   0        0        0     6330 1970-01-01 00:00:00.000000 wiptools-1.2.6.dev0/PKG-INFO
```

### Comparing `wiptools-1.2.5.dev0/README.md` & `wiptools-1.2.6.dev0/README.md`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/pyproject.toml` & `wiptools-1.2.6.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wiptools"
-version = "1.2.5-dev"
+version = "1.2.6-dev"
 description = "Python project skeleton and management"
 authors = ["Bert Tijskens <engelbert.tijskens@uantwerpen.be>"]
 license = "MIT"
 
 readme = 'README.md'
 
 repository = "https://github.com/etijskens/wiptools"
```

### Comparing `wiptools-1.2.5.dev0/wiptools/cookiecutters/CLI/{{cookiecutter.cli_name}}/__main__.py` & `wiptools-1.2.6.dev0/wiptools/cookiecutters/CLI/{{cookiecutter.cli_name}}/__main__.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/cookiecutters/CLI-tests/{{cookiecutter.cli_name}}/test_{{cookiecutter.cli_name}}.py` & `wiptools-1.2.6.dev0/wiptools/cookiecutters/CLI-tests/{{cookiecutter.cli_name}}/test_{{cookiecutter.cli_name}}.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/cookiecutters/CLIsub/{{cookiecutter.cli_name}}/__main__.py` & `wiptools-1.2.6.dev0/wiptools/cookiecutters/CLIsub/{{cookiecutter.cli_name}}/__main__.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/cookiecutters/CLIsub-tests/{{cookiecutter.cli_name}}/test_{{cookiecutter.cli_name}}.py` & `wiptools-1.2.6.dev0/wiptools/cookiecutters/CLIsub-tests/{{cookiecutter.cli_name}}/test_{{cookiecutter.cli_name}}.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/CMakeLists.txt` & `wiptools-1.2.6.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.cpp` & `wiptools-1.2.6.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.cpp`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.md` & `wiptools-1.2.6.dev0/wiptools/cookiecutters/module-cpp/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.md`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/cookiecutters/module-cpp-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py` & `wiptools-1.2.6.dev0/wiptools/cookiecutters/module-cpp-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/CMakeLists.txt` & `wiptools-1.2.6.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.f90` & `wiptools-1.2.6.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.f90`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.md` & `wiptools-1.2.6.dev0/wiptools/cookiecutters/module-f90/{{cookiecutter.module_name}}/{{cookiecutter.module_name}}.md`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/cookiecutters/module-f90-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py` & `wiptools-1.2.6.dev0/wiptools/cookiecutters/module-f90-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/cookiecutters/module-py-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py` & `wiptools-1.2.6.dev0/wiptools/cookiecutters/module-py-tests/{{cookiecutter.module_name}}/test_{{cookiecutter.module_name}}.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/.gitignore` & `wiptools-1.2.6.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/pyproject.toml` & `wiptools-1.2.6.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/tests/{{cookiecutter.package_name}}/test_{{cookiecutter.package_name}}.py` & `wiptools-1.2.6.dev0/wiptools/cookiecutters/project/{{cookiecutter.project_name}}/tests/{{cookiecutter.package_name}}/test_{{cookiecutter.package_name}}.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/mkdocs.yml` & `wiptools-1.2.6.dev0/wiptools/cookiecutters/project-doc-md/{{cookiecutter.project_name}}/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/messages.py` & `wiptools-1.2.6.dev0/wiptools/messages.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/utils.py` & `wiptools-1.2.6.dev0/wiptools/utils.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/wip/__main__.py` & `wiptools-1.2.6.dev0/wiptools/wip/__main__.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/wip/wip_add.py` & `wiptools-1.2.6.dev0/wiptools/wip/wip_add.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/wip/wip_build.py` & `wiptools-1.2.6.dev0/wiptools/wip/wip_build.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/wip/wip_bump.py` & `wiptools-1.2.6.dev0/wiptools/wip/wip_bump.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/wip/wip_docs.py` & `wiptools-1.2.6.dev0/wiptools/wip/wip_docs.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/wip/wip_env.py` & `wiptools-1.2.6.dev0/wiptools/wip/wip_env.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,127 +6,138 @@
 from subprocess import run
 
 import click
 
 import wiptools.messages as messages
 from wiptools.utils import subprocess_run_cmds
 
+
+fg = {
+    0: 'red',
+    1: 'green'
+}
+
 def wip_env(ctx: click.Context):
     """Check the current environment for necessary components."""
 
-    print(("For full `wip` functionality the following commands and packages must be available in our envirionment:\n"))
+    print(("For a full functional `wip` the following commands and packages must be available in our environment:\n"))
 
-    has_python('3.9')
-    has_git('2.35')
-    has_gh('2.31')
-    has_bumpversion('1.0')
-    has_nanobind('1.4')
-    has_numpy('1.22')
-    has_cmake('3.18')
-    has_poetry('1.5')
-    has_mkdocs('1.4.3')
+    ok = True
+    ok &= has_python('3.9')
+    ok &= has_git('2.35')
+    ok &= has_gh('2.31')
+    ok &= has_bumpversion('1.0')
+    ok &= has_nanobind('1.4')
+    ok &= has_numpy('1.22')
+    ok &= has_cmake('3.18')
+    ok &= has_poetry('1.5')
+    ok &= has_mkdocs('1.4.3')
+
+    msg = "\nAll components are present." if ok else \
+          "\nSome components are missing. This is only a problem is you are planning to use them.\n" \
+          "If you are working on your own machine, you must install these components yourself.\n" \
+          "Otherwise, if you are working on a HPC cluster, you must load the corresponding modules."
 
+    click.secho(msg, fg = fg[ok])
 
-fg = {
-    0: 'red',
-    1: 'green'
-}
 
 def check_version(v: str, minimal: str, message: str):
     ok = Version(v) >= Version(minimal)
     click.secho(f"{message} {'(OK)' if ok else f': {minimal=} (not OK)'}", fg=fg[ok])
+    return ok
 
 def missing(what):
     click.secho(f"{what} is missing in the current environment.", fg =fg[False])
+    return False
 
 def has_python(minimal: str):
     """Python"""
-    check_version(python_version(), minimal=minimal, message='python ' + sys.version.replace('\n',' '))
+    return check_version(python_version(), minimal=minimal, message='python ' + sys.version.replace('\n',' '))
 
 def has_git(minimal: str):
     """git"""
     cmd = 'git'
     try:
         completed_proces = run(f"{cmd} --version", shell=True, capture_output=True)
         s = completed_proces.stdout.decode('utf-8')
         version = s.split(' ')[2]
-        check_version(version, minimal=minimal, message=s.replace('\n',' '))
+        return check_version(version, minimal=minimal, message=s.replace('\n',' '))
     except FileNotFoundError:
-        missing(f"Command {cmd}")
+        return missing(f"Command {cmd}")
 
 def has_gh(minimal: str):
     """git CLI"""
     cmd = 'gh'
     try:
         completed_proces = run(f"{cmd} --version", shell=True, capture_output=True)
         s = completed_proces.stdout.decode('utf-8').replace('\n', ' ')
         version = s.split(' ')[2]
-        check_version(version, minimal=minimal, message=s)
+        return check_version(version, minimal=minimal, message=s)
     except FileNotFoundError:
-        missing(f"Command {cmd}")
+        return missing(f"Command {cmd}")
 
 def has_bumpversion(minimal: str):
     cmd = 'bumpversion'
     try:
         completed_process = run([cmd, '-h'], capture_output=True, )
         lines = completed_process.stdout.decode('utf-8').split('\n')
         for line in lines:
             if 'bumpversion:' in line:
                 v = line.split(' ')[1][1:]
-                check_version(v, minimal=minimal, message=line)
-                break
+                return check_version(v, minimal=minimal, message=line)
+
     except FileNotFoundError:
-        missing(f"Command {cmd}")
+        return missing(f"Command {cmd}")
 
 
 def has_nanobind(minimal: str):
     """"""
     try:
         from nanobind import __version__
-        check_version(__version__, minimal=minimal, message=f"nanobind {__version__}")
+        return check_version(__version__, minimal=minimal, message=f"nanobind {__version__}")
     except ModuleNotFoundError:
-        missing(f"Module nanobind")
+        return missing(f"Module nanobind")
 
 def has_numpy(minimal: str):
     """"""
     try:
         from numpy import __version__
-        check_version(__version__, minimal=minimal, message=f"numpy {__version__}")
+        return check_version(__version__, minimal=minimal, message=f"numpy {__version__}")
     except ModuleNotFoundError:
-        missing(f"Module numpy")
+        return missing(f"Module numpy")
 
 
 def has_cmake(minimal: str):
     """git"""
     cmd = 'cmake'
     try:
         completed_proces = run(f"{cmd} --version", shell=True, capture_output=True)
         s = completed_proces.stdout.decode('utf-8')
         p = s.find('\n')
         s = s[:p]
         version = s.split(' ')[2]
-        check_version(version, minimal=minimal, message=s.replace('\n',' '))
+        return check_version(version, minimal=minimal, message=s.replace('\n',' '))
     except FileNotFoundError:
-        missing(f"Command {cmd}")
+        return missing(f"Command {cmd}")
 
 def has_poetry(minimal: str):
     """"""
     cmd = 'poetry'
     try:
         completed_proces = run(f"{cmd} --version", shell=True, capture_output=True)
         s = completed_proces.stdout.decode('utf-8').replace('\n', ' ')
         version = s.split(' ')[2][:-1]
-        check_version(version, minimal=minimal, message=s.replace('\n',' '))
+        return check_version(version, minimal=minimal, message=s.replace('\n',' '))
     except FileNotFoundError:
-        missing(f"Command {cmd}")
+        return missing(f"Command {cmd}")
 
 def has_mkdocs(minimal: str):
     """"""
     cmd = 'mkdocs'
     try:
         completed_proces = run(f"{cmd} --version", shell=True, capture_output=True)
         s = completed_proces.stdout.decode('utf-8')
         version = s.split(' ')[2]
-        check_version(version, minimal=minimal, message=s.replace('\n',' '))
+        return check_version(version, minimal=minimal, message=s.replace('\n',' '))
     except FileNotFoundError:
-        missing(f"Command {cmd}")
+        return missing(f"Command {cmd}")
```

### Comparing `wiptools-1.2.5.dev0/wiptools/wip/wip_info.py` & `wiptools-1.2.6.dev0/wiptools/wip/wip_info.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/wip/wip_init.py` & `wiptools-1.2.6.dev0/wiptools/wip/wip_init.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/wiptools/wip/wip_remote_repo.py` & `wiptools-1.2.6.dev0/wiptools/wip/wip_remote_repo.py`

 * *Files identical despite different names*

### Comparing `wiptools-1.2.5.dev0/PKG-INFO` & `wiptools-1.2.6.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiptools
-Version: 1.2.5.dev0
+Version: 1.2.6.dev0
 Summary: Python project skeleton and management
 Home-page: https://etijskens.github.io/wiptools
 License: MIT
 Author: Bert Tijskens
 Author-email: engelbert.tijskens@uantwerpen.be
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

