# Comparing `tmp/inmanta-core-8.5.0.tar.gz` & `tmp/inmanta-core-9.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inmanta-core-8.5.0.tar", last modified: Tue Jul  4 12:54:32 2023, max compression
+gzip compressed data, was "inmanta-core-9.3.0.tar", last modified: Tue Jul  4 11:30:06 2023, max compression
```

## Comparing `inmanta-core-8.5.0.tar` & `inmanta-core-9.3.0.tar`

### file list

```diff
@@ -1,257 +1,258 @@
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.751522 inmanta-core-8.5.0/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    10174 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/LICENSE
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      311 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/MANIFEST.in
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3195 2023-07-04 12:54:32.751522 inmanta-core-8.5.0/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2238 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/README.md
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.723521 inmanta-core-8.5.0/misc/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       31 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/misc/extensions.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      402 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/misc/inmanta-agent.service
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      333 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/misc/inmanta-server.service
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     8762 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/misc/inmanta-workon-register.sh
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2906 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/misc/inmanta.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    12162 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/misc/inmanta.lang
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1256 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/misc/inmanta.vim
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      141 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/misc/logrotation_config
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1432 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/pyproject.toml
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      918 2023-07-04 12:54:32.752522 inmanta-core-8.5.0/setup.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3416 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/setup.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.721521 inmanta-core-8.5.0/src/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.727521 inmanta-core-8.5.0/src/inmanta/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      914 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/__init__.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.728521 inmanta-core-8.5.0/src/inmanta/agent/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      738 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/agent/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    59119 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/agent/agent.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    10115 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/agent/cache.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5149 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/agent/config.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    43603 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/agent/handler.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.728521 inmanta-core-8.5.0/src/inmanta/agent/io/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2815 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/agent/io/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    19884 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/agent/io/local.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6362 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/agent/io/remote.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3395 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/agent/reporting.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    28443 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/app.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.729521 inmanta-core-8.5.0/src/inmanta/ast/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    32500 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/ast/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7103 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/ast/attribute.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6354 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/ast/blocks.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.729521 inmanta-core-8.5.0/src/inmanta/ast/constraint/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/ast/constraint/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    17182 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/ast/constraint/expression.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    19266 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/ast/entity.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2783 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/ast/export.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.730521 inmanta-core-8.5.0/src/inmanta/ast/statements/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    23361 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/ast/statements/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    23834 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/ast/statements/assign.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    12314 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/ast/statements/call.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    24146 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/ast/statements/define.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    55960 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/ast/statements/generator.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    20775 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/ast/type.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    12524 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/ast/variables.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3400 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/command.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.730521 inmanta-core-8.5.0/src/inmanta/compiler/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    14509 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/compiler/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1963 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/compiler/config.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1110 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/compiler/data.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.730521 inmanta-core-8.5.0/src/inmanta/compiler/help/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/compiler/help/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     8327 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/compiler/help/explainer.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.731521 inmanta-core-8.5.0/src/inmanta/compiler/help/templates/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      235 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/compiler/help/templates/index_collision.j2
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3604 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/compiler/help/templates/modified_after_freeze.j2
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      733 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/compiler/help/templates/module_v2_in_v1_path.j2
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    20756 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/config.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     9233 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/const.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.732521 inmanta-core-8.5.0/src/inmanta/data/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)   247603 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/data/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    46598 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/data/dataview.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    22068 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/data/model.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    12206 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/data/schema.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.732521 inmanta-core-8.5.0/src/inmanta/db/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     8702 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/util.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.736521 inmanta-core-8.5.0/src/inmanta/db/versions/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    12123 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v1.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1737 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v17.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1393 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v2.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2443 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202105170.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      915 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202106080.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1247 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202106210.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1826 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202109100.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      979 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202111260.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1581 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202203140.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2200 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202203160.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      910 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202205250.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      979 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202206290.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      948 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202208180.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1881 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202208190.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      976 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202209090.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3957 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202209130.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      861 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202209160.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2919 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202211230.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1430 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202212010.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1494 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202301100.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      924 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202301110.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      977 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202301120.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      929 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202301160.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      896 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202301170.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1313 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202301190.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      860 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202302200.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1036 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202302270.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      825 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202303070.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1936 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202303071.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1027 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202304070.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1434 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v202306060.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1471 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v3.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3556 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v4.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1529 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v5.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1043 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v6.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1558 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/db/versions/v7.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    16471 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/deploy.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2694 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/docstring_parser.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    56412 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/env.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.737522 inmanta-core-8.5.0/src/inmanta/execute/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/execute/__init__.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.737522 inmanta-core-8.5.0/src/inmanta/execute/dataflow/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    41029 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/execute/dataflow/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     9488 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/execute/dataflow/datatrace.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7405 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/execute/dataflow/graphic.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7152 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/execute/dataflow/root_cause.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     8478 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/execute/proxy.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    50130 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/execute/runtime.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    30598 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/execute/scheduler.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1807 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/execute/tracking.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1451 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/execute/util.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    25819 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/export.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5488 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/file_parser.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    24386 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/loader.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    11292 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/logging.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    35363 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/main.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     9144 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/model.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)   141814 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/module.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    83857 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/moduletool.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.739522 inmanta-core-8.5.0/src/inmanta/parser/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2934 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/parser/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5803 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/parser/cache.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)   549509 2023-07-04 12:54:22.000000 inmanta-core-8.5.0/src/inmanta/parser/parser.out
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    71238 2023-07-04 12:54:22.000000 inmanta-core-8.5.0/src/inmanta/parser/parsetab.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1563 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/parser/pickle.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     8245 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/parser/plyInmantaLex.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    41546 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/parser/plyInmantaParser.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    23793 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/plugins.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5509 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/postgresproc.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      734 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/profile_mem.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.740522 inmanta-core-8.5.0/src/inmanta/protocol/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3131 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/protocol/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    42088 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/protocol/common.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     9024 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/protocol/decorators.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    17283 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/protocol/endpoints.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     4455 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/protocol/exceptions.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    33290 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/protocol/methods.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    64396 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/protocol/methods_v2.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.740522 inmanta-core-8.5.0/src/inmanta/protocol/openapi/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/protocol/openapi/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    20514 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/protocol/openapi/converter.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     9049 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/protocol/openapi/model.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.741522 inmanta-core-8.5.0/src/inmanta/protocol/rest/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    23049 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/protocol/rest/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6064 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/protocol/rest/client.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    13955 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/protocol/rest/server.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2158 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/protocol/return_value_meta.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/py.typed
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6396 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/reporter.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    23670 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/resources.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.742522 inmanta-core-8.5.0/src/inmanta/server/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1363 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    56173 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/agentmanager.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     9866 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/bootloader.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      688 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/compilerservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    10223 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/config.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7314 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/diff.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7672 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/extensions.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    27983 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/protocol.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7705 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/server.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.744522 inmanta-core-8.5.0/src/inmanta/server/services/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/services/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5702 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/services/codeservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    42567 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/services/compilerservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5790 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/services/databaseservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    11640 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/services/dryrunservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    25390 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/services/environment_metrics_service.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    29199 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/services/environmentservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6420 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/services/fileservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     4551 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/services/metricservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7970 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/services/notificationservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    64893 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/services/orchestrationservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    13898 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/services/paramservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6280 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/services/projectservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    48277 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/services/resourceservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     4852 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/services/userservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    11714 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/server/validate_filter.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      865 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/stable_api.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2927 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/types.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6908 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/user_setup.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    27310 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/util.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6487 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta/warnings.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.745522 inmanta-core-8.5.0/src/inmanta_core.egg-info/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3195 2023-07-04 12:54:32.000000 inmanta-core-8.5.0/src/inmanta_core.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7019 2023-07-04 12:54:32.000000 inmanta-core-8.5.0/src/inmanta_core.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-07-04 12:54:32.000000 inmanta-core-8.5.0/src/inmanta_core.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      129 2023-07-04 12:54:32.000000 inmanta-core-8.5.0/src/inmanta_core.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-07-04 12:54:13.000000 inmanta-core-8.5.0/src/inmanta_core.egg-info/not-zip-safe
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      586 2023-07-04 12:54:32.000000 inmanta-core-8.5.0/src/inmanta_core.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       36 2023-07-04 12:54:32.000000 inmanta-core-8.5.0/src/inmanta_core.egg-info/top_level.txt
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.721521 inmanta-core-8.5.0/src/inmanta_ext/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.745522 inmanta-core-8.5.0/src/inmanta_ext/core/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta_ext/core/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2238 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta_ext/core/extension.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.722521 inmanta-core-8.5.0/src/inmanta_plugins/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.745522 inmanta-core-8.5.0/src/inmanta_plugins/1/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/src/inmanta_plugins/1/__init__.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:32.751522 inmanta-core-8.5.0/tests/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7829 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_2way_protocol.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     8023 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_agent.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    54739 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_agent_manager.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    18854 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_app.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    12682 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_app_cli.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    12791 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_cache.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    18791 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_cli.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     4624 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_compilation.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7682 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_compiler_entrypoints.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    11564 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_config.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1300 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_const.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)   127475 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_data.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     8212 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_data_concurrency.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3426 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_data_model.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3912 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_deploy.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     8058 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_discovered_resources.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5151 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_docs_snippets.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3047 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_docstring_parser.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    27584 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_env.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    22013 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_export.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     9400 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_extension_loading.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2789 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_file_parser.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6573 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_handler.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     4111 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_import_entry_points.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5982 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_influxdbreporting.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     8541 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_io.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5352 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_jwt.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    18512 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_loader.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     8697 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_logging.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    58115 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_module_loader.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    18976 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_modules.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    33059 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_openapi.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      988 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_param.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    62820 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_parser.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6367 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_postgres.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2110 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_postgres_proc.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    24509 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_project.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3805 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_projectmetadata.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    78909 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_protocol.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3038 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_proxy.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    11162 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_resource.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    60705 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_server.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3664 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_type.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5678 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_usersetup.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    17775 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tests/test_util.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1924 2023-07-04 12:50:50.000000 inmanta-core-8.5.0/tox.ini
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.147137 inmanta-core-9.3.0/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    10174 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/LICENSE
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      311 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/MANIFEST.in
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3195 2023-07-04 11:30:06.147137 inmanta-core-9.3.0/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2238 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/README.md
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.114136 inmanta-core-9.3.0/misc/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       31 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/misc/extensions.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      402 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/misc/inmanta-agent.service
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      333 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/misc/inmanta-server.service
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     8762 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/misc/inmanta-workon-register.sh
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2906 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/misc/inmanta.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    12162 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/misc/inmanta.lang
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1256 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/misc/inmanta.vim
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      141 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/misc/logrotation_config
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1432 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/pyproject.toml
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      918 2023-07-04 11:30:06.148137 inmanta-core-9.3.0/setup.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3416 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/setup.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.112136 inmanta-core-9.3.0/src/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.118136 inmanta-core-9.3.0/src/inmanta/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      914 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/__init__.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.119136 inmanta-core-9.3.0/src/inmanta/agent/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      738 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/agent/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    59119 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/agent/agent.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    10115 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/agent/cache.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5149 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/agent/config.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    43297 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/agent/handler.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.119136 inmanta-core-9.3.0/src/inmanta/agent/io/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2815 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/agent/io/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    19884 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/agent/io/local.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6362 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/agent/io/remote.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3395 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/agent/reporting.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    28443 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/app.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.120136 inmanta-core-9.3.0/src/inmanta/ast/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    32500 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/ast/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7103 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/ast/attribute.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6354 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/ast/blocks.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.120136 inmanta-core-9.3.0/src/inmanta/ast/constraint/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/ast/constraint/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    17182 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/ast/constraint/expression.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    19266 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/ast/entity.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2783 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/ast/export.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.121136 inmanta-core-9.3.0/src/inmanta/ast/statements/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    23361 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/ast/statements/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    23834 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/ast/statements/assign.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    12314 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/ast/statements/call.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    24146 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/ast/statements/define.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    55960 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/ast/statements/generator.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    20775 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/ast/type.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    12524 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/ast/variables.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3400 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/command.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.121136 inmanta-core-9.3.0/src/inmanta/compiler/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    14509 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/compiler/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1963 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/compiler/config.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1110 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/compiler/data.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.122136 inmanta-core-9.3.0/src/inmanta/compiler/help/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/compiler/help/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     8327 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/compiler/help/explainer.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.122136 inmanta-core-9.3.0/src/inmanta/compiler/help/templates/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      235 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/compiler/help/templates/index_collision.j2
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3604 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/compiler/help/templates/modified_after_freeze.j2
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      733 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/compiler/help/templates/module_v2_in_v1_path.j2
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    20756 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/config.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     9233 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/const.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.123136 inmanta-core-9.3.0/src/inmanta/data/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)   242866 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/data/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    46598 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/data/dataview.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    21742 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/data/model.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    12206 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/data/schema.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.123136 inmanta-core-9.3.0/src/inmanta/db/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     8702 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/util.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.127137 inmanta-core-9.3.0/src/inmanta/db/versions/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    12123 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v1.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1737 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v17.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1393 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v2.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2443 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202105170.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      915 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202106080.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1247 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202106210.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1826 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202109100.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      979 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202111260.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1581 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202203140.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2200 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202203160.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      910 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202205250.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      979 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202206290.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      948 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202208180.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1881 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202208190.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      976 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202209090.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3957 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202209130.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      861 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202209160.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2919 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202211230.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1430 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202212010.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1494 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202301100.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      924 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202301110.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      977 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202301120.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      929 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202301160.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      896 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202301170.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1313 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202301190.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      860 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202302200.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1036 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202302270.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      825 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202303070.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1936 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202303071.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      989 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202304060.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1027 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202304070.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1434 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v202306060.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1471 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v3.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3556 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v4.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1529 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v5.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1043 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v6.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1558 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/db/versions/v7.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    16471 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/deploy.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2694 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/docstring_parser.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    57882 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/env.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.128136 inmanta-core-9.3.0/src/inmanta/execute/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/execute/__init__.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.128136 inmanta-core-9.3.0/src/inmanta/execute/dataflow/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    41029 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/execute/dataflow/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     9488 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/execute/dataflow/datatrace.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7405 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/execute/dataflow/graphic.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7152 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/execute/dataflow/root_cause.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     8478 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/execute/proxy.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    50130 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/execute/runtime.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    30598 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/execute/scheduler.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1807 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/execute/tracking.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1451 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/execute/util.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    25819 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/export.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5488 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/file_parser.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    24386 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/loader.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    11292 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/logging.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    35363 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/main.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     9144 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/model.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)   143695 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/module.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    83933 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/moduletool.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.130137 inmanta-core-9.3.0/src/inmanta/parser/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2934 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/parser/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5803 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/parser/cache.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)   549509 2023-07-04 11:29:55.000000 inmanta-core-9.3.0/src/inmanta/parser/parser.out
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    71238 2023-07-04 11:29:55.000000 inmanta-core-9.3.0/src/inmanta/parser/parsetab.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1563 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/parser/pickle.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     8245 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/parser/plyInmantaLex.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    41546 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/parser/plyInmantaParser.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    23793 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/plugins.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5509 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/postgresproc.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      734 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/profile_mem.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.132137 inmanta-core-9.3.0/src/inmanta/protocol/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3131 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/protocol/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    42088 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/protocol/common.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     9024 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/protocol/decorators.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    17283 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/protocol/endpoints.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     4455 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/protocol/exceptions.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    32616 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/protocol/methods.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    63705 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/protocol/methods_v2.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.132137 inmanta-core-9.3.0/src/inmanta/protocol/openapi/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/protocol/openapi/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    20514 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/protocol/openapi/converter.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     9049 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/protocol/openapi/model.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.133137 inmanta-core-9.3.0/src/inmanta/protocol/rest/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    23049 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/protocol/rest/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6064 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/protocol/rest/client.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    13955 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/protocol/rest/server.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2158 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/protocol/return_value_meta.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/py.typed
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6396 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/reporter.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    23670 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/resources.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.135137 inmanta-core-9.3.0/src/inmanta/server/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1363 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    56173 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/agentmanager.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     9866 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/bootloader.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      688 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/compilerservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    10223 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/config.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7314 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/diff.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7672 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/extensions.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    27983 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/protocol.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7705 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/server.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.138137 inmanta-core-9.3.0/src/inmanta/server/services/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/services/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5702 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/services/codeservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    42567 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/services/compilerservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5790 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/services/databaseservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    11640 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/services/dryrunservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    25390 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/services/environment_metrics_service.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    27899 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/services/environmentservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6420 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/services/fileservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     4551 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/services/metricservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7970 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/services/notificationservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    59626 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/services/orchestrationservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    13898 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/services/paramservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6280 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/services/projectservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    48277 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/services/resourceservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     4852 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/services/userservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    11714 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/server/validate_filter.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      865 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/stable_api.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2927 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/types.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6908 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/user_setup.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    27310 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/util.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6487 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta/warnings.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.139137 inmanta-core-9.3.0/src/inmanta_core.egg-info/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3195 2023-07-04 11:30:06.000000 inmanta-core-9.3.0/src/inmanta_core.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7057 2023-07-04 11:30:06.000000 inmanta-core-9.3.0/src/inmanta_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-07-04 11:30:06.000000 inmanta-core-9.3.0/src/inmanta_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      129 2023-07-04 11:30:06.000000 inmanta-core-9.3.0/src/inmanta_core.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-07-04 11:29:45.000000 inmanta-core-9.3.0/src/inmanta_core.egg-info/not-zip-safe
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      586 2023-07-04 11:30:06.000000 inmanta-core-9.3.0/src/inmanta_core.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       36 2023-07-04 11:30:06.000000 inmanta-core-9.3.0/src/inmanta_core.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.112136 inmanta-core-9.3.0/src/inmanta_ext/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.139137 inmanta-core-9.3.0/src/inmanta_ext/core/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta_ext/core/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2238 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta_ext/core/extension.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.112136 inmanta-core-9.3.0/src/inmanta_plugins/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.139137 inmanta-core-9.3.0/src/inmanta_plugins/1/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/src/inmanta_plugins/1/__init__.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:06.147137 inmanta-core-9.3.0/tests/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7829 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_2way_protocol.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     8023 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_agent.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    54739 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_agent_manager.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    18854 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_app.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    12682 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_app_cli.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    12791 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_cache.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    18791 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_cli.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     4624 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_compilation.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7682 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_compiler_entrypoints.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    11564 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_config.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1300 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_const.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)   123032 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_data.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     8212 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_data_concurrency.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3426 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_data_model.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3912 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_deploy.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     8058 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_discovered_resources.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5151 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_docs_snippets.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3047 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_docstring_parser.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    27584 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_env.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    22013 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_export.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     9400 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_extension_loading.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2789 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_file_parser.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6573 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_handler.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     4111 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_import_entry_points.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5982 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_influxdbreporting.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     8541 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_io.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5352 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_jwt.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    18512 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_loader.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     8697 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_logging.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    58413 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_module_loader.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    18976 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_modules.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    33059 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_openapi.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      988 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_param.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    62820 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_parser.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6367 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_postgres.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2110 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_postgres_proc.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    24277 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_project.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5585 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_projectmetadata.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    78909 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_protocol.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3038 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_proxy.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    11162 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_resource.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    62143 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_server.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3664 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_type.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5678 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_usersetup.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    17775 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tests/test_util.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1924 2023-07-04 11:27:43.000000 inmanta-core-9.3.0/tox.ini
```

### Comparing `inmanta-core-8.5.0/LICENSE` & `inmanta-core-9.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/PKG-INFO` & `inmanta-core-9.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmanta-core
-Version: 8.5.0
+Version: 9.3.0
 Summary: Inmanta deployment tool
 Home-page: https://github.com/inmanta/inmanta-core
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License 2
 Project-URL: Bug Tracker, https://github.com/inmanta/inmanta-core/issues
 Project-URL: Documentation, https://docs.inmanta.com/community/latest/
```

### Comparing `inmanta-core-8.5.0/README.md` & `inmanta-core-9.3.0/README.md`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/misc/inmanta-workon-register.sh` & `inmanta-core-9.3.0/misc/inmanta-workon-register.sh`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/misc/inmanta.cfg` & `inmanta-core-9.3.0/misc/inmanta.cfg`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/misc/inmanta.lang` & `inmanta-core-9.3.0/misc/inmanta.lang`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/misc/inmanta.vim` & `inmanta-core-9.3.0/misc/inmanta.vim`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/pyproject.toml` & `inmanta-core-9.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/setup.cfg` & `inmanta-core-9.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/setup.py` & `inmanta-core-9.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "8.5.0"
+version = "9.3.0"
 
 setup(
     version=version,
     python_requires=">=3.9",  # also update classifiers
     # Meta data
     name="inmanta-core",
     description="Inmanta deployment tool",
```

### Comparing `inmanta-core-8.5.0/src/inmanta/__init__.py` & `inmanta-core-9.3.0/src/inmanta/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
 
-COMPILER_VERSION = "2023.3"
+COMPILER_VERSION = "2024.0"
 RUNNING_TESTS = False
 """
     This is enabled/disabled by the test suite when tests are run.
     This variable is used to disable certain features that shouldn't run during tests.
 """
 
 if __name__ == "__main__":
```

### Comparing `inmanta-core-8.5.0/src/inmanta/agent/__init__.py` & `inmanta-core-9.3.0/src/inmanta/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/agent/agent.py` & `inmanta-core-9.3.0/src/inmanta/agent/agent.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/agent/cache.py` & `inmanta-core-9.3.0/src/inmanta/agent/cache.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/agent/config.py` & `inmanta-core-9.3.0/src/inmanta/agent/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 Each subsequent repair deployment will start agent-repair-interval seconds after the previous one.""",
     is_time,
 )
 
 agent_get_resource_backoff = Option(
     "config",
     "agent-get-resource-backoff",
-    5,
+    3,
     "This is a load management feature. It ensures that the agent will not pull resources from the inmanta server"
     " `<agent-get-resource-backoff>*<duration-last-pull-in-seconds>` seconds after the last time the agent pulled resources"
     " from the server. Setting this option too low may result in a high load on the Inmanta server. Setting it too high"
     " may result in long deployment times.",
     is_float,
 )
```

### Comparing `inmanta-core-8.5.0/src/inmanta/agent/handler.py` & `inmanta-core-9.3.0/src/inmanta/agent/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import base64
 import inspect
 import logging
 import traceback
 import typing
 import uuid
 from abc import ABC, abstractmethod
-from collections import abc, defaultdict
+from collections import defaultdict
 from concurrent.futures import Future
 from typing import Any, Callable, Dict, Generic, List, Optional, Tuple, Type, TypeVar, Union, cast, overload
 
 from tornado import concurrent
 
 import inmanta
 from inmanta import const, data, protocol, resources
@@ -390,18 +390,14 @@
             else:
                 raise InvalidOperation(f"Reported changes for {attribute} not in a type that is recognized.")
 
     @property
     def changes(self) -> Dict[str, AttributeStateChange]:
         return self._changes
 
-    def log_msg(self, level: int, msg: str, args: abc.Sequence[object], kwargs: abc.MutableMapping[str, object]) -> None:
-        LOGGER.warning("Direct calls to the log_msg method are being deprecated, please use the LoggerABC interface instead.")
-        self._log_msg(level, msg, *args, **kwargs)
-
     def _log_msg(self, level: int, msg: str, *args: object, exc_info: bool = False, **kwargs: object) -> None:
         if len(args) > 0:
             raise Exception("Args not supported")
         if exc_info:
             kwargs["traceback"] = traceback.format_exc()
 
         for k, v in kwargs.items():
```

### Comparing `inmanta-core-8.5.0/src/inmanta/agent/io/__init__.py` & `inmanta-core-9.3.0/src/inmanta/agent/io/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/agent/io/local.py` & `inmanta-core-9.3.0/src/inmanta/agent/io/local.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/agent/io/remote.py` & `inmanta-core-9.3.0/src/inmanta/agent/io/remote.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/agent/reporting.py` & `inmanta-core-9.3.0/src/inmanta/agent/reporting.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/app.py` & `inmanta-core-9.3.0/src/inmanta/app.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/ast/__init__.py` & `inmanta-core-9.3.0/src/inmanta/ast/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/ast/attribute.py` & `inmanta-core-9.3.0/src/inmanta/ast/attribute.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/ast/blocks.py` & `inmanta-core-9.3.0/src/inmanta/ast/blocks.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/ast/constraint/__init__.py` & `inmanta-core-9.3.0/src/inmanta/ast/constraint/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/ast/constraint/expression.py` & `inmanta-core-9.3.0/src/inmanta/ast/constraint/expression.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/ast/entity.py` & `inmanta-core-9.3.0/src/inmanta/ast/entity.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/ast/export.py` & `inmanta-core-9.3.0/src/inmanta/ast/export.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/ast/statements/__init__.py` & `inmanta-core-9.3.0/src/inmanta/ast/statements/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/ast/statements/assign.py` & `inmanta-core-9.3.0/src/inmanta/ast/statements/assign.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/ast/statements/call.py` & `inmanta-core-9.3.0/src/inmanta/ast/statements/call.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/ast/statements/define.py` & `inmanta-core-9.3.0/src/inmanta/ast/statements/define.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/ast/statements/generator.py` & `inmanta-core-9.3.0/src/inmanta/ast/statements/generator.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/ast/type.py` & `inmanta-core-9.3.0/src/inmanta/ast/type.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/ast/variables.py` & `inmanta-core-9.3.0/src/inmanta/ast/variables.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/command.py` & `inmanta-core-9.3.0/src/inmanta/command.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/compiler/__init__.py` & `inmanta-core-9.3.0/src/inmanta/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/compiler/config.py` & `inmanta-core-9.3.0/src/inmanta/compiler/config.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/compiler/data.py` & `inmanta-core-9.3.0/src/inmanta/compiler/data.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/compiler/help/__init__.py` & `inmanta-core-9.3.0/src/inmanta/compiler/help/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/compiler/help/explainer.py` & `inmanta-core-9.3.0/src/inmanta/compiler/help/explainer.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/compiler/help/templates/modified_after_freeze.j2` & `inmanta-core-9.3.0/src/inmanta/compiler/help/templates/modified_after_freeze.j2`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/compiler/help/templates/module_v2_in_v1_path.j2` & `inmanta-core-9.3.0/src/inmanta/compiler/help/templates/module_v2_in_v1_path.j2`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/config.py` & `inmanta-core-9.3.0/src/inmanta/config.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/const.py` & `inmanta-core-9.3.0/src/inmanta/const.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/data/__init__.py` & `inmanta-core-9.3.0/src/inmanta/data/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2383,15 +2383,14 @@
 AUTOSTART_ON_START = "autostart_on_start"
 AUTOSTART_AGENT_MAP = "autostart_agent_map"
 AUTOSTART_AGENT_INTERVAL = "autostart_agent_interval"
 AGENT_AUTH = "agent_auth"
 SERVER_COMPILE = "server_compile"
 AUTO_FULL_COMPILE = "auto_full_compile"
 RESOURCE_ACTION_LOGS_RETENTION = "resource_action_logs_retention"
-PURGE_ON_DELETE = "purge_on_delete"
 PROTECTED_ENVIRONMENT = "protected_environment"
 NOTIFICATION_RETENTION = "notification_retention"
 AVAILABLE_VERSIONS_TO_KEEP = "available_versions_to_keep"
 RECOMPILE_BACKOFF = "recompile_backoff"
 ENVIRONMENT_METRICS_RETENTION = "environment_metrics_retention"
 
 
@@ -2645,28 +2644,20 @@
         AVAILABLE_VERSIONS_TO_KEEP: Setting(
             name=AVAILABLE_VERSIONS_TO_KEEP,
             default=100,
             typ="int",
             validator=convert_int,
             doc="The number of versions to keep stored in the database",
         ),
-        PURGE_ON_DELETE: Setting(
-            name=PURGE_ON_DELETE,
-            default=False,
-            typ="bool",
-            validator=convert_boolean,
-            doc="Enable purge on delete. When set to true, the server will detect the absence of resources with purge_on_delete"
-            " set to true and automatically purges them.",
-        ),
         PROTECTED_ENVIRONMENT: Setting(
             name=PROTECTED_ENVIRONMENT,
             default=False,
             typ="bool",
             validator=convert_boolean,
-            doc="When set to true, this environment cannot be cleared, deleted or decommissioned.",
+            doc="When set to true, this environment cannot be cleared or deleted.",
         ),
         NOTIFICATION_RETENTION: Setting(
             name=NOTIFICATION_RETENTION,
             default=365,
             typ="int",
             validator=convert_int,
             doc="The number of days to retain notifications for",
@@ -4767,110 +4758,14 @@
             status=new_resource_state,
             last_non_deploying_status=const.NonDeployingResourceState[new_resource_state.name],
             resource_set=self.resource_set,
             provides=self.provides,
         )
 
     @classmethod
-    async def get_deleted_resources(
-        cls,
-        environment: uuid.UUID,
-        current_version: int,
-        current_resources: Sequence[m.ResourceIdStr],
-        *,
-        connection: Optional[asyncpg.connection.Connection] = None,
-    ) -> List["Resource"]:
-        """
-        This method returns all resources that have been deleted from the model and are not yet marked as purged. It returns
-        the latest version of the resource from a released model.
-
-        :param environment:
-        :param current_version:
-        :param current_resources: A Sequence of all resource ids in the current version.
-        """
-        LOGGER.debug("Starting purge_on_delete queries")
-
-        # get all models that have been released
-        query = (
-            "SELECT version FROM "
-            + ConfigurationModel.table_name()
-            + " WHERE environment=$1 AND released=TRUE ORDER BY version DESC LIMIT "
-            + str(DBLIMIT)
-        )
-        versions = set()
-        latest_version = None
-        async with cls.get_connection(connection) as con:
-            async with con.transaction():
-                async for record in con.cursor(query, cls._get_value(environment)):
-                    version = record["version"]
-                    versions.add(version)
-                    if latest_version is None:
-                        latest_version = version
-
-        LOGGER.debug("  All released versions: %s", versions)
-        LOGGER.debug("  Latest released version: %s", latest_version)
-
-        # find all resources in previous versions that have "purge_on_delete" set
-        (filter_statement, values) = cls._get_composed_filter(environment=environment, model=latest_version)
-        query = (
-            "SELECT DISTINCT resource_id FROM "
-            + cls.table_name()
-            + " WHERE "
-            + filter_statement
-            + " AND attributes @> $"
-            + str(len(values) + 1)
-        )
-        values.append(cls._get_value({"purge_on_delete": True}))
-        resources_records = await cls._fetch_query(query, *values, connection=connection)
-        resources = [r["resource_id"] for r in resources_records]
-
-        LOGGER.debug("  Resource with purge_on_delete true: %s", resources)
-
-        # all resources on current model
-        LOGGER.debug("  All resource in current version (%s): %s", current_version, current_resources)
-
-        # determined deleted resources
-
-        deleted = set(resources) - set(current_resources)
-        LOGGER.debug("  These resources are no longer present in current model: %s", deleted)
-
-        # filter out resources that should not be purged:
-        # 1- resources from versions that have not been deployed
-        # 2- resources that are already recorded as purged (purged and deployed)
-        should_purge = []
-        for deleted_resource in deleted:
-            # get the full resource history, and determine the purge status of this resource
-            (filter_statement, values) = cls._get_composed_filter(environment=environment, resource_id=deleted_resource)
-            query = (
-                "SELECT *"
-                + " FROM "
-                + cls.table_name()
-                + " WHERE "
-                + filter_statement
-                + " AND model < $"
-                + str(len(values) + 1)
-                + " ORDER BY model DESC"
-            )
-            values.append(cls._get_value(current_version))
-
-            async with cls.get_connection(connection) as con:
-                async with con.transaction():
-                    async for obj in con.cursor(query, *values):
-                        # if a resource is part of a released version and it is deployed (this last condition is actually enough
-                        # at the moment), we have found the last status of the resource. If it was not purged in that version,
-                        # add it to the should purge list.
-                        if obj["model"] in versions and obj["status"] == const.ResourceState.deployed.name:
-                            attributes = json.loads(str(obj["attributes"]))
-                            if not attributes["purged"]:
-                                should_purge.append(cls(from_postgres=True, **obj))
-                            break
-
-        return should_purge
-
-    @classmethod
     async def get_resource_details(cls, env: uuid.UUID, resource_id: m.ResourceIdStr) -> Optional[m.ReleasedResourceDetails]:
         status_subquery = """
         (CASE WHEN
             (SELECT resource.model < MAX(configurationmodel.version)
             FROM configurationmodel
             WHERE configurationmodel.released=TRUE
             AND environment = $1)
```

### Comparing `inmanta-core-8.5.0/src/inmanta/data/dataview.py` & `inmanta-core-9.3.0/src/inmanta/data/dataview.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/data/model.py` & `inmanta-core-9.3.0/src/inmanta/data/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,25 +303,14 @@
     type: str
     extra_data: Optional[JsonType]
 
     class Config:
         fields = {"inmanta_compile_state": {"alias": "inmanta:compile:state"}}
 
 
-class ModelVersionInfo(BaseModel):
-    """Version information that can be associated with an orchestration model
-
-    :param export_metadata: Metadata associated with this version
-    :param model: A serialization of the complete orchestration model
-    """
-
-    export_metadata: ModelMetadata
-    model: Optional[JsonType]
-
-
 class ResourceMinimal(BaseModel):
     """
     Represents a resource object as it comes in over the API. Provides strictly required validation only.
     """
 
     id: ResourceVersionIdStr
```

### Comparing `inmanta-core-8.5.0/src/inmanta/data/schema.py` & `inmanta-core-9.3.0/src/inmanta/data/schema.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/__init__.py` & `inmanta-core-9.3.0/src/inmanta/db/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/util.py` & `inmanta-core-9.3.0/src/inmanta/db/util.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/__init__.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v1.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v1.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v17.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v17.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v2.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v2.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202105170.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202105170.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202106080.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202106080.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202106210.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202106210.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202109100.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202109100.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202111260.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202111260.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202203140.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202203140.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202203160.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202203160.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202205250.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202205250.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202206290.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202206290.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202208180.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202208180.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202208190.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202208190.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202209090.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202209090.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202209130.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202209130.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202209160.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202209160.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202211230.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202211230.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202212010.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202212010.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202301100.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202301100.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202301110.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202301110.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202301120.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202301120.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202301160.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202301160.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202301170.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202301170.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202301190.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202301190.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202302200.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202302200.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202302270.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202302270.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202303070.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202303070.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202303071.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202303071.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202304070.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202304070.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v202306060.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v202306060.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v3.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v3.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v4.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v4.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v5.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v5.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v6.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v6.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/db/versions/v7.py` & `inmanta-core-9.3.0/src/inmanta/db/versions/v7.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/deploy.py` & `inmanta-core-9.3.0/src/inmanta/deploy.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/docstring_parser.py` & `inmanta-core-9.3.0/src/inmanta/docstring_parser.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/env.py` & `inmanta-core-9.3.0/src/inmanta/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,43 +327,58 @@
         paths: Optional[List[LocalPackagePath]] = None,
         index_urls: Optional[List[str]] = None,
         upgrade: bool = False,
         upgrade_strategy: PipUpgradeStrategy = PipUpgradeStrategy.ONLY_IF_NEEDED,
         allow_pre_releases: bool = False,
         constraints_files: Optional[List[str]] = None,
         requirements_files: Optional[List[str]] = None,
+        use_pip_config: bool = False,
     ) -> List[str]:
         """
         Generate `pip install` command from the given arguments.
 
         :param python_path: The python interpreter to use in the command
         :param requirements: The requirements that should be installed
         :param paths: Paths to python projects on disk that should be installed in the venv.
         :param index_urls: The Python package repositories to use. When set to None, the system default will be used.
         :param upgrade: Upgrade the specified packages to the latest version.
         :param upgrade_strategy: The upgrade strategy to use for requirements' dependencies.
         :param allow_pre_releases: Allow the installation of packages with pre-releases and development versions.
         :param constraints_files: Files that should be passed to pip using the `-c` option.
         :param requirements_files: Files that should be passed to pip using the `-r` option.
+        :param use_pip_config: Whether the pip config file specified in the PIP_CONFIG_FILE env var should be used
         """
         requirements = requirements if requirements is not None else []
         paths = paths if paths is not None else []
         local_paths: Iterator[LocalPackagePath] = (
             # make sure we only try to install from a local source: add leading `./` and trailing `/` to explicitly tell pip
             # we're pointing to a local directory.
             LocalPackagePath(path=os.path.join(".", path.path, ""), editable=path.editable)
             for path in paths
         )
-        index_args: List[str] = (
-            []
-            if index_urls is None
-            else ["--index-url", index_urls[0], *chain.from_iterable(["--extra-index-url", url] for url in index_urls[1:])]
-            if index_urls
-            else ["--no-index"]
-        )
+        index_args: list[str] = []
+
+        if use_pip_config:
+            if index_urls:
+                # Use only --extra-index-url arguments
+                for url in index_urls:
+                    index_args.append("--extra-index-url")
+                    index_args.append(url)
+        elif index_urls is None:
+            pass
+        elif index_urls:
+            # Use separate --index-url and --extra-index-url arguments
+            index_args.append("--index-url")
+            index_args.append(index_urls[0])
+            for url in index_urls[1:]:
+                index_args.append("--extra-index-url")
+                index_args.append(url)
+        else:
+            index_args = ["--no-index"]
+
         constraints_files = constraints_files if constraints_files is not None else []
         requirements_files = requirements_files if requirements_files is not None else []
         return [
             python_path,
             "-m",
             "pip",
             "install",
@@ -468,31 +483,32 @@
         paths: Optional[List[LocalPackagePath]] = None,
         index_urls: Optional[List[str]] = None,
         upgrade: bool = False,
         upgrade_strategy: PipUpgradeStrategy = PipUpgradeStrategy.ONLY_IF_NEEDED,
         allow_pre_releases: bool = False,
         constraints_files: Optional[List[str]] = None,
         requirements_files: Optional[List[str]] = None,
+        use_pip_config: Optional[bool] = False,
     ) -> None:
         cmd: List[str] = PipCommandBuilder.compose_install_command(
             python_path=python_path,
             requirements=requirements,
             paths=paths,
             index_urls=index_urls,
             upgrade=upgrade,
             upgrade_strategy=upgrade_strategy,
             allow_pre_releases=allow_pre_releases,
             constraints_files=constraints_files,
             requirements_files=requirements_files,
+            use_pip_config=use_pip_config,
         )
-
         sub_env = os.environ.copy()
 
         # if index_urls are set, only use those. Otherwise, use the one from the environment
-        if index_urls is not None:
+        if index_urls is not None and not use_pip_config:
             # setting this env_var to os.devnull disables the loading of all pip configuration files
             sub_env["PIP_CONFIG_FILE"] = os.devnull
         if index_urls is not None and "PIP_EXTRA_INDEX_URL" in sub_env:
             del sub_env["PIP_EXTRA_INDEX_URL"]
         if index_urls is not None and "PIP_INDEX_URL" in sub_env:
             del sub_env["PIP_INDEX_URL"]
 
@@ -574,42 +590,49 @@
         self,
         requirements: List[Requirement],
         index_urls: Optional[List[str]] = None,
         upgrade: bool = False,
         allow_pre_releases: bool = False,
         constraint_files: Optional[List[str]] = None,
         upgrade_strategy: PipUpgradeStrategy = PipUpgradeStrategy.ONLY_IF_NEEDED,
+        use_pip_config: Optional[bool] = False,
     ) -> None:
         if len(requirements) == 0:
             raise Exception("install_from_index requires at least one requirement to install")
         constraint_files = constraint_files if constraint_files is not None else []
         inmanta_requirements = self._get_requirements_on_inmanta_package()
         self._run_pip_install_command(
             python_path=self.python_path,
             requirements=[*requirements, *inmanta_requirements],
             index_urls=index_urls,
             upgrade=upgrade,
             allow_pre_releases=allow_pre_releases,
             constraints_files=[*constraint_files],
             upgrade_strategy=upgrade_strategy,
+            use_pip_config=use_pip_config,
         )
 
-    def install_from_source(self, paths: List[LocalPackagePath], constraint_files: Optional[List[str]] = None) -> None:
+    def install_from_source(
+        self,
+        paths: List[LocalPackagePath],
+        constraint_files: Optional[List[str]] = None,
+    ) -> None:
         """
         Install one or more packages from source. Any path arguments should be local paths to a package directory or wheel.
         """
         if len(paths) == 0:
             raise Exception("install_from_source requires at least one package to install")
         constraint_files = constraint_files if constraint_files is not None else []
         inmanta_requirements = self._get_requirements_on_inmanta_package()
         self._run_pip_install_command(
             python_path=self.python_path,
             paths=paths,
             constraints_files=constraint_files,
             requirements=inmanta_requirements,
+            use_pip_config=True,
         )
 
     @classmethod
     def get_protected_inmanta_packages(cls) -> List[str]:
         """
         Returns the list of packages that should not be installed/updated by any operation on a Python environment.
         """
@@ -735,25 +758,30 @@
         self,
         requirements: List[Requirement],
         index_urls: Optional[List[str]] = None,
         upgrade: bool = False,
         allow_pre_releases: bool = False,
         constraint_files: Optional[List[str]] = None,
         upgrade_strategy: PipUpgradeStrategy = PipUpgradeStrategy.ONLY_IF_NEEDED,
+        use_pip_config: Optional[bool] = False,
     ) -> None:
         if not upgrade and self.are_installed(requirements):
             return
         try:
             super(ActiveEnv, self).install_from_index(
-                requirements, index_urls, upgrade, allow_pre_releases, constraint_files, upgrade_strategy
+                requirements, index_urls, upgrade, allow_pre_releases, constraint_files, upgrade_strategy, use_pip_config
             )
         finally:
             self.notify_change()
 
-    def install_from_source(self, paths: List[LocalPackagePath], constraint_files: Optional[List[str]] = None) -> None:
+    def install_from_source(
+        self,
+        paths: List[LocalPackagePath],
+        constraint_files: Optional[List[str]] = None,
+    ) -> None:
         try:
             super().install_from_source(paths, constraint_files)
         finally:
             self.notify_change()
 
     @classmethod
     def _parse_line(cls, req_line: str) -> Tuple[Optional[str], str]:
@@ -847,37 +875,42 @@
 
     def install_from_list(
         self,
         requirements_list: Sequence[str],
         *,
         upgrade: bool = False,
         upgrade_strategy: PipUpgradeStrategy = PipUpgradeStrategy.ONLY_IF_NEEDED,
+        use_pip_config: Optional[bool] = False,
     ) -> None:
         """
         Install requirements from a list of requirement strings. This method uses the Python package repositories
         configured on the host.
 
         :param requirements_list: List of requirement strings to install.
         :param upgrade: Upgrade requirements to the latest compatible version.
         :param upgrade_strategy: The upgrade strategy to use for requirements' dependencies.
+        :param use_pip_config: Whether the pip config file specified in the PIP_CONFIG_FILE env var should be used
         """
         if not upgrade and self.are_installed(requirements_list):
             # don't fork subprocess if requirements are already met
             return
         try:
-            self._install_from_list(requirements_list, upgrade=upgrade, upgrade_strategy=upgrade_strategy)
+            self._install_from_list(
+                requirements_list, upgrade=upgrade, upgrade_strategy=upgrade_strategy, use_pip_config=use_pip_config
+            )
         finally:
             self.notify_change()
 
     def _install_from_list(
         self,
         requirements_list: Sequence[str],
         *,
         upgrade: bool = False,
         upgrade_strategy: PipUpgradeStrategy = PipUpgradeStrategy.ONLY_IF_NEEDED,
+        use_pip_config: Optional[bool] = False,
     ) -> None:
         """
         This method differs from the `install_from_index()` method in the sense that it calls
         `_gen_content_requirements_file()`, which rewrites the requirements from pep440 format to a format that pip understands.
         This method is maintained for V1 modules only: V2 modules do not require this conversion. It is currently used for both
         v1 and v2 for consistency but it can be substituted by `install_from_index` once V1 support is removed.
         """
@@ -887,14 +920,15 @@
             try:
                 self._run_pip_install_command(
                     python_path=self.python_path,
                     requirements_files=[requirements_file],
                     requirements=inmanta_requirements,
                     upgrade=upgrade,
                     upgrade_strategy=upgrade_strategy,
+                    use_pip_config=use_pip_config,
                 )
             except Exception:
                 LOGGER.info("requirements:\n%s", content_requirements_file)
                 raise
 
     @classmethod
     def get_constraint_violations_for_check(
@@ -1282,36 +1316,44 @@
         self,
         requirements: List[Requirement],
         index_urls: Optional[List[str]] = None,
         upgrade: bool = False,
         allow_pre_releases: bool = False,
         constraint_files: Optional[List[str]] = None,
         upgrade_strategy: PipUpgradeStrategy = PipUpgradeStrategy.ONLY_IF_NEEDED,
+        use_pip_config: Optional[bool] = False,
     ) -> None:
         if not self._using_venv:
             raise Exception(f"Not using venv {self.env_path}. use_virtual_env() should be called first.")
         super(VirtualEnv, self).install_from_index(
-            requirements, index_urls, upgrade, allow_pre_releases, constraint_files, upgrade_strategy
+            requirements, index_urls, upgrade, allow_pre_releases, constraint_files, upgrade_strategy, use_pip_config
         )
 
-    def install_from_source(self, paths: List[LocalPackagePath], constraint_files: Optional[List[str]] = None) -> None:
+    def install_from_source(
+        self,
+        paths: List[LocalPackagePath],
+        constraint_files: Optional[List[str]] = None,
+    ) -> None:
         if not self._using_venv:
             raise Exception(f"Not using venv {self.env_path}. use_virtual_env() should be called first.")
         super(VirtualEnv, self).install_from_source(paths, constraint_files)
 
     def install_from_list(
         self,
         requirements_list: Sequence[str],
         *,
         upgrade: bool = False,
         upgrade_strategy: PipUpgradeStrategy = PipUpgradeStrategy.ONLY_IF_NEEDED,
+        use_pip_config: Optional[bool] = False,
     ) -> None:
         if not self._using_venv:
             raise Exception(f"Not using venv {self.env_path}. use_virtual_env() should be called first.")
-        super(VirtualEnv, self).install_from_list(requirements_list, upgrade=upgrade, upgrade_strategy=upgrade_strategy)
+        super(VirtualEnv, self).install_from_list(
+            requirements_list, upgrade=upgrade, upgrade_strategy=upgrade_strategy, use_pip_config=use_pip_config
+        )
 
 
 class VenvCreationFailedError(Exception):
     def __init__(self, msg: str) -> None:
         super().__init__(msg)
         self.msg = msg
```

### Comparing `inmanta-core-8.5.0/src/inmanta/execute/__init__.py` & `inmanta-core-9.3.0/src/inmanta/execute/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/execute/dataflow/__init__.py` & `inmanta-core-9.3.0/src/inmanta/execute/dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/execute/dataflow/datatrace.py` & `inmanta-core-9.3.0/src/inmanta/execute/dataflow/datatrace.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/execute/dataflow/graphic.py` & `inmanta-core-9.3.0/src/inmanta/execute/dataflow/graphic.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/execute/dataflow/root_cause.py` & `inmanta-core-9.3.0/src/inmanta/execute/dataflow/root_cause.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/execute/proxy.py` & `inmanta-core-9.3.0/src/inmanta/execute/proxy.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/execute/runtime.py` & `inmanta-core-9.3.0/src/inmanta/execute/runtime.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/execute/scheduler.py` & `inmanta-core-9.3.0/src/inmanta/execute/scheduler.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/execute/tracking.py` & `inmanta-core-9.3.0/src/inmanta/execute/tracking.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/execute/util.py` & `inmanta-core-9.3.0/src/inmanta/execute/util.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/export.py` & `inmanta-core-9.3.0/src/inmanta/export.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/file_parser.py` & `inmanta-core-9.3.0/src/inmanta/file_parser.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/loader.py` & `inmanta-core-9.3.0/src/inmanta/loader.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/logging.py` & `inmanta-core-9.3.0/src/inmanta/logging.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/main.py` & `inmanta-core-9.3.0/src/inmanta/main.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/model.py` & `inmanta-core-9.3.0/src/inmanta/model.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/module.py` & `inmanta-core-9.3.0/src/inmanta/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
 
 import configparser
-import enum
 import glob
 import importlib
+import itertools
 import logging
 import operator
 import os
 import re
 import subprocess
 import sys
 import tempfile
@@ -31,14 +31,15 @@
 import traceback
 import types
 import warnings
 from abc import ABC, abstractmethod
 from collections import abc, defaultdict
 from configparser import ConfigParser
 from dataclasses import dataclass
+from enum import Enum
 from functools import reduce
 from importlib.abc import Loader
 from io import BytesIO, TextIOBase
 from itertools import chain
 from subprocess import CalledProcessError
 from tarfile import TarFile
 from time import time
@@ -319,15 +320,15 @@
             f"Unable to load all plug-ins for module {self.module}:"
             f"\n\t{cause_type_name} while loading plugin module {self.fq_import}: {self.cause}"
         )
         exception.set_location(Location(self.path, self.lineno if self.lineno is not None else 0))
         return exception
 
 
-class UntrackedFilesMode(enum.Enum):
+class UntrackedFilesMode(Enum):
     """
     The different options that can be passed to the --untracked-files option of the `git status` command.
     """
 
     ALL = "all"
     NORMAL = "normal"
     NO = "no"
@@ -708,21 +709,22 @@
 
     @classmethod
     def get_namespace_package_name(cls, module_name: str) -> str:
         return f"{const.PLUGINS_PACKAGE}.{module_name}"
 
     def install(self, project: "Project", module_spec: List[InmantaModuleRequirement]) -> Optional["ModuleV2"]:
         module_name: str = self._get_module_name(module_spec)
-        if not self.urls:
+        if not self.urls and not project.metadata.pip.use_config_file:
             raise Exception(
-                f"Attempting to install a v2 module {module_name} but no v2 module source is configured. Add at least one "
-                'repo of type "package" to the project config file. e.g. to add PyPi as a module source, add the following to '
-                "the `repo` section of the project's `project.yml`:"
-                "\n\t- type: package"
-                "\n\t  url: https://pypi.org/simple"
+                f"Attempting to install a v2 module {module_name} but no v2 module source is configured. Add the relevant pip "
+                f"indexes to the project config file. e.g. to add PyPi as a module source, add the following to "
+                "the `pip` section of the project's `project.yml`:"
+                "\n\t  index_urls:"
+                "\n\t\t  - https://pypi.org/simple"
+                "\nAnother option is to set the use_config_file project option to true to use the system's pip config file."
             )
         requirements: List[Requirement] = [req.get_python_package_requirement() for req in module_spec]
         allow_pre_releases = project is not None and project.install_mode in {InstallMode.prerelease, InstallMode.master}
         preinstalled: Optional[ModuleV2] = self.get_installed_module(project, module_name)
 
         # Get known requires and add them to prevent invalidating constraints through updates
         # These could be constraints (-c) as well, but that requires additional sanitation
@@ -739,16 +741,20 @@
                     module_name,
                     preinstalled_version,
                     ",".join(constraint.version_spec_str() for constraint in module_spec if constraint.specs),
                 )
         try:
             self.log_pre_install_information(module_name, module_spec)
             modules_pre_install = self.take_v2_modules_snapshot(header="Modules versions before installation:")
-            env.process_env.install_from_index(requirements, self.urls, allow_pre_releases=allow_pre_releases)
-
+            env.process_env.install_from_index(
+                requirements,
+                self.urls,
+                allow_pre_releases=allow_pre_releases,
+                use_pip_config=project.metadata.pip.use_config_file,
+            )
             self.log_post_install_information(module_name)
             self.log_snapshot_difference_v2_modules(modules_pre_install, header="Modules versions after installation:")
         except env.PackageNotFound:
             return None
         path: Optional[str] = self.path_for(module_name)
         if path is None:
             python_package: str = ModuleV2Source.get_package_name_for(module_name)
@@ -1057,15 +1063,15 @@
         if key not in mainspec:
             mainspec[key] = [req]
         else:
             mainspec[key] = mainspec[key] + [req]
 
 
 @stable_api
-class InstallMode(str, enum.Enum):
+class InstallMode(str, Enum):
     """
     The module install mode determines what version of a module should be selected when a module is downloaded.
     """
 
     release = "release"
     """
     Only use a released version that is compatible with the current compiler and any version constraints defined in the
@@ -1094,15 +1100,15 @@
 INSTALL_OPTS: List[str] = [mode.value for mode in InstallMode]  # Part of the stable API
 """
 List of possible module install modes, kept for backwards compatibility. New code should use :class:`InstallMode` instead.
 """
 
 
 @stable_api
-class FreezeOperator(str, enum.Enum):
+class FreezeOperator(str, Enum):
     eq = "=="
     compatible = "~="
     ge = ">="
 
     @classmethod
     def get_regex_for_validation(cls) -> str:
         all_values = [re.escape(o.value) for o in cls]
@@ -1477,15 +1483,15 @@
                 out.add_section("egg_info")
             out.set("egg_info", "tag_build", self.version_tag)
 
         return out
 
 
 @stable_api
-class ModuleRepoType(enum.Enum):
+class ModuleRepoType(Enum):
     git = "git"
     package = "package"
 
 
 @stable_api
 class ModuleRepoInfo(BaseModel):
     url: str
@@ -1525,14 +1531,31 @@
         )
 
     def __str__(self) -> str:
         return f"{self.first_type}.{self.first_relation_name} before {self.then_type}.{self.then_relation_name}"
 
 
 @stable_api
+class ProjectPipConfig(BaseModel):
+    """
+    :param use_config_file: Indicates whether the pip configuration files have to be taken into account when installing
+        Python packages.
+    :param index_urls: List of pip indexes to use project-wide. These repositories should be
+        `PEP 503 <https://www.python.org/dev/peps/pep-0503/>`_ (the simple repository API)
+        compliant. If more than one index url is configured, they will all be passed to pip. This is generally only
+        recommended if all configured indexes are under full control of the end user to protect against dependency
+        confusion attacks. See the `pip install documentation <https://pip.pypa.io/en/stable/cli/pip_install/>`_ and
+        `PEP 708 (draft) <https://peps.python.org/pep-0708/>`_ for more information.
+    """
+
+    use_config_file: bool = False
+    index_urls: List[str] = []
+
+
+@stable_api
 class ProjectMetadata(Metadata, MetadataFieldRequires):
     """
     :param name: The name of the project.
     :param description: (Optional) An optional description of the project
     :param author: (Optional) The author of the project
     :param author_email: (Optional) The contact email address of author
     :param license: (Optional) License the project is released under
@@ -1545,20 +1568,16 @@
     :param repo: (Optional) A list (a yaml list) of repositories where Inmanta can find modules. Inmanta tries each repository
         in the order they appear in the list. Each element of this list requires a ``type`` and a ``url`` field. The type field
         can have the following values:
 
         * git: When the type is set to git, the url field should contain a template of the Git repo URL. Inmanta creates the
           git repo url by formatting {} or {0} with the name of the module. If no formatter is present it appends the name
           of the module to the URL.
-        * package: When the type is set to package, the URL field should contain the URL of the Python package repository.
-          The repository should be `PEP 503 <https://www.python.org/dev/peps/pep-0503/>`_ (the simple repository API)
-          compliant. If more than one package url is configured, they will all be passed to pip. This is generally only
-          recommended if all configured indexes are under full control of the end user to protect against dependency
-          confusion attacks. See the `pip install documentation <https://pip.pypa.io/en/stable/cli/pip_install/>`_ and
-          `PEP 708 (draft) <https://peps.python.org/pep-0708/>`_ for more information.
+        * package: [DEPRECATED] Setting up pip indexes should be done via the ``index_urls`` option of the ``pip`` section. See
+          :py:class:`inmanta.module.ProjectPipConfig` for more details.
 
         The old syntax, which only defines a Git URL per list entry is maintained for backward compatibility.
     :param requires: (Optional) This key can contain a list (a yaml list) of version constraints for modules used in this
         project. Similar to the module, version constraints are defined using
         `PEP440 syntax <https://www.python.org/dev/peps/pep-0440/#version-specifiers>`_.
     :param freeze_recursive: (Optional) This key determined if the freeze command will behave recursively or not. If
         freeze_recursive is set to false or not set, the current version of all modules imported directly in the main.cf file
@@ -1589,14 +1608,16 @@
         account when making changes to handler code.
 
         Another caveat is that if the dependency module does contain code that is relevant for the agent, it will be loaded
         like any other handler code and it will be this code that is imported by any dependent modules (though depending on
         the load order the very first import may use the version installed by pip). If at some point this dependency module's
         handlers cease to be relevant for this agent, its code will remain stale. Therefore this feature should not be depended
         on in transient scenarios like this.
+    :param pip: A configuration section that holds information about the pip configuration that should be taken into account
+                when installing Python packages (See: :py:class:`inmanta.module.ProjectPipConfig` for more details).
     """
 
     _raw_parser: Type[YamlParser] = YamlParser
     _re_relation_precedence_rule: str = r"^(?P<ft>[^\s.]+)\.(?P<fr>[^\s.]+)\s+before\s+(?P<tt>[^\s.]+)\.(?P<tr>[^\s.]+)$"
     _re_relation_precedence_rule_compiled: re.Pattern[str] = re.compile(_re_relation_precedence_rule)
 
     author: Optional[str] = None
@@ -1607,14 +1628,15 @@
     repo: List[ModuleRepoInfo] = []
     downloadpath: Optional[str] = None
     install_mode: InstallMode = InstallMode.release
     requires: List[str] = []
     relation_precedence_policy: List[constr(strip_whitespace=True, regex=_re_relation_precedence_rule, min_length=1)] = []
     strict_deps_check: bool = True
     agent_install_dependency_modules: bool = False
+    pip: ProjectPipConfig = ProjectPipConfig()
 
     @validator("modulepath", pre=True)
     @classmethod
     def modulepath_to_list(cls, v: object) -> object:
         return cls.to_list(v)
 
     @validator("repo", pre=True)
@@ -1623,27 +1645,37 @@
         v_as_list = cls.to_list(v)
         result = []
         for elem in v_as_list:
             if isinstance(elem, str):
                 # Ensure backward compatibility with the version of Inmanta that didn't have support for the type field.
                 result.append({"url": elem, "type": ModuleRepoType.git})
             elif isinstance(elem, dict):
+                if elem["type"] == ModuleRepoType.package.value:
+                    LOGGER.warning(
+                        "Setting a pip index through the `repo -> url` option with type `package` in the project.yml file "
+                        "is deprecated. Please set the pip index url through the `pip -> index_urls` option instead."
+                    )
                 result.append(elem)
             else:
                 raise ValueError(f"Value should be either a string of a dict, got {elem}")
         return result
 
     def get_relation_precedence_rules(self) -> List[RelationPrecedenceRule]:
         """
         Return all RelationPrecedenceRules defined in the project.yml file.
         """
         return [RelationPrecedenceRule.from_string(rule_as_str) for rule_as_str in self.relation_precedence_policy]
 
     def get_index_urls(self) -> List[str]:
-        return [repo.url for repo in self.repo if repo.type == ModuleRepoType.package]
+        # Once setting repos with type package is no longer supported, this method can return self.pip.index_urls alone.
+        index_urls_deprecated_option: List[str] = [repo.url for repo in self.repo if repo.type == ModuleRepoType.package]
+
+        # This ensures no duplicates are returned and insertion order is preserved.
+        # i.e. the left-most index will be passed to pip as --index-url and the others as --extra-index-url
+        return list({value: None for value in itertools.chain(self.pip.index_urls, index_urls_deprecated_option)})
 
 
 @stable_api
 class ModuleLike(ABC, Generic[TMetadata]):
     """
     Commons superclass for projects and modules, which are both versioned by git
 
@@ -2058,14 +2090,15 @@
         if len(pyreq) > 0:
             # upgrade both direct and transitive module dependencies: eager upgrade strategy
             self.virtualenv.install_from_index(
                 pyreq,
                 upgrade=update_dependencies,
                 index_urls=indexes_urls if indexes_urls else None,
                 upgrade_strategy=env.PipUpgradeStrategy.EAGER,
+                use_pip_config=self.metadata.pip.use_config_file,
             )
 
         self.verify()
 
     def load(self, install: bool = False) -> None:
         """
         Load this project's AST and plugins.
@@ -2353,15 +2386,14 @@
         """
         if not self.is_using_virtual_env():
             self.use_virtual_env()
         reqs: Mapping[str, List[InmantaModuleRequirement]] = self.collect_requirements()
         module_reqs: List[InmantaModuleRequirement] = (
             list(reqs[module_name]) if module_name in reqs else [InmantaModuleRequirement.parse(module_name)]
         )
-
         module: Optional[Union[ModuleV1, ModuleV2]]
         try:
             module = self.module_source.get_module(self, module_reqs, install=install_v2)
             if module is not None and self.module_source_v1.path_for(module_name) is not None:
                 LOGGER.warning("Module %s is installed as a V1 module and a V2 module: V1 will be ignored.", module_name)
             if module is None and allow_v1:
                 module = self.module_source_v1.get_module(self, module_reqs, install=install_v1)
@@ -2671,15 +2703,15 @@
         super().__init__(tempfile.gettempdir(), autostd=autostd, attach_cf_cache=False)
 
     def _get_metadata_from_disk(self) -> ProjectMetadata:
         return ProjectMetadata(name="DUMMY")
 
 
 @stable_api
-class ModuleGeneration(enum.Enum):
+class ModuleGeneration(Enum):
     """
     The generation of a module. This might affect the on-disk structure of a module as well as how it's distributed.
     """
 
     V1: int = 1
     V2: int = 2
```

### Comparing `inmanta-core-8.5.0/src/inmanta/moduletool.py` & `inmanta-core-9.3.0/src/inmanta/moduletool.py`

 * *Files 0% similar despite different names*

```diff
@@ -485,14 +485,15 @@
                 # Because for pip not every valid -r is a valid -c
                 current_requires = my_project.get_strict_python_requirements_as_list()
                 env.process_env.install_from_index(
                     v2_python_specs + [Requirement.parse(r) for r in current_requires],
                     my_project.module_source.urls,
                     upgrade=True,
                     allow_pre_releases=my_project.install_mode != InstallMode.release,
+                    use_pip_config=my_project.metadata.pip.use_config_file,
                 )
 
             for v1_module in set(modules).difference(v2_modules):
                 spec = specs.get(v1_module, [])
                 try:
                     ModuleV1.update(my_project, v1_module, spec, install_mode=my_project.install_mode)
                 except Exception:
```

### Comparing `inmanta-core-8.5.0/src/inmanta/parser/__init__.py` & `inmanta-core-9.3.0/src/inmanta/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/parser/cache.py` & `inmanta-core-9.3.0/src/inmanta/parser/cache.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/parser/parser.out` & `inmanta-core-9.3.0/src/inmanta/parser/parser.out`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/parser/parsetab.py` & `inmanta-core-9.3.0/src/inmanta/parser/parsetab.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/parser/pickle.py` & `inmanta-core-9.3.0/src/inmanta/parser/pickle.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/parser/plyInmantaLex.py` & `inmanta-core-9.3.0/src/inmanta/parser/plyInmantaLex.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/parser/plyInmantaParser.py` & `inmanta-core-9.3.0/src/inmanta/parser/plyInmantaParser.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/plugins.py` & `inmanta-core-9.3.0/src/inmanta/plugins.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/postgresproc.py` & `inmanta-core-9.3.0/src/inmanta/postgresproc.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/profile_mem.py` & `inmanta-core-9.3.0/src/inmanta/profile_mem.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/protocol/__init__.py` & `inmanta-core-9.3.0/src/inmanta/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/protocol/common.py` & `inmanta-core-9.3.0/src/inmanta/protocol/common.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/protocol/decorators.py` & `inmanta-core-9.3.0/src/inmanta/protocol/decorators.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/protocol/endpoints.py` & `inmanta-core-9.3.0/src/inmanta/protocol/endpoints.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/protocol/exceptions.py` & `inmanta-core-9.3.0/src/inmanta/protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/protocol/methods.py` & `inmanta-core-9.3.0/src/inmanta/protocol/methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,37 +245,14 @@
     :param tid: The environment id
     :param client_types: The client types for which this token is valid (api, agent, compiler)
     :param idempotent: The token should be idempotent, such tokens do not have an expire or issued at set so their
                        value will not change.
     """
 
 
-#  Decomission an environment
-
-
-@method(
-    path="/decommission/<id>",
-    operation="POST",
-    arg_options={"id": ArgOption(getter=convert_environment)},
-    client_types=[const.ClientType.api],
-    api_version=1,
-)
-def decomission_environment(id: uuid.UUID, metadata: dict = None):
-    """
-    Decommision an environment. This is done by uploading an empty model to the server and let purge_on_delete handle
-    removal.
-
-    :param id: The uuid of the environment.
-    :param metadata: Optional metadata associated with the decommissioning
-
-    :raises NotFound: The given environment doesn't exist.
-    :raises Forbidden: The given environment is protected.
-    """
-
-
 @method(
     path="/decommission/<id>",
     operation="DELETE",
     arg_options={"id": ArgOption(getter=convert_environment)},
     client_types=[const.ClientType.api],
 )
 def clear_environment(id: uuid.UUID):
```

### Comparing `inmanta-core-8.5.0/src/inmanta/protocol/methods_v2.py` & `inmanta-core-9.3.0/src/inmanta/protocol/methods_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,34 +245,14 @@
 
     :raises NotFound: The given environment doesn't exist.
     """
 
 
 @typedmethod(
     path="/decommission/<id>",
-    operation="POST",
-    arg_options={"id": methods.ArgOption(getter=methods.convert_environment)},
-    client_types=[ClientType.api],
-    api_version=2,
-)
-def environment_decommission(id: uuid.UUID, metadata: Optional[model.ModelMetadata] = None) -> int:
-    """
-    Decommission an environment. This is done by uploading an empty model to the server and let purge_on_delete handle
-    removal.
-
-    :param id: The uuid of the environment.
-    :param metadata: Optional metadata associated with the decommissioning
-
-    :raises NotFound: The given environment doesn't exist.
-    :raises Forbidden: The given environment is protected.
-    """
-
-
-@typedmethod(
-    path="/decommission/<id>",
     operation="DELETE",
     arg_options={"id": methods.ArgOption(getter=methods.convert_environment)},
     client_types=[ClientType.api],
     api_version=2,
 )
 def environment_clear(id: uuid.UUID) -> None:
     """
```

### Comparing `inmanta-core-8.5.0/src/inmanta/protocol/openapi/__init__.py` & `inmanta-core-9.3.0/src/inmanta/protocol/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/protocol/openapi/converter.py` & `inmanta-core-9.3.0/src/inmanta/protocol/openapi/converter.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/protocol/openapi/model.py` & `inmanta-core-9.3.0/src/inmanta/protocol/openapi/model.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/protocol/rest/__init__.py` & `inmanta-core-9.3.0/src/inmanta/protocol/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/protocol/rest/client.py` & `inmanta-core-9.3.0/src/inmanta/protocol/rest/client.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/protocol/rest/server.py` & `inmanta-core-9.3.0/src/inmanta/protocol/rest/server.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/protocol/return_value_meta.py` & `inmanta-core-9.3.0/src/inmanta/protocol/return_value_meta.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/reporter.py` & `inmanta-core-9.3.0/src/inmanta/reporter.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/resources.py` & `inmanta-core-9.3.0/src/inmanta/resources.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/__init__.py` & `inmanta-core-9.3.0/src/inmanta/server/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/agentmanager.py` & `inmanta-core-9.3.0/src/inmanta/server/agentmanager.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/bootloader.py` & `inmanta-core-9.3.0/src/inmanta/server/bootloader.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/compilerservice.py` & `inmanta-core-9.3.0/src/inmanta/server/compilerservice.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/config.py` & `inmanta-core-9.3.0/src/inmanta/server/config.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/diff.py` & `inmanta-core-9.3.0/src/inmanta/server/diff.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/extensions.py` & `inmanta-core-9.3.0/src/inmanta/server/extensions.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/protocol.py` & `inmanta-core-9.3.0/src/inmanta/server/protocol.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/server.py` & `inmanta-core-9.3.0/src/inmanta/server/server.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/services/__init__.py` & `inmanta-core-9.3.0/src/inmanta/server/services/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/services/codeservice.py` & `inmanta-core-9.3.0/src/inmanta/server/services/codeservice.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/services/compilerservice.py` & `inmanta-core-9.3.0/src/inmanta/server/services/compilerservice.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/services/databaseservice.py` & `inmanta-core-9.3.0/src/inmanta/server/services/databaseservice.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/services/dryrunservice.py` & `inmanta-core-9.3.0/src/inmanta/server/services/dryrunservice.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/services/environment_metrics_service.py` & `inmanta-core-9.3.0/src/inmanta/server/services/environment_metrics_service.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/services/environmentservice.py` & `inmanta-core-9.3.0/src/inmanta/server/services/environmentservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 )
 from inmanta.server.agentmanager import AgentManager, AutostartedAgentManager
 from inmanta.server.server import Server
 from inmanta.server.services import compilerservice
 from inmanta.server.services.orchestrationservice import OrchestrationService
 from inmanta.server.services.resourceservice import ResourceService
 from inmanta.types import Apireturn, JsonType, Warnings
-from inmanta.util import get_compiler_version
 
 LOGGER = logging.getLogger(__name__)
 
 
 def rename_fields(env: model.Environment) -> JsonType:
     env_dict = env.dict()
     env_dict["project"] = env_dict["project_id"]
@@ -284,23 +283,14 @@
                         return
 
                     await refreshed_env.update_fields(halted=False, connection=connection)
                     await self.agent_manager.resume_agents(refreshed_env, connection=connection)
             await self.autostarted_agent_manager.restart_agents(refreshed_env)
         await self.server_slice.compiler.resume_environment(refreshed_env.id)
 
-    @handle(methods.decomission_environment, env="id")
-    async def decommission_environment(self, env: data.Environment, metadata: Optional[JsonType]) -> Apireturn:
-        data: Optional[model.ModelMetadata] = None
-        if metadata:
-            data = model.ModelMetadata(message=metadata.get("message", ""), type=metadata.get("type", ""))
-
-        version = await self.environment_decommission(env, data)
-        return 200, {"version": version}
-
     @handle(methods.clear_environment, env="id")
     async def clear_environment(self, env: data.Environment) -> Apireturn:
         await self.environment_clear(env)
         return 200
 
     @handle(methods.create_token, env="tid")
     async def create_token(self, env: data.Environment, client_types: List[str], idempotent: bool) -> Apireturn:
@@ -487,27 +477,16 @@
             raise Forbidden(f"Environment {environment_id} is protected. See environment setting: {data.PROTECTED_ENVIRONMENT}")
 
         self._disable_schedules(env)
         await asyncio.gather(self.autostarted_agent_manager.stop_agents(env), env.delete_cascade())
 
         self.resource_service.close_resource_action_logger(environment_id)
         await self.notify_listeners(EnvironmentAction.deleted, env.to_dto())
-        self._delete_environment_dir(environment_id)
 
-    @handle(methods_v2.environment_decommission, env="id")
-    async def environment_decommission(self, env: data.Environment, metadata: Optional[model.ModelMetadata]) -> int:
-        is_protected_environment = await env.get(data.PROTECTED_ENVIRONMENT)
-        if is_protected_environment:
-            raise Forbidden(f"Environment {env.id} is protected. See environment setting: {data.PROTECTED_ENVIRONMENT}")
-        version = await env.get_next_version()
-        if metadata is None:
-            metadata = model.ModelMetadata(message="Decommission of environment", type="api")
-        version_info = model.ModelVersionInfo(export_metadata=metadata)
-        await self.orchestration_service.put_version(env, version, [], {}, [], version_info.dict(), get_compiler_version())
-        return version
+        self._delete_environment_dir(environment_id)
 
     @handle(methods_v2.environment_clear, env="id")
     async def environment_clear(self, env: data.Environment) -> None:
         """
         Clear the environment
         """
         is_protected_environment = await env.get(data.PROTECTED_ENVIRONMENT)
```

### Comparing `inmanta-core-8.5.0/src/inmanta/server/services/fileservice.py` & `inmanta-core-9.3.0/src/inmanta/server/services/fileservice.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/services/metricservice.py` & `inmanta-core-9.3.0/src/inmanta/server/services/metricservice.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/services/notificationservice.py` & `inmanta-core-9.3.0/src/inmanta/server/services/notificationservice.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/services/orchestrationservice.py` & `inmanta-core-9.3.0/src/inmanta/server/services/orchestrationservice.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import asyncpg
 import asyncpg.connection
 import asyncpg.exceptions
 import pydantic
 
 from inmanta import const, data
 from inmanta.const import ResourceState
-from inmanta.data import APILIMIT, AVAILABLE_VERSIONS_TO_KEEP, ENVIRONMENT_AGENT_TRIGGER_METHOD, PURGE_ON_DELETE, InvalidSort
+from inmanta.data import APILIMIT, AVAILABLE_VERSIONS_TO_KEEP, ENVIRONMENT_AGENT_TRIGGER_METHOD, InvalidSort
 from inmanta.data.dataview import DesiredStateVersionView
 from inmanta.data.model import (
     DesiredStateVersion,
     PromoteTriggerMethod,
     ResourceDiff,
     ResourceIdStr,
     ResourceMinimal,
@@ -626,16 +626,15 @@
         removed_resource_sets: Optional[List[str]] = None,
         *,
         connection: asyncpg.connection.Connection,
     ) -> None:
         """
         :param rid_to_resource: This parameter should contain all the resources when a full compile is done.
                                 When a partial compile is done, it should contain all the resources that belong to the
-                                updated resource sets or the shared resource sets. This method updates this object with
-                                purge-on-delete resources.
+                                updated resource sets or the shared resource sets.
         :param unknowns: This parameter should contain all the unknowns for all the resources in the new version of the model.
                          Also the unknowns for resources that are not present in rid_to_resource.
         :param partial_base_version: When a partial compile is done, this parameter contains the version of the
                                      configurationmodel this partial compile was based on. Otherwise this parameter should be
                                      None.
         :param removed_resource_sets: When a partial compile is done, this parameter should indicate the names of the resource
                                       sets that are removed by the partial compile. When no resource sets are removed by
@@ -645,21 +644,14 @@
             * The requires and provides relationships of the resources in rid_to_resource must be set correctly. For a
               partial compile, this means it is assumed to be valid with respect to all absolute constraints that apply to
               partial compiles. Constraints that are relative to the base version will be verified by this method.
             * When a partial compile was done, all resources in rid_to_resource must meet the constraints of a partial compile.
             * The resource sets defined in the removed_resource_sets argument must not overlap with the resource sets present
               in the resource_sets argument.
 
-        This method adds resources to the model that are no longer present in the new version of the model and had the
-        purge_on_delete flag set to true. This method makes sure that the requires and provides relationships of these
-        additional resources are set correctly. This dependency wiring is also safe for a partial compile because
-        a partial compile cannot delete shared resources and because resources that belong to a non-shared resource set cannot
-        reference resources in another non-shared resource set. That way all dependencies of the deleted resources are present
-        in the rid_to_resource parameter.
-
         When a partial compile is done, the undeployable and skipped_for_undeployable resources of a configurationmodel are
         copied from the old version to the new version. This operation is safe because the only resources missing from
         rid_to_resource are resources that belong to an unchanged, non-shared resource set. Those resources can only have
         cross resource set dependencies in a non-shared resource set and the latter resource set cannot be changed by a partial
         compile.
 
         Validations done by this method:
@@ -765,25 +757,14 @@
                         f"    {rid} moved from {rids_unchanged_resource_sets[rid]} to {resource_sets[rid]}"
                         for rid in resources_that_moved_resource_sets
                     )
 
                     raise BadRequest(msg)
                 all_ids |= {Id.parse_id(rid, version) for rid in rids_unchanged_resource_sets.keys()}
 
-            purge_on_delete_resources: Dict[ResourceIdStr, data.Resource] = await self._get_resources_for_purge_on_delete(
-                env=env,
-                version=version,
-                rid_to_resource=rid_to_resource,
-                all_resource_ids=[i.resource_str() for i in all_ids],
-                version_info=version_info,
-                connection=connection,
-            )
-            rid_to_resource.update(purge_on_delete_resources)
-            all_ids |= {Id.parse_id(rid, version) for rid in purge_on_delete_resources.keys()}
-
             await data.Resource.insert_many(list(rid_to_resource.values()), connection=connection)
             await cm.recalculate_total(connection=connection)
 
             await data.UnknownParameter.insert_many(unknowns, connection=connection)
 
             all_agents: abc.Set[str] = {res.agent for res in rid_to_resource.values()}
             for agent in all_agents:
@@ -806,91 +787,14 @@
                     finished=now,
                     messages=[log_line],
                 )
                 await ra.insert(connection=connection)
 
         LOGGER.debug("Successfully stored version %d", version)
 
-    async def _get_resources_for_purge_on_delete(
-        self,
-        env: data.Environment,
-        version: int,
-        rid_to_resource: abc.Mapping[ResourceIdStr, data.Resource],
-        all_resource_ids: abc.Sequence[ResourceIdStr],
-        version_info: Optional[JsonType] = None,
-        *,
-        connection: asyncpg.connection.Connection,
-    ) -> dict[ResourceIdStr, data.Resource]:
-        """
-        Return a dictionary of resources that were present in the old version of the model but that no longer exist in this
-        version (in rid_to_resource) and had the purge_on_delete flag set to true. The returned resources will have the purged
-        attribute set to True and their requires/provides relationships inverted.
-
-        :param env: The environment we are discovering purged resources for.
-        :param version: The new version of the configuration model in which the purge_on_delete resources should be added.
-        :param rid_to_resource: When a full compile is done, this dictionary contains an entry for all resources that are
-                                part of the full compile. When a partial compile is done, this dictionary contains an entry
-                                for each resource in the new version of the model that belongs to an updated or shared
-                                resource set.
-        :param all_resource_ids: All the resource ids of all the resources present in the new version of the model. When
-                                 a partial compile is done, this sequence also includes the resource ids of resources that were
-                                 not updated by the partial compile.
-        """
-
-        def safe_get(input: object, key: str, default: object) -> object:
-            if not isinstance(input, dict):
-                return default
-            if key not in input:
-                return default
-            return input[key]
-
-        rid_to_resource = dict(rid_to_resource)
-
-        # detect failed compiles
-        metadata: object = safe_get(version_info, const.EXPORT_META_DATA, {})
-        compile_state = safe_get(metadata, const.META_DATA_COMPILE_STATE, "")
-        failed = compile_state == const.Compilestate.failed
-
-        result = {}
-        if not failed and (await env.get(PURGE_ON_DELETE)):
-            # search for deleted resources (purge_on_delete)
-            resources_to_purge: List[data.Resource] = await data.Resource.get_deleted_resources(
-                env.id, version, all_resource_ids, connection=connection
-            )
-
-            previous_requires = {}
-            for res in resources_to_purge:
-                LOGGER.warning("Purging %s, purged resource based on %s", res.resource_id, res.resource_version_id)
-
-                attributes = res.attributes.copy()
-                attributes["purged"] = True
-                attributes["requires"] = []
-                res_obj = data.Resource.new(
-                    env.id,
-                    resource_version_id=ResourceVersionIdStr("%s,v=%s" % (res.resource_id, version)),
-                    attributes=attributes,
-                )
-
-                previous_requires[res_obj.resource_id] = res.attributes["requires"]
-                rid_to_resource[res_obj.resource_id] = res_obj
-                result[res_obj.resource_id] = res_obj
-
-            # invert dependencies on purges
-            for res_id, requires in previous_requires.items():
-                res_obj = rid_to_resource[res_id]
-                for require in requires:
-                    req_id = Id.parse_id(require)
-
-                    if req_id.resource_str() in rid_to_resource:
-                        req_res = rid_to_resource[req_id.resource_str()]
-                        req_res.attributes["requires"].append(res_obj.resource_id)
-                        if res_obj.agent != req_res.agent:
-                            res_obj.provides.append(req_res.resource_id)
-        return result
-
     async def _trigger_auto_deploy(
         self,
         env: data.Environment,
         version: int,
     ) -> None:
         """
         Triggers auto-deploy for stored resources. Must be called only after transaction that stores resources has been allowed
```

### Comparing `inmanta-core-8.5.0/src/inmanta/server/services/paramservice.py` & `inmanta-core-9.3.0/src/inmanta/server/services/paramservice.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/services/projectservice.py` & `inmanta-core-9.3.0/src/inmanta/server/services/projectservice.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/services/resourceservice.py` & `inmanta-core-9.3.0/src/inmanta/server/services/resourceservice.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/services/userservice.py` & `inmanta-core-9.3.0/src/inmanta/server/services/userservice.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/server/validate_filter.py` & `inmanta-core-9.3.0/src/inmanta/server/validate_filter.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/stable_api.py` & `inmanta-core-9.3.0/src/inmanta/stable_api.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/types.py` & `inmanta-core-9.3.0/src/inmanta/types.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/user_setup.py` & `inmanta-core-9.3.0/src/inmanta/user_setup.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/util.py` & `inmanta-core-9.3.0/src/inmanta/util.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta/warnings.py` & `inmanta-core-9.3.0/src/inmanta/warnings.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta_core.egg-info/PKG-INFO` & `inmanta-core-9.3.0/src/inmanta_core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmanta-core
-Version: 8.5.0
+Version: 9.3.0
 Summary: Inmanta deployment tool
 Home-page: https://github.com/inmanta/inmanta-core
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License 2
 Project-URL: Bug Tracker, https://github.com/inmanta/inmanta-core/issues
 Project-URL: Documentation, https://docs.inmanta.com/community/latest/
```

### Comparing `inmanta-core-8.5.0/src/inmanta_core.egg-info/SOURCES.txt` & `inmanta-core-9.3.0/src/inmanta_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 src/inmanta/db/versions/v202301160.py
 src/inmanta/db/versions/v202301170.py
 src/inmanta/db/versions/v202301190.py
 src/inmanta/db/versions/v202302200.py
 src/inmanta/db/versions/v202302270.py
 src/inmanta/db/versions/v202303070.py
 src/inmanta/db/versions/v202303071.py
+src/inmanta/db/versions/v202304060.py
 src/inmanta/db/versions/v202304070.py
 src/inmanta/db/versions/v202306060.py
 src/inmanta/db/versions/v3.py
 src/inmanta/db/versions/v4.py
 src/inmanta/db/versions/v5.py
 src/inmanta/db/versions/v6.py
 src/inmanta/db/versions/v7.py
```

### Comparing `inmanta-core-8.5.0/src/inmanta_core.egg-info/requires.txt` & `inmanta-core-9.3.0/src/inmanta_core.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 [datatrace]
 graphviz
 
 [debug]
 rpdb
 
 [pytest-inmanta-extensions]
-pytest-inmanta-extensions~=8.5.0.0.dev
+pytest-inmanta-extensions~=9.3.0.0.dev
```

### Comparing `inmanta-core-8.5.0/src/inmanta_ext/core/__init__.py` & `inmanta-core-9.3.0/src/inmanta_ext/core/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta_ext/core/extension.py` & `inmanta-core-9.3.0/src/inmanta_ext/core/extension.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/src/inmanta_plugins/1/__init__.py` & `inmanta-core-9.3.0/src/inmanta_plugins/1/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_2way_protocol.py` & `inmanta-core-9.3.0/tests/test_2way_protocol.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_agent.py` & `inmanta-core-9.3.0/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_agent_manager.py` & `inmanta-core-9.3.0/tests/test_agent_manager.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_app.py` & `inmanta-core-9.3.0/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_app_cli.py` & `inmanta-core-9.3.0/tests/test_app_cli.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_cache.py` & `inmanta-core-9.3.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_cli.py` & `inmanta-core-9.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_compilation.py` & `inmanta-core-9.3.0/tests/test_compilation.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_compiler_entrypoints.py` & `inmanta-core-9.3.0/tests/test_compiler_entrypoints.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_config.py` & `inmanta-core-9.3.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_const.py` & `inmanta-core-9.3.0/tests/test_const.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_data.py` & `inmanta-core-9.3.0/tests/test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1198,163 +1198,14 @@
     res4 = get_resource(4, [3])
     await res4.insert()
 
     res5 = get_resource(5, [4])
     await res5.insert()
 
 
-async def test_resource_purge_on_delete(init_dataclasses_and_load_schema):
-    project = data.Project(name="test")
-    await project.insert()
-
-    env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
-    await env.insert()
-
-    # model 1
-    version = 1
-    cm1 = data.ConfigurationModel(
-        environment=env.id,
-        version=version,
-        date=datetime.datetime.now(),
-        total=2,
-        version_info={},
-        released=True,
-        deployed=True,
-        is_suitable_for_partial_compiles=False,
-    )
-    await cm1.insert()
-
-    res11 = data.Resource.new(
-        environment=env.id,
-        resource_version_id="std::File[agent1,path=/etc/motd],v=%s" % version,
-        status=const.ResourceState.deployed,
-        attributes={"path": "/etc/motd", "purge_on_delete": True, "purged": False},
-    )
-    await res11.insert()
-
-    res12 = data.Resource.new(
-        environment=env.id,
-        resource_version_id="std::File[agent2,path=/etc/motd],v=%s" % version,
-        status=const.ResourceState.deployed,
-        attributes={"path": "/etc/motd", "purge_on_delete": True, "purged": True},
-    )
-    await res12.insert()
-
-    # model 2 (multiple undeployed versions)
-    while version < 10:
-        version += 1
-        cm2 = data.ConfigurationModel(
-            environment=env.id,
-            version=version,
-            date=datetime.datetime.now(),
-            total=1,
-            version_info={},
-            released=False,
-            deployed=False,
-            is_suitable_for_partial_compiles=False,
-        )
-        await cm2.insert()
-
-        res21 = data.Resource.new(
-            environment=env.id,
-            resource_version_id="std::File[agent5,path=/etc/motd],v=%s" % version,
-            status=const.ResourceState.available,
-            attributes={"path": "/etc/motd", "purge_on_delete": True, "purged": False},
-        )
-        await res21.insert()
-
-    # model 3
-    version += 1
-    cm3 = data.ConfigurationModel(
-        environment=env.id,
-        version=version,
-        date=datetime.datetime.now(),
-        total=0,
-        version_info={},
-        is_suitable_for_partial_compiles=False,
-    )
-    await cm3.insert()
-
-    to_purge = await data.Resource.get_deleted_resources(env.id, version, set())
-
-    assert len(to_purge) == 1
-    assert to_purge[0].model == 1
-    assert to_purge[0].resource_id == "std::File[agent1,path=/etc/motd]"
-
-
-async def test_issue_422(init_dataclasses_and_load_schema):
-    project = data.Project(name="test")
-    await project.insert()
-
-    env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
-    await env.insert()
-
-    # model 1
-    version = 1
-    cm1 = data.ConfigurationModel(
-        environment=env.id,
-        version=version,
-        date=datetime.datetime.now(),
-        total=1,
-        version_info={},
-        released=True,
-        deployed=True,
-        is_suitable_for_partial_compiles=False,
-    )
-    await cm1.insert()
-
-    res11 = data.Resource.new(
-        environment=env.id,
-        resource_version_id="std::File[agent1,path=/etc/motd],v=%s" % version,
-        status=const.ResourceState.deployed,
-        attributes={"path": "/etc/motd", "purge_on_delete": True, "purged": False},
-    )
-    await res11.insert()
-
-    # model 2 (multiple undeployed versions)
-    version += 1
-    cm2 = data.ConfigurationModel(
-        environment=env.id,
-        version=version,
-        date=datetime.datetime.now(),
-        total=1,
-        version_info={},
-        released=False,
-        deployed=False,
-        is_suitable_for_partial_compiles=False,
-    )
-    await cm2.insert()
-
-    res21 = data.Resource.new(
-        environment=env.id,
-        resource_version_id="std::File[agent1,path=/etc/motd],v=%s" % version,
-        status=const.ResourceState.available,
-        attributes={"path": "/etc/motd", "purge_on_delete": True, "purged": False},
-    )
-    await res21.insert()
-
-    # model 3
-    version += 1
-    cm3 = data.ConfigurationModel(
-        environment=env.id,
-        version=version,
-        date=datetime.datetime.now(),
-        total=0,
-        version_info={},
-        is_suitable_for_partial_compiles=False,
-    )
-    await cm3.insert()
-
-    to_purge = await data.Resource.get_deleted_resources(env.id, version, set())
-
-    assert len(to_purge) == 1
-    assert to_purge[0].model == 1
-    assert to_purge[0].resource_id == "std::File[agent1,path=/etc/motd]"
-
-
 async def test_get_latest_resource(init_dataclasses_and_load_schema, postgresql_client):
     project = data.Project(name="test")
     await project.insert()
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env.insert()
```

### Comparing `inmanta-core-8.5.0/tests/test_data_concurrency.py` & `inmanta-core-9.3.0/tests/test_data_concurrency.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_data_model.py` & `inmanta-core-9.3.0/tests/test_data_model.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_deploy.py` & `inmanta-core-9.3.0/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_discovered_resources.py` & `inmanta-core-9.3.0/tests/test_discovered_resources.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_docs_snippets.py` & `inmanta-core-9.3.0/tests/test_docs_snippets.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_docstring_parser.py` & `inmanta-core-9.3.0/tests/test_docstring_parser.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_env.py` & `inmanta-core-9.3.0/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_export.py` & `inmanta-core-9.3.0/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_extension_loading.py` & `inmanta-core-9.3.0/tests/test_extension_loading.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_file_parser.py` & `inmanta-core-9.3.0/tests/test_file_parser.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_handler.py` & `inmanta-core-9.3.0/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_import_entry_points.py` & `inmanta-core-9.3.0/tests/test_import_entry_points.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_influxdbreporting.py` & `inmanta-core-9.3.0/tests/test_influxdbreporting.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_io.py` & `inmanta-core-9.3.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_jwt.py` & `inmanta-core-9.3.0/tests/test_jwt.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_loader.py` & `inmanta-core-9.3.0/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_logging.py` & `inmanta-core-9.3.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_module_loader.py` & `inmanta-core-9.3.0/tests/test_module_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,17 +170,22 @@
             snippet=f"import {module_name}",
             install_project=True,
             python_package_sources=[],
             python_requires=[
                 InmantaModuleRequirement.parse(module_name).get_python_package_requirement(),
             ],
         )
+
     message: str = (
-        "Attempting to install a v2 module non_existing_module but no v2 module source is configured. Add at least one repo of "
-        'type "package" to the project config file.'
+        "Attempting to install a v2 module non_existing_module but no v2 module source is configured. Add the relevant pip "
+        "indexes to the project config file. e.g. to add PyPi as a module source, add the following to "
+        "the `pip` section of the project's `project.yml`:"
+        "\n\t  index_urls:"
+        "\n\t\t  - https://pypi.org/simple"
+        "\nAnother option is to set the use_config_file project option to true to use the system's pip config file."
     )
     assert message in e.value.format_trace()
 
 
 @pytest.mark.parametrize("allow_v1", [True, False])
 def test_load_module_v1_already_installed(snippetcompiler, modules_dir: str, allow_v1: bool) -> None:
     """
```

### Comparing `inmanta-core-8.5.0/tests/test_modules.py` & `inmanta-core-9.3.0/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_openapi.py` & `inmanta-core-9.3.0/tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_param.py` & `inmanta-core-9.3.0/tests/test_param.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_parser.py` & `inmanta-core-9.3.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_postgres.py` & `inmanta-core-9.3.0/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_postgres_proc.py` & `inmanta-core-9.3.0/tests/test_postgres_proc.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_project.py` & `inmanta-core-9.3.0/tests/test_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,18 +208,14 @@
     # Operation on non existing
     result = await client_v2.environment_get(id=uuid.uuid4())
     assert result.code == 404
 
     result = await client_v2.environment_delete(id=uuid.uuid4())
     assert result.code == 404
 
-    # Decommission
-    result = await client_v2.environment_decommission(id=env1_id)
-    assert result.code == 200
-
 
 async def test_modify_environment_project(client_v2):
     """Test modifying the project of an environment"""
 
     # Create two projects and two environments
     result = await client_v2.project_create("dev-project")
     assert result.code == 200
@@ -394,18 +390,14 @@
     result = await client_v2.environment_get(id=env1_id)
     assert result.code == 200
     assert result.result["data"]["name"] == "dev"
 
     result = await client_v2.environment_delete(id=uuid.uuid4())
     assert result.code == 404
 
-    # Decommission
-    result = await client_v2.environment_decommission(id=env1_id)
-    assert result.code == 200
-
     # Clear
     result = await client_v2.environment_clear(id=env1_id)
     assert result.code == 200
 
     # Delete
     result = await client_v2.environment_delete(id=env1_id)
     assert result.code == 200
```

### Comparing `inmanta-core-8.5.0/tests/test_projectmetadata.py` & `inmanta-core-9.3.0/tests/test_projectmetadata.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 import logging
 from typing import List, Optional
 
 import pytest
 
 from inmanta.module import ModuleRepoType, Project, ProjectMetadata, RelationPrecedenceRule
-from utils import assert_no_warning
+from utils import assert_no_warning, log_contains
 
 
 @pytest.mark.parametrize(
     "repo",
     [
         ("https://github.com/inmanta/{}.git"),
         ("git@github.com:inmanta/{}.git"),
@@ -86,15 +86,76 @@
 def test_no_module_path(tmp_path, caplog):
     with caplog.at_level(logging.WARNING):
         with (tmp_path / "project.yml").open("w") as fh:
             fh.write(
                 """
     name: testproject
     downloadpath: libs
+    pip:
+        index_urls:
+            - https://pypi.org/simple
+    """
+            )
+
+        Project(tmp_path, autostd=False)
+    assert_no_warning(caplog)
+
+
+def test_deprecation_warning_repo_of_type_package(tmp_path, caplog):
+    with caplog.at_level(logging.WARNING):
+        with (tmp_path / "project.yml").open("w") as fh:
+            fh.write(
+                """
+    name: testproject
+    downloadpath: libs
     repo:
-        - url: https://pypi.org/simple
-          type: package
+       - url: https://pypi.org/simple
+         type: package
+    pip:
+        index_urls:
+            - https://pypi.org/simple
     """
             )
 
         Project(tmp_path, autostd=False)
+    log_contains(
+        caplog,
+        "inmanta.module",
+        logging.WARNING,
+        (
+            "Setting a pip index through the `repo -> url` option with type `package` in the project.yml file is deprecated. "
+            "Please set the pip index url through the `pip -> index_urls` option instead."
+        ),
+    )
+
+
+@pytest.mark.parametrize("use_pip_config_file, value", [(True, True), (True, False), (False, False)])
+def test_pip_config(tmp_path, caplog, use_pip_config_file, value):
+    """
+    Verify that "use_config_file" can be specified in a project.yml file but that it isn't mandatory
+    If it is not specified, verify that the default value "False" is used in the project.
+    """
+    pip_config_file = """
+    pip:
+        index_urls:
+            - https://pypi.org/simple
+
+    """
+    pip_config_file += (
+        f"""
+        use_config_file: {value}
+        """
+        if use_pip_config_file
+        else ""
+    )
+    with caplog.at_level(logging.WARNING):
+        with (tmp_path / "project.yml").open("w") as fh:
+            fh.write(
+                f"""
+    name: testproject
+    downloadpath: libs
+    {pip_config_file}
+    """
+            )
+    project = Project(tmp_path, autostd=False)
     assert_no_warning(caplog)
+    assert project.metadata.pip.use_config_file == value
```

### Comparing `inmanta-core-8.5.0/tests/test_protocol.py` & `inmanta-core-9.3.0/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_proxy.py` & `inmanta-core-9.3.0/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_resource.py` & `inmanta-core-9.3.0/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_server.py` & `inmanta-core-9.3.0/tests/test_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1442,14 +1442,21 @@
     await env1.insert()
     env2 = data.Environment(name="env2", project=project.id)
     await env2.insert()
 
     await env1.set(data.AUTOSTART_AGENT_MAP, {"agent3": "", "internal": ""})
     await env2.set(data.AUTOSTART_AGENT_MAP, {"agent1": "", "internal": ""})
 
+    # these checks are here to investigate the fact that the test case is flaky and that we have a suspicion
+    # that it is an issue with the agent map
+    agentmap_env1 = await client.get_setting(tid=env1.id, id=data.AUTOSTART_AGENT_MAP)
+    agentmap_env2 = await client.get_setting(tid=env2.id, id=data.AUTOSTART_AGENT_MAP)
+    assert agentmap_env1.result["value"] == {"agent3": "", "internal": ""}
+    assert agentmap_env2.result["value"] == {"agent1": "", "internal": ""}
+
     if env1_halted:
         result = await client.halt_environment(env1.id)
         assert result.code == 200
     if env2_halted:
         result = await client.halt_environment(env2.id)
         assert result.code == 200
 
@@ -1514,15 +1521,30 @@
         paused=False,
         id_primary=None,
     ).insert()
 
     agents_before_purge = await data.Agent.get_list()
     assert len(agents_before_purge) == 6
 
+    # these checks are here to investigate the fact that the test case is flaky and that we have a suspicion
+    # that it is an issue with the agent map
+    agentmap_env1 = await client.get_setting(tid=env1.id, id=data.AUTOSTART_AGENT_MAP)
+    agentmap_env2 = await client.get_setting(tid=env2.id, id=data.AUTOSTART_AGENT_MAP)
+    assert agentmap_env1.result["value"] == {"agent3": "", "internal": ""}
+    assert agentmap_env2.result["value"] == {"agent1": "", "internal": ""}
+
     await server.get_slice(SLICE_ORCHESTRATION)._purge_versions()
+
+    # these checks are here to investigate the fact that the test case is flaky and that we have a suspicion
+    # that it is an issue with the agent map
+    agentmap_env1 = await client.get_setting(tid=env1.id, id=data.AUTOSTART_AGENT_MAP)
+    agentmap_env2 = await client.get_setting(tid=env2.id, id=data.AUTOSTART_AGENT_MAP)
+    assert agentmap_env1.result["value"] == {"agent3": "", "internal": ""}
+    assert agentmap_env2.result["value"] == {"agent1": "", "internal": ""}
+
     agents_after_purge = [(agent.environment, agent.name) for agent in await data.Agent.get_list()]
     number_agents_env1_after_purge = 4 if env1_halted else 3
     number_agents_env2_after_purge = 2 if env2_halted else 1
     assert len(agents_after_purge) == number_agents_env1_after_purge + number_agents_env2_after_purge
     if not (env1_halted or env2_halted):
         expected_agents_after_purge = [
             (env1.id, "agent2"),
```

### Comparing `inmanta-core-8.5.0/tests/test_type.py` & `inmanta-core-9.3.0/tests/test_type.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_usersetup.py` & `inmanta-core-9.3.0/tests/test_usersetup.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tests/test_util.py` & `inmanta-core-9.3.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.5.0/tox.ini` & `inmanta-core-9.3.0/tox.ini`

 * *Files identical despite different names*

