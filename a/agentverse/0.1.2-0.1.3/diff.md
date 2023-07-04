# Comparing `tmp/agentverse-0.1.2.tar.gz` & `tmp/agentverse-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentverse-0.1.2.tar", last modified: Tue Jul  4 02:05:25 2023, max compression
+gzip compressed data, was "agentverse-0.1.3.tar", last modified: Tue Jul  4 02:13:01 2023, max compression
```

## Comparing `agentverse-0.1.2.tar` & `agentverse-0.1.3.tar`

### file list

```diff
@@ -1,139 +1,147 @@
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.489344 agentverse-0.1.2/
--rw-r--r--   0 weize      (501) staff       (20)    11357 2023-06-29 00:40:08.000000 agentverse-0.1.2/LICENSE
--rw-r--r--   0 weize      (501) staff       (20)       60 2023-07-04 01:57:36.000000 agentverse-0.1.2/MANIFEST.in
--rw-r--r--   0 weize      (501) staff       (20)    19013 2023-07-04 02:05:25.487965 agentverse-0.1.2/PKG-INFO
--rw-r--r--   0 weize      (501) staff       (20)    18474 2023-06-29 00:40:09.000000 agentverse-0.1.2/README.md
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.336606 agentverse-0.1.2/agentverse/
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.359239 agentverse-0.1.2/agentverse/agents/
--rw-r--r--   0 weize      (501) staff       (20)      293 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/agents/__init__.py
--rw-r--r--   0 weize      (501) staff       (20)     2514 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/agents/base.py
--rw-r--r--   0 weize      (501) staff       (20)     3250 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/agents/conversation_agent.py
--rw-r--r--   0 weize      (501) staff       (20)     5701 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/agents/prisoner_dilemma_agent.py
--rw-r--r--   0 weize      (501) staff       (20)     6921 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/agents/tool_agent.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.367174 agentverse-0.1.2/agentverse/agentverse.egg-info/
--rw-r--r--   0 weize      (501) staff       (20)    19013 2023-07-04 02:05:25.000000 agentverse-0.1.2/agentverse/agentverse.egg-info/PKG-INFO
--rw-r--r--   0 weize      (501) staff       (20)     4927 2023-07-04 02:05:25.000000 agentverse-0.1.2/agentverse/agentverse.egg-info/SOURCES.txt
--rw-r--r--   0 weize      (501) staff       (20)        1 2023-07-04 02:05:25.000000 agentverse-0.1.2/agentverse/agentverse.egg-info/dependency_links.txt
--rw-r--r--   0 weize      (501) staff       (20)      103 2023-07-04 02:05:25.000000 agentverse-0.1.2/agentverse/agentverse.egg-info/requires.txt
--rw-r--r--   0 weize      (501) staff       (20)       38 2023-07-04 02:05:25.000000 agentverse-0.1.2/agentverse/agentverse.egg-info/top_level.txt
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.377473 agentverse-0.1.2/agentverse/environments/
--rw-r--r--   0 weize      (501) staff       (20)      390 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/__init__.py
--rw-r--r--   0 weize      (501) staff       (20)     1204 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/base.py
--rw-r--r--   0 weize      (501) staff       (20)     3023 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/basic.py
--rw-r--r--   0 weize      (501) staff       (20)     7639 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/pokemon.py
--rw-r--r--   0 weize      (501) staff       (20)     1458 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/prisoner_dilemma.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.380606 agentverse-0.1.2/agentverse/environments/rules/
--rw-r--r--   0 weize      (501) staff       (20)       22 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/__init__.py
--rw-r--r--   0 weize      (501) staff       (20)     3124 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/base.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.388709 agentverse-0.1.2/agentverse/environments/rules/describer/
--rw-r--r--   0 weize      (501) staff       (20)      285 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/describer/__init__.py
--rw-r--r--   0 weize      (501) staff       (20)      556 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/describer/base.py
--rw-r--r--   0 weize      (501) staff       (20)      520 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/describer/basic.py
--rw-r--r--   0 weize      (501) staff       (20)     1410 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/describer/classroom.py
--rw-r--r--   0 weize      (501) staff       (20)     2219 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/describer/pokemon.py
--rw-r--r--   0 weize      (501) staff       (20)     1630 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/describer/prisoner.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.398613 agentverse-0.1.2/agentverse/environments/rules/order/
--rw-r--r--   0 weize      (501) staff       (20)      396 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/order/__init__.py
--rw-r--r--   0 weize      (501) staff       (20)      446 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/order/base.py
--rw-r--r--   0 weize      (501) staff       (20)     4592 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/order/classroom.py
--rw-r--r--   0 weize      (501) staff       (20)      479 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/order/concurrent.py
--rw-r--r--   0 weize      (501) staff       (20)     1828 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/order/prisoner.py
--rw-r--r--   0 weize      (501) staff       (20)      536 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/order/random.py
--rw-r--r--   0 weize      (501) staff       (20)      835 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/order/sde_team.py
--rw-r--r--   0 weize      (501) staff       (20)     1003 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/order/sde_team_given_tests.py
--rw-r--r--   0 weize      (501) staff       (20)      763 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/order/sequential.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.409157 agentverse-0.1.2/agentverse/environments/rules/selector/
--rw-r--r--   0 weize      (501) staff       (20)      337 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/selector/__init__.py
--rw-r--r--   0 weize      (501) staff       (20)      680 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/selector/base.py
--rw-r--r--   0 weize      (501) staff       (20)      644 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/selector/basic.py
--rw-r--r--   0 weize      (501) staff       (20)     1797 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/selector/classroom.py
--rw-r--r--   0 weize      (501) staff       (20)     3294 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/selector/code_api.py
--rw-r--r--   0 weize      (501) staff       (20)     4310 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/selector/pokemon.py
--rw-r--r--   0 weize      (501) staff       (20)     2692 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/selector/sde_team.py
--rw-r--r--   0 weize      (501) staff       (20)     1855 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/selector/sde_team_given_tests.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.418235 agentverse-0.1.2/agentverse/environments/rules/updater/
--rw-r--r--   0 weize      (501) staff       (20)      270 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/updater/__init__.py
--rw-r--r--   0 weize      (501) staff       (20)      557 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/updater/base.py
--rw-r--r--   0 weize      (501) staff       (20)     2469 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/updater/basic.py
--rw-r--r--   0 weize      (501) staff       (20)     1299 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/updater/classroom.py
--rw-r--r--   0 weize      (501) staff       (20)     1614 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/updater/pokemon.py
--rw-r--r--   0 weize      (501) staff       (20)     1723 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/updater/sde_team.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.427266 agentverse-0.1.2/agentverse/environments/rules/visibility/
--rw-r--r--   0 weize      (501) staff       (20)      392 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/visibility/__init__.py
--rw-r--r--   0 weize      (501) staff       (20)      452 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/visibility/all.py
--rw-r--r--   0 weize      (501) staff       (20)      430 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/visibility/base.py
--rw-r--r--   0 weize      (501) staff       (20)     3512 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/visibility/classroom.py
--rw-r--r--   0 weize      (501) staff       (20)      533 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/visibility/oneself.py
--rw-r--r--   0 weize      (501) staff       (20)      863 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/visibility/pokemon.py
--rw-r--r--   0 weize      (501) staff       (20)     1597 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/visibility/prisoner.py
--rw-r--r--   0 weize      (501) staff       (20)      562 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/rules/visibility/sde_team.py
--rw-r--r--   0 weize      (501) staff       (20)     4411 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/sde_team.py
--rw-r--r--   0 weize      (501) staff       (20)     4640 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/environments/sde_team_given_tests.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.430847 agentverse-0.1.2/agentverse/llms/
--rw-r--r--   0 weize      (501) staff       (20)      209 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/llms/__init__.py
--rw-r--r--   0 weize      (501) staff       (20)      646 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/llms/base.py
--rw-r--r--   0 weize      (501) staff       (20)     4583 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/llms/openai.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.438445 agentverse-0.1.2/agentverse/memory/
--rw-r--r--   0 weize      (501) staff       (20)      237 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/memory/__init__.py
--rw-r--r--   0 weize      (501) staff       (20)      393 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/memory/base.py
--rw-r--r--   0 weize      (501) staff       (20)      936 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/memory/chat_history.py
--rw-r--r--   0 weize      (501) staff       (20)     1169 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/memory/sde_team.py
--rw-r--r--   0 weize      (501) staff       (20)     3166 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/memory/summary.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.440223 agentverse-0.1.2/agentverse/tasks/
--rw-r--r--   0 weize      (501) staff       (20)      759 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/__init__.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.441815 agentverse-0.1.2/agentverse/tasks/__pycache__/
--rw-r--r--   0 weize      (501) staff       (20)     1023 2023-07-03 09:14:53.000000 agentverse-0.1.2/agentverse/tasks/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.445575 agentverse-0.1.2/agentverse/tasks/db_diag/
--rw-r--r--   0 weize      (501) staff       (20)      948 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/db_diag/README.md
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.446872 agentverse-0.1.2/agentverse/tasks/db_diag/__pycache__/
--rw-r--r--   0 weize      (501) staff       (20)     1451 2023-07-03 09:14:54.000000 agentverse-0.1.2/agentverse/tasks/db_diag/__pycache__/output_parser.cpython-310.pyc
--rw-r--r--   0 weize      (501) staff       (20)    10134 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/db_diag/config.yaml
--rw-r--r--   0 weize      (501) staff       (20)     1577 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/db_diag/output_parser.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.449790 agentverse-0.1.2/agentverse/tasks/math_problem_2players_tools/
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.451423 agentverse-0.1.2/agentverse/tasks/math_problem_2players_tools/__pycache__/
--rw-r--r--   0 weize      (501) staff       (20)     1379 2023-07-03 09:14:53.000000 agentverse-0.1.2/agentverse/tasks/math_problem_2players_tools/__pycache__/output_parser.cpython-310.pyc
--rw-r--r--   0 weize      (501) staff       (20)     3681 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/math_problem_2players_tools/config.yaml
--rw-r--r--   0 weize      (501) staff       (20)     1267 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/math_problem_2players_tools/output_parser.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.453352 agentverse-0.1.2/agentverse/tasks/nlp_classroom_3players/
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.454100 agentverse-0.1.2/agentverse/tasks/nlp_classroom_3players/__pycache__/
--rw-r--r--   0 weize      (501) staff       (20)     1292 2023-07-03 09:14:54.000000 agentverse-0.1.2/agentverse/tasks/nlp_classroom_3players/__pycache__/output_parser.cpython-310.pyc
--rw-r--r--   0 weize      (501) staff       (20)     2216 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/nlp_classroom_3players/config.yaml
--rw-r--r--   0 weize      (501) staff       (20)     1128 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/nlp_classroom_3players/output_parser.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.457183 agentverse-0.1.2/agentverse/tasks/nlp_classroom_3players_withtool/
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.458288 agentverse-0.1.2/agentverse/tasks/nlp_classroom_3players_withtool/__pycache__/
--rw-r--r--   0 weize      (501) staff       (20)     1555 2023-07-03 09:14:54.000000 agentverse-0.1.2/agentverse/tasks/nlp_classroom_3players_withtool/__pycache__/output_parser.cpython-310.pyc
--rw-r--r--   0 weize      (501) staff       (20)     8358 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/nlp_classroom_3players_withtool/config.yaml
--rw-r--r--   0 weize      (501) staff       (20)     1573 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/nlp_classroom_3players_withtool/output_parser.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.460726 agentverse-0.1.2/agentverse/tasks/nlp_classroom_9players/
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.461830 agentverse-0.1.2/agentverse/tasks/nlp_classroom_9players/__pycache__/
--rw-r--r--   0 weize      (501) staff       (20)     1458 2023-07-03 09:14:54.000000 agentverse-0.1.2/agentverse/tasks/nlp_classroom_9players/__pycache__/output_parser.cpython-310.pyc
--rw-r--r--   0 weize      (501) staff       (20)     9037 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/nlp_classroom_9players/config.yaml
--rw-r--r--   0 weize      (501) staff       (20)     1454 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/nlp_classroom_9players/output_parser.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.464338 agentverse-0.1.2/agentverse/tasks/nlp_classroom_9players_group/
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.465867 agentverse-0.1.2/agentverse/tasks/nlp_classroom_9players_group/__pycache__/
--rw-r--r--   0 weize      (501) staff       (20)     1456 2023-07-03 09:14:54.000000 agentverse-0.1.2/agentverse/tasks/nlp_classroom_9players_group/__pycache__/output_parser.cpython-310.pyc
--rw-r--r--   0 weize      (501) staff       (20)    10096 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/nlp_classroom_9players_group/config.yaml
--rw-r--r--   0 weize      (501) staff       (20)     1382 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/nlp_classroom_9players_group/output_parser.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.468862 agentverse-0.1.2/agentverse/tasks/pokemon/
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.470341 agentverse-0.1.2/agentverse/tasks/pokemon/__pycache__/
--rw-r--r--   0 weize      (501) staff       (20)     1365 2023-07-03 09:14:54.000000 agentverse-0.1.2/agentverse/tasks/pokemon/__pycache__/output_parser.cpython-310.pyc
--rw-r--r--   0 weize      (501) staff       (20)    13707 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/pokemon/config.yaml
--rw-r--r--   0 weize      (501) staff       (20)     1331 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/pokemon/output_parser.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.473247 agentverse-0.1.2/agentverse/tasks/prisoner_dilemma/
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.474597 agentverse-0.1.2/agentverse/tasks/prisoner_dilemma/__pycache__/
--rw-r--r--   0 weize      (501) staff       (20)     1979 2023-07-03 09:14:54.000000 agentverse-0.1.2/agentverse/tasks/prisoner_dilemma/__pycache__/output_parser.cpython-310.pyc
--rw-r--r--   0 weize      (501) staff       (20)     4509 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/prisoner_dilemma/config.yaml
--rw-r--r--   0 weize      (501) staff       (20)     3832 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/prisoner_dilemma/output_parser.py
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.475595 agentverse-0.1.2/agentverse/tasks/sde_team/
--rw-r--r--   0 weize      (501) staff       (20)     4742 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/sde_team/readme.md
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.481301 agentverse-0.1.2/agentverse/tasks/sde_team/sde_team_2players/
--rw-r--r--   0 weize      (501) staff       (20)      593 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/sde_team/sde_team_2players/build_config.py
--rw-r--r--   0 weize      (501) staff       (20)      962 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/sde_team/sde_team_2players/code_problem.json
--rw-r--r--   0 weize      (501) staff       (20)    14010 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/sde_team/sde_team_2players/config.yaml
--rw-r--r--   0 weize      (501) staff       (20)      705 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/sde_team/sde_team_2players/output_parser.py
--rw-r--r--   0 weize      (501) staff       (20)     6714 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/sde_team/sde_team_2players/partial_config.yaml
-drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:05:25.486405 agentverse-0.1.2/agentverse/tasks/sde_team/sde_team_3players/
--rw-r--r--   0 weize      (501) staff       (20)     8515 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/sde_team/sde_team_3players/config.yaml
--rw-r--r--   0 weize      (501) staff       (20)      696 2023-06-29 00:40:10.000000 agentverse-0.1.2/agentverse/tasks/sde_team/sde_team_3players/output_parser.py
--rw-r--r--   0 weize      (501) staff       (20)       38 2023-07-04 02:05:25.489666 agentverse-0.1.2/setup.cfg
--rw-r--r--   0 weize      (501) staff       (20)     1265 2023-07-04 02:05:15.000000 agentverse-0.1.2/setup.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.100720 agentverse-0.1.3/
+-rw-r--r--   0 weize      (501) staff       (20)    11357 2023-06-29 00:40:08.000000 agentverse-0.1.3/LICENSE
+-rw-r--r--   0 weize      (501) staff       (20)       60 2023-07-04 01:57:36.000000 agentverse-0.1.3/MANIFEST.in
+-rw-r--r--   0 weize      (501) staff       (20)    19013 2023-07-04 02:13:01.099918 agentverse-0.1.3/PKG-INFO
+-rw-r--r--   0 weize      (501) staff       (20)    18474 2023-06-29 00:40:09.000000 agentverse-0.1.3/README.md
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:00.988629 agentverse-0.1.3/agentverse/
+-rw-r--r--   0 weize      (501) staff       (20)      596 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/__init__.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:00.997210 agentverse-0.1.3/agentverse/agents/
+-rw-r--r--   0 weize      (501) staff       (20)      293 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/agents/__init__.py
+-rw-r--r--   0 weize      (501) staff       (20)     2514 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/agents/base.py
+-rw-r--r--   0 weize      (501) staff       (20)     3250 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/agents/conversation_agent.py
+-rw-r--r--   0 weize      (501) staff       (20)     5701 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/agents/prisoner_dilemma_agent.py
+-rw-r--r--   0 weize      (501) staff       (20)     6921 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/agents/tool_agent.py
+-rw-r--r--   0 weize      (501) staff       (20)     2183 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/agentverse.py
+-rw-r--r--   0 weize      (501) staff       (20)    20978 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/demo.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.006657 agentverse-0.1.3/agentverse/environments/
+-rw-r--r--   0 weize      (501) staff       (20)      390 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/__init__.py
+-rw-r--r--   0 weize      (501) staff       (20)     1204 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/base.py
+-rw-r--r--   0 weize      (501) staff       (20)     3023 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/basic.py
+-rw-r--r--   0 weize      (501) staff       (20)     7639 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/pokemon.py
+-rw-r--r--   0 weize      (501) staff       (20)     1458 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/prisoner_dilemma.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.010353 agentverse-0.1.3/agentverse/environments/rules/
+-rw-r--r--   0 weize      (501) staff       (20)       22 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/__init__.py
+-rw-r--r--   0 weize      (501) staff       (20)     3124 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/base.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.018018 agentverse-0.1.3/agentverse/environments/rules/describer/
+-rw-r--r--   0 weize      (501) staff       (20)      285 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/describer/__init__.py
+-rw-r--r--   0 weize      (501) staff       (20)      556 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/describer/base.py
+-rw-r--r--   0 weize      (501) staff       (20)      520 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/describer/basic.py
+-rw-r--r--   0 weize      (501) staff       (20)     1410 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/describer/classroom.py
+-rw-r--r--   0 weize      (501) staff       (20)     2219 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/describer/pokemon.py
+-rw-r--r--   0 weize      (501) staff       (20)     1630 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/describer/prisoner.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.028836 agentverse-0.1.3/agentverse/environments/rules/order/
+-rw-r--r--   0 weize      (501) staff       (20)      396 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/order/__init__.py
+-rw-r--r--   0 weize      (501) staff       (20)      446 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/order/base.py
+-rw-r--r--   0 weize      (501) staff       (20)     4592 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/order/classroom.py
+-rw-r--r--   0 weize      (501) staff       (20)      479 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/order/concurrent.py
+-rw-r--r--   0 weize      (501) staff       (20)     1828 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/order/prisoner.py
+-rw-r--r--   0 weize      (501) staff       (20)      536 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/order/random.py
+-rw-r--r--   0 weize      (501) staff       (20)      835 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/order/sde_team.py
+-rw-r--r--   0 weize      (501) staff       (20)     1003 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/order/sde_team_given_tests.py
+-rw-r--r--   0 weize      (501) staff       (20)      763 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/order/sequential.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.036145 agentverse-0.1.3/agentverse/environments/rules/selector/
+-rw-r--r--   0 weize      (501) staff       (20)      337 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/selector/__init__.py
+-rw-r--r--   0 weize      (501) staff       (20)      680 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/selector/base.py
+-rw-r--r--   0 weize      (501) staff       (20)      644 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/selector/basic.py
+-rw-r--r--   0 weize      (501) staff       (20)     1797 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/selector/classroom.py
+-rw-r--r--   0 weize      (501) staff       (20)     3294 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/selector/code_api.py
+-rw-r--r--   0 weize      (501) staff       (20)     4310 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/selector/pokemon.py
+-rw-r--r--   0 weize      (501) staff       (20)     2692 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/selector/sde_team.py
+-rw-r--r--   0 weize      (501) staff       (20)     1855 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/selector/sde_team_given_tests.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.041432 agentverse-0.1.3/agentverse/environments/rules/updater/
+-rw-r--r--   0 weize      (501) staff       (20)      270 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/updater/__init__.py
+-rw-r--r--   0 weize      (501) staff       (20)      557 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/updater/base.py
+-rw-r--r--   0 weize      (501) staff       (20)     2469 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/updater/basic.py
+-rw-r--r--   0 weize      (501) staff       (20)     1299 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/updater/classroom.py
+-rw-r--r--   0 weize      (501) staff       (20)     1614 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/updater/pokemon.py
+-rw-r--r--   0 weize      (501) staff       (20)     1723 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/updater/sde_team.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.047879 agentverse-0.1.3/agentverse/environments/rules/visibility/
+-rw-r--r--   0 weize      (501) staff       (20)      392 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/visibility/__init__.py
+-rw-r--r--   0 weize      (501) staff       (20)      452 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/visibility/all.py
+-rw-r--r--   0 weize      (501) staff       (20)      430 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/visibility/base.py
+-rw-r--r--   0 weize      (501) staff       (20)     3512 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/visibility/classroom.py
+-rw-r--r--   0 weize      (501) staff       (20)      533 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/visibility/oneself.py
+-rw-r--r--   0 weize      (501) staff       (20)      863 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/visibility/pokemon.py
+-rw-r--r--   0 weize      (501) staff       (20)     1597 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/visibility/prisoner.py
+-rw-r--r--   0 weize      (501) staff       (20)      562 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/rules/visibility/sde_team.py
+-rw-r--r--   0 weize      (501) staff       (20)     4411 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/sde_team.py
+-rw-r--r--   0 weize      (501) staff       (20)     4640 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/environments/sde_team_given_tests.py
+-rw-r--r--   0 weize      (501) staff       (20)     3484 2023-07-04 00:56:47.000000 agentverse-0.1.3/agentverse/initialization.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.051171 agentverse-0.1.3/agentverse/llms/
+-rw-r--r--   0 weize      (501) staff       (20)      209 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/llms/__init__.py
+-rw-r--r--   0 weize      (501) staff       (20)      646 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/llms/base.py
+-rw-r--r--   0 weize      (501) staff       (20)     4583 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/llms/openai.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.058606 agentverse-0.1.3/agentverse/memory/
+-rw-r--r--   0 weize      (501) staff       (20)      237 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/memory/__init__.py
+-rw-r--r--   0 weize      (501) staff       (20)      393 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/memory/base.py
+-rw-r--r--   0 weize      (501) staff       (20)      936 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/memory/chat_history.py
+-rw-r--r--   0 weize      (501) staff       (20)     1169 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/memory/sde_team.py
+-rw-r--r--   0 weize      (501) staff       (20)     3166 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/memory/summary.py
+-rw-r--r--   0 weize      (501) staff       (20)      339 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/message.py
+-rw-r--r--   0 weize      (501) staff       (20)      672 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/parser.py
+-rw-r--r--   0 weize      (501) staff       (20)      712 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/registry.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.059898 agentverse-0.1.3/agentverse/tasks/
+-rw-r--r--   0 weize      (501) staff       (20)      759 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/__init__.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.061182 agentverse-0.1.3/agentverse/tasks/__pycache__/
+-rw-r--r--   0 weize      (501) staff       (20)     1023 2023-07-03 09:14:53.000000 agentverse-0.1.3/agentverse/tasks/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.064621 agentverse-0.1.3/agentverse/tasks/db_diag/
+-rw-r--r--   0 weize      (501) staff       (20)      948 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/db_diag/README.md
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.066439 agentverse-0.1.3/agentverse/tasks/db_diag/__pycache__/
+-rw-r--r--   0 weize      (501) staff       (20)     1451 2023-07-03 09:14:54.000000 agentverse-0.1.3/agentverse/tasks/db_diag/__pycache__/output_parser.cpython-310.pyc
+-rw-r--r--   0 weize      (501) staff       (20)    10134 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/db_diag/config.yaml
+-rw-r--r--   0 weize      (501) staff       (20)     1577 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/db_diag/output_parser.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.068795 agentverse-0.1.3/agentverse/tasks/math_problem_2players_tools/
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.070106 agentverse-0.1.3/agentverse/tasks/math_problem_2players_tools/__pycache__/
+-rw-r--r--   0 weize      (501) staff       (20)     1379 2023-07-03 09:14:53.000000 agentverse-0.1.3/agentverse/tasks/math_problem_2players_tools/__pycache__/output_parser.cpython-310.pyc
+-rw-r--r--   0 weize      (501) staff       (20)     3681 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/math_problem_2players_tools/config.yaml
+-rw-r--r--   0 weize      (501) staff       (20)     1267 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/math_problem_2players_tools/output_parser.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.072860 agentverse-0.1.3/agentverse/tasks/nlp_classroom_3players/
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.074462 agentverse-0.1.3/agentverse/tasks/nlp_classroom_3players/__pycache__/
+-rw-r--r--   0 weize      (501) staff       (20)     1292 2023-07-03 09:14:54.000000 agentverse-0.1.3/agentverse/tasks/nlp_classroom_3players/__pycache__/output_parser.cpython-310.pyc
+-rw-r--r--   0 weize      (501) staff       (20)     2216 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/nlp_classroom_3players/config.yaml
+-rw-r--r--   0 weize      (501) staff       (20)     1128 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/nlp_classroom_3players/output_parser.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.076515 agentverse-0.1.3/agentverse/tasks/nlp_classroom_3players_withtool/
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.077659 agentverse-0.1.3/agentverse/tasks/nlp_classroom_3players_withtool/__pycache__/
+-rw-r--r--   0 weize      (501) staff       (20)     1555 2023-07-03 09:14:54.000000 agentverse-0.1.3/agentverse/tasks/nlp_classroom_3players_withtool/__pycache__/output_parser.cpython-310.pyc
+-rw-r--r--   0 weize      (501) staff       (20)     8358 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/nlp_classroom_3players_withtool/config.yaml
+-rw-r--r--   0 weize      (501) staff       (20)     1573 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/nlp_classroom_3players_withtool/output_parser.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.079878 agentverse-0.1.3/agentverse/tasks/nlp_classroom_9players/
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.080739 agentverse-0.1.3/agentverse/tasks/nlp_classroom_9players/__pycache__/
+-rw-r--r--   0 weize      (501) staff       (20)     1458 2023-07-03 09:14:54.000000 agentverse-0.1.3/agentverse/tasks/nlp_classroom_9players/__pycache__/output_parser.cpython-310.pyc
+-rw-r--r--   0 weize      (501) staff       (20)     9037 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/nlp_classroom_9players/config.yaml
+-rw-r--r--   0 weize      (501) staff       (20)     1454 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/nlp_classroom_9players/output_parser.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.083280 agentverse-0.1.3/agentverse/tasks/nlp_classroom_9players_group/
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.084137 agentverse-0.1.3/agentverse/tasks/nlp_classroom_9players_group/__pycache__/
+-rw-r--r--   0 weize      (501) staff       (20)     1456 2023-07-03 09:14:54.000000 agentverse-0.1.3/agentverse/tasks/nlp_classroom_9players_group/__pycache__/output_parser.cpython-310.pyc
+-rw-r--r--   0 weize      (501) staff       (20)    10096 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/nlp_classroom_9players_group/config.yaml
+-rw-r--r--   0 weize      (501) staff       (20)     1382 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/nlp_classroom_9players_group/output_parser.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.086238 agentverse-0.1.3/agentverse/tasks/pokemon/
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.087248 agentverse-0.1.3/agentverse/tasks/pokemon/__pycache__/
+-rw-r--r--   0 weize      (501) staff       (20)     1365 2023-07-03 09:14:54.000000 agentverse-0.1.3/agentverse/tasks/pokemon/__pycache__/output_parser.cpython-310.pyc
+-rw-r--r--   0 weize      (501) staff       (20)    13707 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/pokemon/config.yaml
+-rw-r--r--   0 weize      (501) staff       (20)     1331 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/pokemon/output_parser.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.089550 agentverse-0.1.3/agentverse/tasks/prisoner_dilemma/
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.091107 agentverse-0.1.3/agentverse/tasks/prisoner_dilemma/__pycache__/
+-rw-r--r--   0 weize      (501) staff       (20)     1979 2023-07-03 09:14:54.000000 agentverse-0.1.3/agentverse/tasks/prisoner_dilemma/__pycache__/output_parser.cpython-310.pyc
+-rw-r--r--   0 weize      (501) staff       (20)     4509 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/prisoner_dilemma/config.yaml
+-rw-r--r--   0 weize      (501) staff       (20)     3832 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/prisoner_dilemma/output_parser.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.091993 agentverse-0.1.3/agentverse/tasks/sde_team/
+-rw-r--r--   0 weize      (501) staff       (20)     4742 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/sde_team/readme.md
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.096628 agentverse-0.1.3/agentverse/tasks/sde_team/sde_team_2players/
+-rw-r--r--   0 weize      (501) staff       (20)      593 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/sde_team/sde_team_2players/build_config.py
+-rw-r--r--   0 weize      (501) staff       (20)      962 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/sde_team/sde_team_2players/code_problem.json
+-rw-r--r--   0 weize      (501) staff       (20)    14010 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/sde_team/sde_team_2players/config.yaml
+-rw-r--r--   0 weize      (501) staff       (20)      705 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/sde_team/sde_team_2players/output_parser.py
+-rw-r--r--   0 weize      (501) staff       (20)     6714 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/sde_team/sde_team_2players/partial_config.yaml
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:01.098454 agentverse-0.1.3/agentverse/tasks/sde_team/sde_team_3players/
+-rw-r--r--   0 weize      (501) staff       (20)     8515 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/sde_team/sde_team_3players/config.yaml
+-rw-r--r--   0 weize      (501) staff       (20)      696 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/tasks/sde_team/sde_team_3players/output_parser.py
+-rw-r--r--   0 weize      (501) staff       (20)      268 2023-06-29 00:40:10.000000 agentverse-0.1.3/agentverse/utils.py
+drwxr-xr-x   0 weize      (501) staff       (20)        0 2023-07-04 02:13:00.992713 agentverse-0.1.3/agentverse.egg-info/
+-rw-r--r--   0 weize      (501) staff       (20)    19013 2023-07-04 02:13:00.000000 agentverse-0.1.3/agentverse.egg-info/PKG-INFO
+-rw-r--r--   0 weize      (501) staff       (20)     5054 2023-07-04 02:13:00.000000 agentverse-0.1.3/agentverse.egg-info/SOURCES.txt
+-rw-r--r--   0 weize      (501) staff       (20)        1 2023-07-04 02:13:00.000000 agentverse-0.1.3/agentverse.egg-info/dependency_links.txt
+-rw-r--r--   0 weize      (501) staff       (20)      103 2023-07-04 02:13:00.000000 agentverse-0.1.3/agentverse.egg-info/requires.txt
+-rw-r--r--   0 weize      (501) staff       (20)       11 2023-07-04 02:13:00.000000 agentverse-0.1.3/agentverse.egg-info/top_level.txt
+-rw-r--r--   0 weize      (501) staff       (20)       38 2023-07-04 02:13:01.100984 agentverse-0.1.3/setup.cfg
+-rw-r--r--   0 weize      (501) staff       (20)     1211 2023-07-04 02:12:37.000000 agentverse-0.1.3/setup.py
```

### Comparing `agentverse-0.1.2/LICENSE` & `agentverse-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/PKG-INFO` & `agentverse-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentverse
-Version: 0.1.2
+Version: 0.1.3
 Summary: A versatile framework that streamlines the process of creating custom multi-agent environments for large language models (LLMs).
 Home-page: https://github.com/OpenBMB/AgentVerse
 Author: OpenBMB
 Author-email: chenweize1998@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agentverse Version: 0.1.2 Summary: A versatile
+Metadata-Version: 2.1 Name: agentverse Version: 0.1.3 Summary: A versatile
 framework that streamlines the process of creating custom multi-agent
 environments for large language models (LLMs). Home-page: https://github.com/
 OpenBMB/AgentVerse Author: OpenBMB Author-email: chenweize1998@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agentverse-0.1.2/README.md` & `agentverse-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/agents/base.py` & `agentverse-0.1.3/agentverse/agents/base.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/agents/conversation_agent.py` & `agentverse-0.1.3/agentverse/agents/conversation_agent.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/agents/prisoner_dilemma_agent.py` & `agentverse-0.1.3/agentverse/agents/prisoner_dilemma_agent.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/agents/tool_agent.py` & `agentverse-0.1.3/agentverse/agents/tool_agent.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/agentverse.egg-info/PKG-INFO` & `agentverse-0.1.3/agentverse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentverse
-Version: 0.1.2
+Version: 0.1.3
 Summary: A versatile framework that streamlines the process of creating custom multi-agent environments for large language models (LLMs).
 Home-page: https://github.com/OpenBMB/AgentVerse
 Author: OpenBMB
 Author-email: chenweize1998@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agentverse Version: 0.1.2 Summary: A versatile
+Metadata-Version: 2.1 Name: agentverse Version: 0.1.3 Summary: A versatile
 framework that streamlines the process of creating custom multi-agent
 environments for large language models (LLMs). Home-page: https://github.com/
 OpenBMB/AgentVerse Author: OpenBMB Author-email: chenweize1998@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agentverse-0.1.2/agentverse/agentverse.egg-info/SOURCES.txt` & `agentverse-0.1.3/agentverse.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+agentverse/__init__.py
+agentverse/agentverse.py
+agentverse/demo.py
+agentverse/initialization.py
+agentverse/message.py
+agentverse/parser.py
+agentverse/registry.py
+agentverse/utils.py
+agentverse.egg-info/PKG-INFO
+agentverse.egg-info/SOURCES.txt
+agentverse.egg-info/dependency_links.txt
+agentverse.egg-info/requires.txt
+agentverse.egg-info/top_level.txt
 agentverse/agents/__init__.py
 agentverse/agents/base.py
 agentverse/agents/conversation_agent.py
 agentverse/agents/prisoner_dilemma_agent.py
 agentverse/agents/tool_agent.py
-agentverse/agentverse.egg-info/PKG-INFO
-agentverse/agentverse.egg-info/SOURCES.txt
-agentverse/agentverse.egg-info/dependency_links.txt
-agentverse/agentverse.egg-info/requires.txt
-agentverse/agentverse.egg-info/top_level.txt
 agentverse/environments/__init__.py
 agentverse/environments/base.py
 agentverse/environments/basic.py
 agentverse/environments/pokemon.py
 agentverse/environments/prisoner_dilemma.py
 agentverse/environments/sde_team.py
 agentverse/environments/sde_team_given_tests.py
```

### Comparing `agentverse-0.1.2/agentverse/environments/base.py` & `agentverse-0.1.3/agentverse/environments/base.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/basic.py` & `agentverse-0.1.3/agentverse/environments/basic.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/pokemon.py` & `agentverse-0.1.3/agentverse/environments/pokemon.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/prisoner_dilemma.py` & `agentverse-0.1.3/agentverse/environments/prisoner_dilemma.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/base.py` & `agentverse-0.1.3/agentverse/environments/rules/base.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/describer/base.py` & `agentverse-0.1.3/agentverse/environments/rules/describer/base.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/describer/basic.py` & `agentverse-0.1.3/agentverse/environments/rules/describer/basic.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/describer/classroom.py` & `agentverse-0.1.3/agentverse/environments/rules/describer/classroom.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/describer/pokemon.py` & `agentverse-0.1.3/agentverse/environments/rules/describer/pokemon.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/describer/prisoner.py` & `agentverse-0.1.3/agentverse/environments/rules/describer/prisoner.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/order/classroom.py` & `agentverse-0.1.3/agentverse/environments/rules/order/classroom.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/order/prisoner.py` & `agentverse-0.1.3/agentverse/environments/rules/order/prisoner.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/order/random.py` & `agentverse-0.1.3/agentverse/environments/rules/order/random.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/order/sde_team.py` & `agentverse-0.1.3/agentverse/environments/rules/order/sde_team.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/order/sde_team_given_tests.py` & `agentverse-0.1.3/agentverse/environments/rules/order/sde_team_given_tests.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/order/sequential.py` & `agentverse-0.1.3/agentverse/environments/rules/order/sequential.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/selector/base.py` & `agentverse-0.1.3/agentverse/environments/rules/selector/base.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/selector/basic.py` & `agentverse-0.1.3/agentverse/environments/rules/selector/basic.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/selector/classroom.py` & `agentverse-0.1.3/agentverse/environments/rules/selector/classroom.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/selector/code_api.py` & `agentverse-0.1.3/agentverse/environments/rules/selector/code_api.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/selector/pokemon.py` & `agentverse-0.1.3/agentverse/environments/rules/selector/pokemon.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/selector/sde_team.py` & `agentverse-0.1.3/agentverse/environments/rules/selector/sde_team.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/selector/sde_team_given_tests.py` & `agentverse-0.1.3/agentverse/environments/rules/selector/sde_team_given_tests.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/updater/base.py` & `agentverse-0.1.3/agentverse/environments/rules/updater/base.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/updater/basic.py` & `agentverse-0.1.3/agentverse/environments/rules/updater/basic.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/updater/classroom.py` & `agentverse-0.1.3/agentverse/environments/rules/updater/classroom.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/updater/pokemon.py` & `agentverse-0.1.3/agentverse/environments/rules/updater/pokemon.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/updater/sde_team.py` & `agentverse-0.1.3/agentverse/environments/rules/updater/sde_team.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/visibility/classroom.py` & `agentverse-0.1.3/agentverse/environments/rules/visibility/classroom.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/visibility/oneself.py` & `agentverse-0.1.3/agentverse/environments/rules/visibility/oneself.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/visibility/pokemon.py` & `agentverse-0.1.3/agentverse/environments/rules/visibility/pokemon.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/visibility/prisoner.py` & `agentverse-0.1.3/agentverse/environments/rules/visibility/prisoner.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/rules/visibility/sde_team.py` & `agentverse-0.1.3/agentverse/environments/rules/visibility/sde_team.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/sde_team.py` & `agentverse-0.1.3/agentverse/environments/sde_team.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/environments/sde_team_given_tests.py` & `agentverse-0.1.3/agentverse/environments/sde_team_given_tests.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/llms/base.py` & `agentverse-0.1.3/agentverse/llms/base.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/llms/openai.py` & `agentverse-0.1.3/agentverse/llms/openai.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/memory/chat_history.py` & `agentverse-0.1.3/agentverse/memory/chat_history.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/memory/sde_team.py` & `agentverse-0.1.3/agentverse/memory/sde_team.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/memory/summary.py` & `agentverse-0.1.3/agentverse/memory/summary.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/__init__.py` & `agentverse-0.1.3/agentverse/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/__pycache__/__init__.cpython-310.pyc` & `agentverse-0.1.3/agentverse/tasks/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/db_diag/README.md` & `agentverse-0.1.3/agentverse/tasks/db_diag/README.md`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/db_diag/__pycache__/output_parser.cpython-310.pyc` & `agentverse-0.1.3/agentverse/tasks/db_diag/__pycache__/output_parser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/db_diag/config.yaml` & `agentverse-0.1.3/agentverse/tasks/db_diag/config.yaml`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/db_diag/output_parser.py` & `agentverse-0.1.3/agentverse/tasks/db_diag/output_parser.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/math_problem_2players_tools/__pycache__/output_parser.cpython-310.pyc` & `agentverse-0.1.3/agentverse/tasks/math_problem_2players_tools/__pycache__/output_parser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/math_problem_2players_tools/config.yaml` & `agentverse-0.1.3/agentverse/tasks/math_problem_2players_tools/config.yaml`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/math_problem_2players_tools/output_parser.py` & `agentverse-0.1.3/agentverse/tasks/math_problem_2players_tools/output_parser.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/nlp_classroom_3players/__pycache__/output_parser.cpython-310.pyc` & `agentverse-0.1.3/agentverse/tasks/nlp_classroom_3players/__pycache__/output_parser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/nlp_classroom_3players/config.yaml` & `agentverse-0.1.3/agentverse/tasks/nlp_classroom_3players/config.yaml`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/nlp_classroom_3players/output_parser.py` & `agentverse-0.1.3/agentverse/tasks/nlp_classroom_3players/output_parser.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/nlp_classroom_3players_withtool/__pycache__/output_parser.cpython-310.pyc` & `agentverse-0.1.3/agentverse/tasks/nlp_classroom_3players_withtool/__pycache__/output_parser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/nlp_classroom_3players_withtool/config.yaml` & `agentverse-0.1.3/agentverse/tasks/nlp_classroom_3players_withtool/config.yaml`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/nlp_classroom_3players_withtool/output_parser.py` & `agentverse-0.1.3/agentverse/tasks/nlp_classroom_3players_withtool/output_parser.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/nlp_classroom_9players/__pycache__/output_parser.cpython-310.pyc` & `agentverse-0.1.3/agentverse/tasks/nlp_classroom_9players/__pycache__/output_parser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/nlp_classroom_9players/config.yaml` & `agentverse-0.1.3/agentverse/tasks/nlp_classroom_9players/config.yaml`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/nlp_classroom_9players/output_parser.py` & `agentverse-0.1.3/agentverse/tasks/nlp_classroom_9players/output_parser.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/nlp_classroom_9players_group/__pycache__/output_parser.cpython-310.pyc` & `agentverse-0.1.3/agentverse/tasks/nlp_classroom_9players_group/__pycache__/output_parser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/nlp_classroom_9players_group/config.yaml` & `agentverse-0.1.3/agentverse/tasks/nlp_classroom_9players_group/config.yaml`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/nlp_classroom_9players_group/output_parser.py` & `agentverse-0.1.3/agentverse/tasks/nlp_classroom_9players_group/output_parser.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/pokemon/__pycache__/output_parser.cpython-310.pyc` & `agentverse-0.1.3/agentverse/tasks/pokemon/__pycache__/output_parser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/pokemon/config.yaml` & `agentverse-0.1.3/agentverse/tasks/pokemon/config.yaml`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/pokemon/output_parser.py` & `agentverse-0.1.3/agentverse/tasks/pokemon/output_parser.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/prisoner_dilemma/__pycache__/output_parser.cpython-310.pyc` & `agentverse-0.1.3/agentverse/tasks/prisoner_dilemma/__pycache__/output_parser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/prisoner_dilemma/config.yaml` & `agentverse-0.1.3/agentverse/tasks/prisoner_dilemma/config.yaml`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/prisoner_dilemma/output_parser.py` & `agentverse-0.1.3/agentverse/tasks/prisoner_dilemma/output_parser.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/sde_team/readme.md` & `agentverse-0.1.3/agentverse/tasks/sde_team/readme.md`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/sde_team/sde_team_2players/build_config.py` & `agentverse-0.1.3/agentverse/tasks/sde_team/sde_team_2players/build_config.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/sde_team/sde_team_2players/code_problem.json` & `agentverse-0.1.3/agentverse/tasks/sde_team/sde_team_2players/code_problem.json`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/sde_team/sde_team_2players/config.yaml` & `agentverse-0.1.3/agentverse/tasks/sde_team/sde_team_2players/config.yaml`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/sde_team/sde_team_2players/output_parser.py` & `agentverse-0.1.3/agentverse/tasks/sde_team/sde_team_2players/output_parser.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/sde_team/sde_team_2players/partial_config.yaml` & `agentverse-0.1.3/agentverse/tasks/sde_team/sde_team_2players/partial_config.yaml`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/sde_team/sde_team_3players/config.yaml` & `agentverse-0.1.3/agentverse/tasks/sde_team/sde_team_3players/config.yaml`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/agentverse/tasks/sde_team/sde_team_3players/output_parser.py` & `agentverse-0.1.3/agentverse/tasks/sde_team/sde_team_3players/output_parser.py`

 * *Files identical despite different names*

### Comparing `agentverse-0.1.2/setup.py` & `agentverse-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 #     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="agentverse",
-    version="0.1.2",
+    version="0.1.3",
     author="OpenBMB",
     author_email="chenweize1998@gmail.com",
     description="A versatile framework that streamlines the process of creating custom multi-agent environments for large language models (LLMs).",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OpenBMB/AgentVerse",
-    packages=setuptools.find_packages(where="agentverse"),
-    package_dir={"": "agentverse"},
+    packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         'License :: OSI Approved :: Apache Software License',
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9",
     install_requires=[
```

