# Comparing `tmp/ewokscore-0.7.0.tar.gz` & `tmp/ewokscore-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewokscore-0.7.0.tar", last modified: Mon Jul  3 08:35:52 2023, max compression
+gzip compressed data, was "dist/ewokscore-0.7.1.tar", last modified: Tue Jul  4 06:52:55 2023, max compression
```

## Comparing `ewokscore-0.7.0.tar` & `ewokscore-0.7.1.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-07-03 08:01:07.000000 ewokscore-0.7.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2664 2023-07-03 08:35:52.000000 ewokscore-0.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1896 2023-07-03 08:01:07.000000 ewokscore-0.7.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-03 08:01:07.000000 ewokscore-0.7.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1540 2023-07-03 08:35:52.000000 ewokscore-0.7.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-03 08:01:07.000000 ewokscore-0.7.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-07-03 08:34:01.000000 ewokscore-0.7.0/src/ewokscore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1721 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/bindings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/cliutils/
--rw-rw-rw-   0 root         (0) root         (0)      738 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/cliutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2997 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/cliutils/cliconvertutils.py
--rw-rw-rw-   0 root         (0) root         (0)     4778 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/cliutils/cliexecuteutils.py
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/cliutils/clilogutils.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/cliutils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/dynamictask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/events/
--rw-rw-rw-   0 root         (0) root         (0)      590 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2826 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/events/contexts.py
--rw-rw-rw-   0 root         (0) root         (0)     4996 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/events/global_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/events/handlers/
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/events/handlers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/events/handlers/base.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/events/handlers/sqlite3.py
--rw-rw-rw-   0 root         (0) root         (0)     1896 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/events/initialize_events.py
--rw-rw-rw-   0 root         (0) root         (0)     8072 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/events/send_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/graph/
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12469 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     1822 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/compare.py
--rw-rw-rw-   0 root         (0) root         (0)     2337 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/error_handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/graph/execute/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 08:35:46.000000 ewokscore-0.7.0/src/ewokscore/graph/execute/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4888 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/execute/sequential.py
--rw-rw-rw-   0 root         (0) root         (0)     7034 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/graph_io.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/multigraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/graph/schema/
--rw-rw-rw-   0 root         (0) root         (0)     4434 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/schema/v0_0.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/schema/v0_1.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/schema/v0_2.py
--rw-rw-rw-   0 root         (0) root         (0)     6803 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/serialize.py
--rw-rw-rw-   0 root         (0) root         (0)    10989 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/subgraph.py
--rw-rw-rw-   0 root         (0) root         (0)     5556 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/taskgraph.py
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/validate.py
--rw-rw-rw-   0 root         (0) root         (0)     8690 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/hashing.py
--rw-rw-rw-   0 root         (0) root         (0)     8893 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/inittask.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/methodtask.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/missing_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1799 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/node.py
--rw-rw-rw-   0 root         (0) root         (0)     2800 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/notebooktask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/persistence/
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/persistence/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1951 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/persistence/atomic.py
--rw-rw-rw-   0 root         (0) root         (0)     5623 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/persistence/file.py
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/persistence/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2328 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/persistence/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     6064 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/persistence/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     3717 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/persistence/uri.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/ppftasks.py
--rw-rw-rw-   0 root         (0) root         (0)     3415 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/registration.py
--rw-rw-rw-   0 root         (0) root         (0)     2960 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/scripttask.py
--rw-rw-rw-   0 root         (0) root         (0)    14409 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/task.py
--rw-rw-rw-   0 root         (0) root         (0)     7274 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/task_discovery.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/taskwithprogress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 08:35:46.000000 ewokscore-0.7.0/src/ewokscore/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/discover_module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 08:35:46.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/
--rw-rw-rw-   0 root         (0) root         (0)      878 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4825 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/acyclic1.py
--rw-rw-rw-   0 root         (0) root         (0)     2447 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/acyclic2.py
--rw-rw-rw-   0 root         (0) root         (0)     3029 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/acyclic3.py
--rw-rw-rw-   0 root         (0) root         (0)     3166 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/cyclic1.py
--rw-rw-rw-   0 root         (0) root         (0)     4139 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/demo.py
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/empty.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/triangle1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/loadtest/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 08:35:46.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/loadtest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/loadtest/graph.json
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/loadtest/subgraph.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 08:35:46.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/addfunc.py
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/condsumtask.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/errorsumtask.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/nooutputtask.py
--rw-rw-rw-   0 root         (0) root         (0)     3072 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/notebooktask.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      159 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/simplemethods.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/sumlist.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/sumtask.py
--rw-rw-rw-   0 root         (0) root         (0)     1671 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_cli_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     7990 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_default_error_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_dynamic_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2223 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_events.py
--rw-rw-rw-   0 root         (0) root         (0)     4897 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_examples.py
--rw-rw-rw-   0 root         (0) root         (0)     7341 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_execute_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     3896 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     6597 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_graph_io.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_graph_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2700 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_graph_serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_graph_start_end_nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     4107 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_hashing.py
--rw-rw-rw-   0 root         (0) root         (0)     7463 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_link_is_required.py
--rw-rw-rw-   0 root         (0) root         (0)     1610 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_method_task.py
--rw-rw-rw-   0 root         (0) root         (0)     1931 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_notebook_task.py
--rw-rw-rw-   0 root         (0) root         (0)     3810 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_persistence.py
--rw-rw-rw-   0 root         (0) root         (0)     3397 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_script_task.py
--rw-rw-rw-   0 root         (0) root         (0)     8223 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_sub_graph.py
--rw-rw-rw-   0 root         (0) root         (0)    10843 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_sub_graph_serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     4985 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_task.py
--rw-rw-rw-   0 root         (0) root         (0)     6101 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_task_discovery.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_task_progress.py
--rw-rw-rw-   0 root         (0) root         (0)     2213 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_uri.py
--rw-rw-rw-   0 root         (0) root         (0)    14406 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_variable.py
--rw-rw-rw-   0 root         (0) root         (0)     2401 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_variable_namespaces.py
--rw-rw-rw-   0 root         (0) root         (0)     7495 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_workflow_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 08:35:46.000000 ewokscore-0.7.0/src/ewokscore/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4916 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/utils/results.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/utils/show.py
--rw-rw-rw-   0 root         (0) root         (0)     1182 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    21421 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/variable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2664 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4341 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      398 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:52:55.000000 ewokscore-0.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-07-04 06:43:50.000000 ewokscore-0.7.1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2664 2023-07-04 06:52:55.000000 ewokscore-0.7.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1896 2023-07-04 06:43:50.000000 ewokscore-0.7.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-04 06:43:50.000000 ewokscore-0.7.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2023-07-04 06:52:55.000000 ewokscore-0.7.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-04 06:43:50.000000 ewokscore-0.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1721 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/bindings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore/cliutils/
+-rw-rw-rw-   0 root         (0) root         (0)      738 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/cliutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/cliutils/cliconvertutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4778 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/cliutils/cliexecuteutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/cliutils/clilogutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/cliutils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/dynamictask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore/events/
+-rw-rw-rw-   0 root         (0) root         (0)      590 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/events/contexts.py
+-rw-rw-rw-   0 root         (0) root         (0)     4996 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/events/global_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore/events/handlers/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/events/handlers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/events/handlers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/events/handlers/sqlite3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1896 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/events/initialize_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     8072 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/events/send_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore/graph/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/graph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12469 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/graph/analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     1822 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/graph/compare.py
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/graph/error_handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore/graph/execute/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 06:52:49.000000 ewokscore-0.7.1/src/ewokscore/graph/execute/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4888 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/graph/execute/sequential.py
+-rw-rw-rw-   0 root         (0) root         (0)     7034 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/graph/graph_io.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/graph/multigraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore/graph/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     4434 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/graph/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/graph/schema/v0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/graph/schema/v0_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/graph/schema/v0_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     6803 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/graph/serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)    10989 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/graph/subgraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     5556 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/graph/taskgraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/graph/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)     8690 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/hashing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8893 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/inittask.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/methodtask.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/missing_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1799 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2800 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/notebooktask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore/persistence/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/persistence/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/persistence/atomic.py
+-rw-rw-rw-   0 root         (0) root         (0)     5623 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/persistence/file.py
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/persistence/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/persistence/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6064 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/persistence/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3717 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/persistence/uri.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/ppftasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3415 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/registration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2960 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/scripttask.py
+-rw-rw-rw-   0 root         (0) root         (0)    14409 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     7274 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/task_discovery.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/taskwithprogress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 06:52:49.000000 ewokscore-0.7.1/src/ewokscore/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/discover_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 06:52:49.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/graphs/
+-rw-rw-rw-   0 root         (0) root         (0)      878 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/graphs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4825 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/graphs/acyclic1.py
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/graphs/acyclic2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3029 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/graphs/acyclic3.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/graphs/cyclic1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4139 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/graphs/demo.py
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/graphs/empty.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/graphs/triangle1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/loadtest/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 06:52:49.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/loadtest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/loadtest/graph.json
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/loadtest/subgraph.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 06:52:49.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/tasks/addfunc.py
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/tasks/condsumtask.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/tasks/errorsumtask.py
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/tasks/nooutputtask.py
+-rw-rw-rw-   0 root         (0) root         (0)     3072 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/tasks/notebooktask.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      159 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/tasks/simplemethods.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/tasks/sumlist.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/examples/tasks/sumtask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_cli_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     7990 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_default_error_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_dynamic_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2223 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     4897 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     7341 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_execute_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     6597 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_graph_io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_graph_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2700 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_graph_serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_graph_start_end_nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4107 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_hashing.py
+-rw-rw-rw-   0 root         (0) root         (0)     7463 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_link_is_required.py
+-rw-rw-rw-   0 root         (0) root         (0)     1610 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_method_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     2197 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_notebook_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     3810 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_persistence.py
+-rw-rw-rw-   0 root         (0) root         (0)     3397 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_script_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     8223 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_sub_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    10843 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_sub_graph_serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     4985 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     6101 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_task_discovery.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_task_progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     2213 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_uri.py
+-rw-rw-rw-   0 root         (0) root         (0)    14406 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_variable.py
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_variable_namespaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     7495 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/test_workflow_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 06:52:49.000000 ewokscore-0.7.1/src/ewokscore/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4916 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/utils/results.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/tests/utils/show.py
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    21421 2023-07-04 06:43:50.000000 ewokscore-0.7.1/src/ewokscore/variable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2664 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4341 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      398 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-04 06:52:55.000000 ewokscore-0.7.1/src/ewokscore.egg-info/top_level.txt
```

### Comparing `ewokscore-0.7.0/LICENSE.md` & `ewokscore-0.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/PKG-INFO` & `ewokscore-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewokscore
-Version: 0.7.0
+Version: 0.7.1
 Summary: API for graphs and tasks in Ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Project-URL: Documentation, https://ewokscore.readthedocs.io/
```

### Comparing `ewokscore-0.7.0/README.md` & `ewokscore-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/setup.cfg` & `ewokscore-0.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/bindings.py` & `ewokscore-0.7.1/src/ewokscore/bindings.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/cliutils/__init__.py` & `ewokscore-0.7.1/src/ewokscore/cliutils/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/cliutils/cliconvertutils.py` & `ewokscore-0.7.1/src/ewokscore/cliutils/cliconvertutils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/cliutils/cliexecuteutils.py` & `ewokscore-0.7.1/src/ewokscore/cliutils/cliexecuteutils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/cliutils/clilogutils.py` & `ewokscore-0.7.1/src/ewokscore/cliutils/clilogutils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/cliutils/utils.py` & `ewokscore-0.7.1/src/ewokscore/cliutils/utils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/dynamictask.py` & `ewokscore-0.7.1/src/ewokscore/dynamictask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/events/__init__.py` & `ewokscore-0.7.1/src/ewokscore/events/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/events/contexts.py` & `ewokscore-0.7.1/src/ewokscore/events/contexts.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/events/global_state.py` & `ewokscore-0.7.1/src/ewokscore/events/global_state.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/events/initialize_events.py` & `ewokscore-0.7.1/src/ewokscore/events/initialize_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/events/send_events.py` & `ewokscore-0.7.1/src/ewokscore/events/send_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/graph/analysis.py` & `ewokscore-0.7.1/src/ewokscore/graph/analysis.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/graph/compare.py` & `ewokscore-0.7.1/src/ewokscore/graph/compare.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/graph/error_handlers.py` & `ewokscore-0.7.1/src/ewokscore/graph/error_handlers.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/graph/execute/sequential.py` & `ewokscore-0.7.1/src/ewokscore/graph/execute/sequential.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/graph/graph_io.py` & `ewokscore-0.7.1/src/ewokscore/graph/graph_io.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/graph/multigraph.py` & `ewokscore-0.7.1/src/ewokscore/graph/multigraph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/graph/schema/__init__.py` & `ewokscore-0.7.1/src/ewokscore/graph/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/graph/serialize.py` & `ewokscore-0.7.1/src/ewokscore/graph/serialize.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/graph/subgraph.py` & `ewokscore-0.7.1/src/ewokscore/graph/subgraph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/graph/taskgraph.py` & `ewokscore-0.7.1/src/ewokscore/graph/taskgraph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/graph/validate.py` & `ewokscore-0.7.1/src/ewokscore/graph/validate.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/hashing.py` & `ewokscore-0.7.1/src/ewokscore/hashing.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/inittask.py` & `ewokscore-0.7.1/src/ewokscore/inittask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/methodtask.py` & `ewokscore-0.7.1/src/ewokscore/methodtask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/missing_data.py` & `ewokscore-0.7.1/src/ewokscore/missing_data.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/node.py` & `ewokscore-0.7.1/src/ewokscore/node.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/notebooktask.py` & `ewokscore-0.7.1/src/ewokscore/notebooktask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/persistence/atomic.py` & `ewokscore-0.7.1/src/ewokscore/persistence/atomic.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/persistence/file.py` & `ewokscore-0.7.1/src/ewokscore/persistence/file.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/persistence/json.py` & `ewokscore-0.7.1/src/ewokscore/persistence/json.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/persistence/nexus.py` & `ewokscore-0.7.1/src/ewokscore/persistence/nexus.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/persistence/proxy.py` & `ewokscore-0.7.1/src/ewokscore/persistence/proxy.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/persistence/uri.py` & `ewokscore-0.7.1/src/ewokscore/persistence/uri.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/ppftasks.py` & `ewokscore-0.7.1/src/ewokscore/ppftasks.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/progress.py` & `ewokscore-0.7.1/src/ewokscore/progress.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/registration.py` & `ewokscore-0.7.1/src/ewokscore/registration.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/scripttask.py` & `ewokscore-0.7.1/src/ewokscore/scripttask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/task.py` & `ewokscore-0.7.1/src/ewokscore/task.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/task_discovery.py` & `ewokscore-0.7.1/src/ewokscore/task_discovery.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/taskwithprogress.py` & `ewokscore-0.7.1/src/ewokscore/taskwithprogress.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/__init__.py` & `ewokscore-0.7.1/src/ewokscore/tests/examples/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/acyclic1.py` & `ewokscore-0.7.1/src/ewokscore/tests/examples/graphs/acyclic1.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/acyclic2.py` & `ewokscore-0.7.1/src/ewokscore/tests/examples/graphs/acyclic2.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/acyclic3.py` & `ewokscore-0.7.1/src/ewokscore/tests/examples/graphs/acyclic3.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/cyclic1.py` & `ewokscore-0.7.1/src/ewokscore/tests/examples/graphs/cyclic1.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/demo.py` & `ewokscore-0.7.1/src/ewokscore/tests/examples/graphs/demo.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/triangle1.py` & `ewokscore-0.7.1/src/ewokscore/tests/examples/graphs/triangle1.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/notebooktask.ipynb` & `ewokscore-0.7.1/src/ewokscore/tests/examples/tasks/notebooktask.ipynb`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/sumlist.py` & `ewokscore-0.7.1/src/ewokscore/tests/examples/tasks/sumlist.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/sumtask.py` & `ewokscore-0.7.1/src/ewokscore/tests/examples/tasks/sumtask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_cli_utils.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_default_error_handlers.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_default_error_handlers.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_dynamic_tasks.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_dynamic_tasks.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_events.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_examples.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_execute_graph.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_execute_graph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_graph.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_graph_io.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_graph_io.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_graph_schema.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_graph_schema.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_graph_serialize.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_graph_serialize.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_graph_start_end_nodes.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_graph_start_end_nodes.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_hashing.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_link_is_required.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_link_is_required.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_method_task.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_method_task.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_notebook_task.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_notebook_task.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import os
+import sys
 import pytest
 from ewokscore.task import Task
 from .examples import tasks
 
 
 @pytest.fixture(scope="module")
 def notebook():
     return os.path.join(tasks.__path__[0], "notebooktask.ipynb")
 
 
+@pytest.mark.xfail(sys.version_info < (3, 8), reason="papermill #711", strict=False)
 def test_notebook_task(notebook, testkernel):
     task = Task.instantiate(
         "NotebookExecutorTask",
         inputs={
             "_notebook": notebook,
             "_kernel_name": testkernel,
             "_execution_timeout": 60,
@@ -26,14 +28,15 @@
     expected = {
         "output_notebook": None,
         "results": {"result": 8, "x": "string", "y": 10, "z": [1, 2, 3]},
     }
     assert task.get_output_values() == expected
 
 
+@pytest.mark.xfail(sys.version_info < (3, 8), reason="papermill #711", strict=False)
 def test_notebook_task_save(tmpdir, notebook, testkernel):
     output_notebook = tmpdir / "nb.ipynb"
     notebook = os.path.join(tasks.__path__[0], "notebooktask.ipynb")
     task = Task.instantiate(
         "NotebookExecutorTask",
         inputs={
             "_notebook": notebook,
@@ -51,14 +54,15 @@
         "output_notebook": str(output_notebook),
         "results": {"result": 8, "x": "string", "y": 10, "z": [1, 2, 3]},
     }
     assert task.get_output_values() == expected
     assert output_notebook.exists()
 
 
+@pytest.mark.xfail(sys.version_info < (3, 8), reason="papermill #711", strict=False)
 def test_notebook_task_failure(notebook, testkernel):
     task = Task.instantiate(
         "NotebookExecutorTask",
         inputs={
             "_notebook": notebook,
             "_kernel_name": testkernel,
             "_execution_timeout": 60,
```

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_persistence.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_persistence.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_script_task.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_script_task.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_sub_graph.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_sub_graph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_sub_graph_serialize.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_sub_graph_serialize.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_task.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_task_discovery.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_task_discovery.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_task_progress.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_task_progress.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_uri.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_uri.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_variable.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_variable_namespaces.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_variable_namespaces.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/test_workflow_events.py` & `ewokscore-0.7.1/src/ewokscore/tests/test_workflow_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/tests/utils/results.py` & `ewokscore-0.7.1/src/ewokscore/tests/utils/results.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/utils.py` & `ewokscore-0.7.1/src/ewokscore/utils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore/variable.py` & `ewokscore-0.7.1/src/ewokscore/variable.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.7.0/src/ewokscore.egg-info/PKG-INFO` & `ewokscore-0.7.1/src/ewokscore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewokscore
-Version: 0.7.0
+Version: 0.7.1
 Summary: API for graphs and tasks in Ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Project-URL: Documentation, https://ewokscore.readthedocs.io/
```

### Comparing `ewokscore-0.7.0/src/ewokscore.egg-info/SOURCES.txt` & `ewokscore-0.7.1/src/ewokscore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

