# Comparing `tmp/mindflow-0.5.5.tar.gz` & `tmp/mindflow-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindflow-0.5.5.tar", last modified: Mon Jul  3 03:03:30 2023, max compression
+gzip compressed data, was "mindflow-0.6.0.tar", last modified: Tue Jul  4 14:47:18 2023, max compression
```

## Comparing `mindflow-0.5.5.tar` & `mindflow-0.6.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:30.436972 mindflow-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-03 03:03:18.000000 mindflow-0.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-03 03:03:18.000000 mindflow-0.5.5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 03:03:18.000000 mindflow-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-03 03:03:18.000000 mindflow-0.5.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-07-03 03:03:30.436972 mindflow-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-07-03 03:03:18.000000 mindflow-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-03 03:03:18.000000 mindflow-0.5.5/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:30.412972 mindflow-0.5.5/mindflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:30.416972 mindflow-0.5.5/mindflow/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:30.420972 mindflow-0.5.5/mindflow/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/commands/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/commands/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:30.420972 mindflow-0.5.5/mindflow/cli/commands/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/commands/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/commands/git/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/commands/git/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/commands/git/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/commands/git/mr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/commands/git/pr.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/commands/git/push.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/commands/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/cli/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:30.424972 mindflow-0.5.5/mindflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:30.424972 mindflow-0.5.5/mindflow/core/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/commands/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/commands/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:30.428972 mindflow-0.5.5/mindflow/core/commands/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/commands/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/commands/git/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/commands/git/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/commands/git/pr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/commands/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/commands/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:30.428972 mindflow-0.5.5/mindflow/core/file_processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/file_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/file_processing/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/file_processing/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/prompt_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:30.428972 mindflow-0.5.5/mindflow/core/resolving/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/resolving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/resolving/resolve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:30.428972 mindflow-0.5.5/mindflow/core/resolving/resolvers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/resolving/resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/resolving/resolvers/document_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/resolving/resolvers/file_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:30.428972 mindflow-0.5.5/mindflow/core/text_processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/text_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/text_processing/utf8.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/text_processing/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/token_counting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:30.432972 mindflow-0.5.5/mindflow/core/types/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/types/conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:30.436972 mindflow-0.5.5/mindflow/core/types/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/types/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/types/definitions/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/types/definitions/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/types/definitions/mind_flow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/types/definitions/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/types/definitions/model_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/types/definitions/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/types/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/types/mindflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18846 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/types/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/types/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:30.436972 mindflow-0.5.5/mindflow/core/types/store_traits/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/types/store_traits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/types/store_traits/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/types/store_traits/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/core/types/store_traits/static.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:30.436972 mindflow-0.5.5/mindflow/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/unit_tests/dummy_diff.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/unit_tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-07-03 03:03:18.000000 mindflow-0.5.5/mindflow/unit_tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:03:30.416972 mindflow-0.5.5/mindflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-07-03 03:03:30.000000 mindflow-0.5.5/mindflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-03 03:03:30.000000 mindflow-0.5.5/mindflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 03:03:30.000000 mindflow-0.5.5/mindflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-03 03:03:30.000000 mindflow-0.5.5/mindflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-03 03:03:30.000000 mindflow-0.5.5/mindflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 03:03:30.000000 mindflow-0.5.5/mindflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-03 03:03:18.000000 mindflow-0.5.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 03:03:30.436972 mindflow-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-03 03:03:18.000000 mindflow-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:18.304366 mindflow-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-04 14:47:07.000000 mindflow-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-04 14:47:07.000000 mindflow-0.6.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 14:47:07.000000 mindflow-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-04 14:47:07.000000 mindflow-0.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-07-04 14:47:18.304366 mindflow-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-07-04 14:47:07.000000 mindflow-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-04 14:47:07.000000 mindflow-0.6.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:18.292366 mindflow-0.6.0/mindflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:18.292366 mindflow-0.6.0/mindflow/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:18.292366 mindflow-0.6.0/mindflow/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/commands/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/commands/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:18.296366 mindflow-0.6.0/mindflow/cli/commands/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/commands/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/commands/git/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/commands/git/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/commands/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/commands/git/mr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/commands/git/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/commands/git/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/commands/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/cli/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:18.296366 mindflow-0.6.0/mindflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:18.296366 mindflow-0.6.0/mindflow/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/commands/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/commands/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:18.300366 mindflow-0.6.0/mindflow/core/commands/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/commands/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/commands/git/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/commands/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/commands/git/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/commands/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/commands/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:18.300366 mindflow-0.6.0/mindflow/core/file_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/file_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/file_processing/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/file_processing/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/prompt_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:18.300366 mindflow-0.6.0/mindflow/core/resolving/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/resolving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/resolving/resolve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:18.300366 mindflow-0.6.0/mindflow/core/resolving/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/resolving/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/resolving/resolvers/document_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/resolving/resolvers/file_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:18.300366 mindflow-0.6.0/mindflow/core/text_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/text_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/text_processing/utf8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/text_processing/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/token_counting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:18.300366 mindflow-0.6.0/mindflow/core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/types/conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:18.300366 mindflow-0.6.0/mindflow/core/types/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/types/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/types/definitions/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/types/definitions/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/types/definitions/mind_flow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/types/definitions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/types/definitions/model_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/types/definitions/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/types/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/types/mindflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/types/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/types/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:18.304366 mindflow-0.6.0/mindflow/core/types/store_traits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/types/store_traits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/types/store_traits/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/types/store_traits/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/core/types/store_traits/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:18.304366 mindflow-0.6.0/mindflow/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/unit_tests/dummy_diff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/unit_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-07-04 14:47:07.000000 mindflow-0.6.0/mindflow/unit_tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:47:18.292366 mindflow-0.6.0/mindflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-07-04 14:47:18.000000 mindflow-0.6.0/mindflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-04 14:47:18.000000 mindflow-0.6.0/mindflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:47:18.000000 mindflow-0.6.0/mindflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-04 14:47:18.000000 mindflow-0.6.0/mindflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 14:47:18.000000 mindflow-0.6.0/mindflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 14:47:18.000000 mindflow-0.6.0/mindflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 14:47:07.000000 mindflow-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 14:47:18.304366 mindflow-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-04 14:47:07.000000 mindflow-0.6.0/setup.py
```

### Comparing `mindflow-0.5.5/.gitignore` & `mindflow-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/Makefile` & `mindflow-0.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/PKG-INFO` & `mindflow-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindflow
-Version: 0.5.5
+Version: 0.6.0
 Summary: AI-powered search engine for your code!
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # :brain: mindflow :ocean:
 The [ChatGPT](https://openai.com/blog/chatgpt)-powered swiss army knife for the modern developer! We provide an AI-powered CLI git wrapper, boilerplate code generator, code search engine, a conversation history manager, and much more!
 
@@ -15,24 +15,27 @@
 - [Code Generator](#code-generator)
 - [Managing Chat History](#chat-history)
 - [Git Diff Summaries](#git-diff-summaries)
 - [Automatic Git Commits](#automatic-git-commits)
 - [Automatic Pull Requests](#automatic-pull-requests)
 - [Use-case showcase](#showcase)
 
+## Demo
+[![Alternate Text](http://img.youtube.com/vi/e2bedjyv-Nw/0.jpg)](https://www.youtube.com/watch?v=e2bedjyv-Nw)
+
 ## Join Our Community!
 1. Follow us on [Twitter](https://twitter.com/mindflow_ai)
 2. Join our [discord](https://discord.com/invite/P2cQACzB)
 3. BONUS: Consider [becoming a patron](https://www.patreon.com/MindFlowAI) :heart:
 
 ## Getting Started
 
 Pre-requisite: 
 - You'll need to create an [OpenAI](https://openai.com/blog/openai-api) account.
-- Also, create a [Pinecone](https://www.pinecone.io/start) account to use their vector database.
+- Also, create a [Pinecone](https://www.pinecone.io/start) account to use their vector database if you would like to use the `chat with documents` feature.
 
 1. Run `pip install mindflow`, or you can clone this repo and run `pip install -e path/to/mindflow`.
 2. Run `mf login`:
     - Register with OpenAI to use their models. You can find your OpenAI API key [here](https://platform.openai.com/account/api-keys).
     - Register with Pinecone to use their vector database. You can find your Pinecone API key and Environment [here](https://www.pinecone.io/start).
 3. Now, you're ready to start using MindFlow!
```

### Comparing `mindflow-0.5.5/README.md` & `mindflow-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,27 @@
 - [Code Generator](#code-generator)
 - [Managing Chat History](#chat-history)
 - [Git Diff Summaries](#git-diff-summaries)
 - [Automatic Git Commits](#automatic-git-commits)
 - [Automatic Pull Requests](#automatic-pull-requests)
 - [Use-case showcase](#showcase)
 
+## Demo
+[![Alternate Text](http://img.youtube.com/vi/e2bedjyv-Nw/0.jpg)](https://www.youtube.com/watch?v=e2bedjyv-Nw)
+
 ## Join Our Community!
 1. Follow us on [Twitter](https://twitter.com/mindflow_ai)
 2. Join our [discord](https://discord.com/invite/P2cQACzB)
 3. BONUS: Consider [becoming a patron](https://www.patreon.com/MindFlowAI) :heart:
 
 ## Getting Started
 
 Pre-requisite: 
 - You'll need to create an [OpenAI](https://openai.com/blog/openai-api) account.
-- Also, create a [Pinecone](https://www.pinecone.io/start) account to use their vector database.
+- Also, create a [Pinecone](https://www.pinecone.io/start) account to use their vector database if you would like to use the `chat with documents` feature.
 
 1. Run `pip install mindflow`, or you can clone this repo and run `pip install -e path/to/mindflow`.
 2. Run `mf login`:
     - Register with OpenAI to use their models. You can find your OpenAI API key [here](https://platform.openai.com/account/api-keys).
     - Register with Pinecone to use their vector database. You can find your Pinecone API key and Environment [here](https://www.pinecone.io/start).
 3. Now, you're ready to start using MindFlow!
```

### Comparing `mindflow-0.5.5/mindflow/cli/cli_main.py` & `mindflow-0.6.0/mindflow/cli/cli_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 from mindflow.cli.commands.delete import delete
 from mindflow.cli.commands.index import index
 from mindflow.cli.commands.inspect import inspect
 from mindflow.cli.commands.login import login
 from mindflow.cli.commands.gen import gen
 from mindflow.cli.commands.config import config
 
-# from mindflow.cli.new_click_cli.commands.config import config
-
 
 @click.group()
 def mindflow_cli():
     pass
 
 
 @mindflow_cli.command()
```

### Comparing `mindflow-0.5.5/mindflow/cli/commands/chat.py` & `mindflow-0.6.0/mindflow/cli/commands/chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,33 +37,35 @@
     async def stream_chat(settings: Settings, prompt: str):
         click.echo(colored("\nGPT:", attrs=["bold"]))
         async for char_stream_chunk in run_chat(settings, [], prompt):
             if isinstance(char_stream_chunk, Ok):
                 click.echo(char_stream_chunk.value, nl=False)
             else:
                 click.echo(char_stream_chunk.value)
+        print("\n")
 
     async def stream_query(settings: Settings, file_paths: List[str], prompt: str):
         click.echo(colored("\nGPT:", attrs=["bold"]))
         async for char_stream_chunk in run_query(settings, file_paths, prompt):
             if isinstance(char_stream_chunk, Ok):
                 click.echo(char_stream_chunk.value, nl=False)
             else:
                 click.echo(char_stream_chunk.value)
+        print("\n")
 
     prompt, paths = parse_chat_prompt_and_paths_from_args(prompt_args)
     settings = Settings()
     if paths:
         if skip_index:
             click.echo(
-                "Skipping indexing step, only using the current index for context. You can run `mf index` to pre-index specific paths."
+                colored("Skipping indexing step, only using the current index for context. You can run `mf index` to pre-index specific paths.", "yellow")
             )
         else:
             click.echo(
-                "Indexing paths... Note: this may take a while, if you want to skip this step, use the `--skip-index` flag. If you do so, you can pre-select specific paths to index with `mf index`.\n"
+                colored("Indexing paths... Note: this may take a while, especially the first time. If it fails, or gets stuck, retry and it will pick up where you left off. If you want to skip this step, use the `--skip-index` flag. If you do so, you can pre-select specific paths to index with `mf index`.\n", "yellow")
             )
 
             asyncio.run(run_index(settings, paths))
 
         asyncio.run(stream_query(settings, paths, prompt))
 
         save_json_store()
```

### Comparing `mindflow-0.5.5/mindflow/cli/commands/config.py` & `mindflow-0.6.0/mindflow/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/cli/commands/delete.py` & `mindflow-0.6.0/mindflow/cli/commands/delete.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/cli/commands/gen.py` & `mindflow-0.6.0/mindflow/cli/commands/gen.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/cli/commands/git/commit.py` & `mindflow-0.6.0/mindflow/cli/commands/git/commit.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,20 @@
     help="Don't use mindflow to generate a commit message, use this one instead.",
     default=None,
 )
 def commit(args: Tuple[str], message: Optional[str] = None):
     import asyncio
 
     from result import Err, Result
+    from termcolor import colored
 
     from mindflow.cli.util import execute_command_without_trace
     from mindflow.core.commands.git.commit import create_gpt_commit_message
     from mindflow.core.settings import Settings
     from mindflow.core.types.model import ModelApiCallError
-    from termcolor import colored
 
     if message is not None:
         click.echo(
             colored(
                 f"Warning: Using message '{message}' instead of mindflow generated message.",
                 "yellow",
             )
```

### Comparing `mindflow-0.5.5/mindflow/cli/commands/git/diff.py` & `mindflow-0.6.0/mindflow/cli/commands/git/diff.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import click
 from typing import Tuple
-
 from mindflow.cli.util import passthrough_command
 
 
 @passthrough_command(
     help="Wrapper around git diff that summarizes the output. Treat this command exactly like git diff, it supports all arguments that git diff provides."
 )
 @click.option("--detailed", type=bool, default=False, is_flag=True)
 def diff(args: Tuple[str], detailed: bool):
     import asyncio
 
+    from termcolor import colored
+    from result import Ok
+
     from mindflow.core.commands.git.diff import create_gpt_summarized_diff
     from mindflow.cli.util import execute_command_without_trace
     from mindflow.core.settings import Settings
-    from termcolor import colored
-    from result import Ok
 
     diff_output = execute_command_without_trace(["git", "diff"] + list(args)).strip()
     if not diff_output:
         click.echo("No diff output to summarize.")
         return
 
     if not detailed:
@@ -35,9 +35,10 @@
         async for char_stream_chunk in create_gpt_summarized_diff(
             settings, diff_output, detailed=detailed
         ):
             if isinstance(char_stream_chunk, Ok):
                 click.echo(char_stream_chunk.value, nl=False)
             else:
                 click.echo(char_stream_chunk.value)
+        print("\n")
 
     asyncio.run(stream_diff(Settings(), diff_output, detailed=detailed))
```

### Comparing `mindflow-0.5.5/mindflow/cli/commands/git/mr.py` & `mindflow-0.6.0/mindflow/cli/commands/git/mr.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/cli/commands/git/pr.py` & `mindflow-0.6.0/mindflow/cli/commands/git/pr.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/cli/commands/inspect.py` & `mindflow-0.6.0/mindflow/cli/commands/inspect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import click
-
 from typing import List
 
 
 @click.command(help="Inspect your MindFlow index")
 @click.argument("document_paths", type=str, nargs=-1)
 def inspect(document_paths: List[str]):
     import asyncio
```

### Comparing `mindflow-0.5.5/mindflow/cli/commands/login.py` & `mindflow-0.6.0/mindflow/cli/commands/login.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mindflow.core.types.store_traits.json import save_json_store
 
     service_ids = [
         ServiceConfigID.OPENAI.value,
         ServiceConfigID.PINECONE.value,
     ]
     service_options = [
-        ServiceConfig.load(service_id, False) for service_id in service_ids
+        ServiceConfig.load(service_id) if ServiceConfig.load(service_id) is not None else ServiceConfig(service_id) for service_id in service_ids
     ]
     service_descriptions = ["OpenAI", "Pinecone: (Vector DB)"]
     service_config: ServiceConfig = select_option(
         "Choose service to configure. Enter #",
         service_options,
         service_descriptions,
     )
```

### Comparing `mindflow-0.5.5/mindflow/cli/util.py` & `mindflow-0.6.0/mindflow/cli/util.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/commands/chat.py` & `mindflow-0.6.0/mindflow/core/commands/chat.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/commands/delete.py` & `mindflow-0.6.0/mindflow/core/commands/delete.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/commands/gen.py` & `mindflow-0.6.0/mindflow/core/commands/gen.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/commands/git/commit.py` & `mindflow-0.6.0/mindflow/core/commands/git/commit.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/commands/git/diff.py` & `mindflow-0.6.0/mindflow/core/commands/git/diff.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/commands/git/pr.py` & `mindflow-0.6.0/mindflow/core/commands/git/pr.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/commands/index.py` & `mindflow-0.6.0/mindflow/core/commands/index.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/commands/inspect.py` & `mindflow-0.6.0/mindflow/core/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/commands/query.py` & `mindflow-0.6.0/mindflow/core/commands/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     while left <= right:
         mid = (left + right) // 2
         if (
             get_token_count_of_text_for_model(
                 configured_model.tokenizer, query + selected_content[:mid]
             )
             <= configured_model.model.hard_token_limit
-            - MinimumReservedLength.QUERY.value
+            - 800
         ):
             left = mid + 1
             continue
         right = mid - 1
 
     return selected_content[:right]
```

### Comparing `mindflow-0.5.5/mindflow/core/file_processing/extract.py` & `mindflow-0.6.0/mindflow/core/file_processing/extract.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/file_processing/git.py` & `mindflow-0.6.0/mindflow/core/file_processing/git.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/prompt_builders.py` & `mindflow-0.6.0/mindflow/core/prompt_builders.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import json
-import anthropic  # type: ignore
 
 from enum import Enum
-from typing import Dict, Union, List
+from typing import Dict, List
 
 from mindflow.core.types.model import ConfiguredModel
-from mindflow.core.types.definitions.service import ServiceID
-from mindflow.core.constants import MinimumReservedLength
 from mindflow.core.token_counting import get_token_count_of_text_for_model
 
 
 class Role(Enum):
     SYSTEM = "system"
     USER = "user"
     ASSISTANT = "assistant"
```

### Comparing `mindflow-0.5.5/mindflow/core/prompts.py` & `mindflow-0.6.0/mindflow/core/prompts.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/resolving/resolve.py` & `mindflow-0.6.0/mindflow/core/resolving/resolve.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module for resolving documents types."""
 import sys
 
 from typing import List
-from mindflow.core.types.document import DocumentReference
 
+from mindflow.core.types.document import DocumentReference
 from mindflow.core.resolving.resolvers.file_resolver import FileResolver
 
 
 def resolve_path_to_document_reference(
     document_path: str,
 ) -> List[DocumentReference]:
     resolvers = [FileResolver()]
```

### Comparing `mindflow-0.5.5/mindflow/core/resolving/resolvers/file_resolver.py` & `mindflow-0.6.0/mindflow/core/resolving/resolvers/file_resolver.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/token_counting.py` & `mindflow-0.6.0/mindflow/core/token_counting.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/types/definitions/mind_flow_model.py` & `mindflow-0.6.0/mindflow/core/types/definitions/mind_flow_model.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/types/definitions/model.py` & `mindflow-0.6.0/mindflow/core/types/definitions/model.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/types/definitions/service.py` & `mindflow-0.6.0/mindflow/core/types/definitions/service.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/types/document.py` & `mindflow-0.6.0/mindflow/core/types/document.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/types/mindflow_model.py` & `mindflow-0.6.0/mindflow/core/types/mindflow_model.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/types/model.py` & `mindflow-0.6.0/mindflow/core/types/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import sys
 import time
 import aiohttp
 import logging
 import asyncio
 import tiktoken
 
 from abc import ABC, abstractmethod
@@ -185,16 +186,22 @@
             self.config = ModelConfig(
                 {
                     "id": f"{model_id}_config",
                     "soft_token_limit": self.model.default_soft_token_limit,
                 }
             )
 
-        if service_config := ServiceConfig.load(f"{self.model.service}_config"):
-            self.api_key = service_config.api_key
+        service_config = ServiceConfig.load(f"{self.model.service}_config")
+        if service_config == None or not hasattr(service_config, "api_key"):
+            print(
+                f"No {self.model.service} API key found. Please set {self.model.service} API key with `mf login`."
+            )
+            sys.exit(1)
+        
+        self.api_key = service_config.api_key
 
         self.headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
         }
         self.status_tracker = ModelStatusTracker(
             self.model.max_requests_per_minute, self.model.max_tokens_per_minute
@@ -395,15 +402,14 @@
                                 result = json.loads(lines[-1][5:])  # remove "data: "
                             except Exception as e:
                                 return
                             if "error" not in result:
                                 await self.status_tracker.increment_requests_count_successful()
                                 await self.status_tracker.decrement_requests_count_in_progress()
                                 if not result["choices"][0]["delta"]:
-                                    print("No delta")
                                     continue
                                 yield Ok(
                                     result["choices"][0]["delta"]["content"]
                                 )  # Yield the result
                             else:
                                 logging.warning(
                                     f"Request {payload} failed with error {result['error']}"
```

### Comparing `mindflow-0.5.5/mindflow/core/types/service.py` & `mindflow-0.6.0/mindflow/core/types/service.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/types/store_traits/json.py` & `mindflow-0.6.0/mindflow/core/types/store_traits/json.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/types/store_traits/pinecone.py` & `mindflow-0.6.0/mindflow/core/types/store_traits/pinecone.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/core/types/store_traits/static.py` & `mindflow-0.6.0/mindflow/core/types/store_traits/static.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/unit_tests/dummy_diff.txt` & `mindflow-0.6.0/mindflow/unit_tests/dummy_diff.txt`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow/unit_tests/test_utils.py` & `mindflow-0.6.0/mindflow/unit_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/mindflow.egg-info/PKG-INFO` & `mindflow-0.6.0/mindflow.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindflow
-Version: 0.5.5
+Version: 0.6.0
 Summary: AI-powered search engine for your code!
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # :brain: mindflow :ocean:
 The [ChatGPT](https://openai.com/blog/chatgpt)-powered swiss army knife for the modern developer! We provide an AI-powered CLI git wrapper, boilerplate code generator, code search engine, a conversation history manager, and much more!
 
@@ -15,24 +15,27 @@
 - [Code Generator](#code-generator)
 - [Managing Chat History](#chat-history)
 - [Git Diff Summaries](#git-diff-summaries)
 - [Automatic Git Commits](#automatic-git-commits)
 - [Automatic Pull Requests](#automatic-pull-requests)
 - [Use-case showcase](#showcase)
 
+## Demo
+[![Alternate Text](http://img.youtube.com/vi/e2bedjyv-Nw/0.jpg)](https://www.youtube.com/watch?v=e2bedjyv-Nw)
+
 ## Join Our Community!
 1. Follow us on [Twitter](https://twitter.com/mindflow_ai)
 2. Join our [discord](https://discord.com/invite/P2cQACzB)
 3. BONUS: Consider [becoming a patron](https://www.patreon.com/MindFlowAI) :heart:
 
 ## Getting Started
 
 Pre-requisite: 
 - You'll need to create an [OpenAI](https://openai.com/blog/openai-api) account.
-- Also, create a [Pinecone](https://www.pinecone.io/start) account to use their vector database.
+- Also, create a [Pinecone](https://www.pinecone.io/start) account to use their vector database if you would like to use the `chat with documents` feature.
 
 1. Run `pip install mindflow`, or you can clone this repo and run `pip install -e path/to/mindflow`.
 2. Run `mf login`:
     - Register with OpenAI to use their models. You can find your OpenAI API key [here](https://platform.openai.com/account/api-keys).
     - Register with Pinecone to use their vector database. You can find your Pinecone API key and Environment [here](https://www.pinecone.io/start).
 3. Now, you're ready to start using MindFlow!
```

### Comparing `mindflow-0.5.5/mindflow.egg-info/SOURCES.txt` & `mindflow-0.6.0/mindflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.5/setup.py` & `mindflow-0.6.0/setup.py`

 * *Files identical despite different names*

